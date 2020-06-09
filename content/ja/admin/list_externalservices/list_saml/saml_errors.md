---
title: "SAML認証のトラブルシューティング"
weight: 400
---
SAML認証に関するトラブルの解決方法を説明します。  

{{% warning %}}
{{% subtitle %}}
Identity Provider（IdP）にActive Directory Federation Services（ADFS）2.0を使用している場合の注意
{{% /subtitle %}}
{{%service%}}からログアウトし、同じWebブラウザーで再度{{%service%}}にアクセスすると、ログイン後の画面が表示される場合があります。  
この現象はADFSにCookieが残存するために発生します。ログイン後の画面が表示されても、{{%service%}}からのログアウト自体は成功しています。  
ログアウト後にWebブラウザーを再起動してから、{{%service%}}にアクセスしてください。  
{{% /warning %}}

## SAML認証の設定ミスでログインできなくなった場合 {#list_saml_saml_errors_10}

SAML認証に失敗すると、ユーザーは{{%service%}}にログインできません。  
ただし、{{%slash%}}共通管理者だけは、下記URLから{{%service%}}標準の認証を利用して、{{%service%}}にログインできます。

1. SAML認証を無効にするURLにアクセスします。  
  https://（サブドメイン名）.{{%cybozu_com%}}/login?saml=off  
  管理者以外のユーザーにも、このURLの利用を許可する場合は、ログイン時にSAML認証だけを使う制限を無効にする必要があります。  
  詳細は、[ログイン時にSAML認証だけを使うように制限する](/general/ja/admin/list_externalservices/list_saml/saml_restriction.html)を参照してください。  

1. {{%slash%}}共通管理に登録しているログイン名とパスワードを入力し、{{%service%}}にログインします。  

## SAML認証に関するエラー {#list_saml_saml_errors_20}

<table>
    <thead>
        <tr>
            <th width="10%" scope="col"><b>エラーコード</b></th>
            <th width="23%" scope="col"><b>エラーメッセージ</b></th>
            <th width="32%" scope="col"><b>原因</b></th>
            <th width="35%" scope="col"><b>対処</b></th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>SLASH_SA01</td>
            <td>SAMLResponse内のNameIDと一致するログイン名を持つユーザーが見つかりません。</td>
            <td>SAMLResponse内のNameIDと一致するログイン名を持つユーザーが、{{%service%}}に存在しません。</td>
            <td>
            <ul>
                <li>IdPの設定を変更し、ユーザーを識別する要素にNameIDを指定してください。</li>
                <li>NameIDに関連付けた値と、{{%service%}}のユーザーのログイン名を一致させてください。</li>
            </ul>
            </td>
        </tr>
        <tr>
            <td>SLASH_SA02</td>
            <td>SAMLResponseに対応するAuthnRequestがありません。</td>
            <td>次のような場合に発生します。<br />
            <ul>
                <li>1つのセッションで複数のSAMLリクエストを発行した。<br />
                例:<br />
                <ul>
                    <li>同じWebブラウザーの複数のタブで、SSOを行おうとした。</li>
                    <li>SSO後に、Webブラウザーの戻るボタンをクリックし、{{%service%}}のエンドポイントURLを表示しようとした。</li>
                </ul>
                </li>
                <li>IdP InitiatedなSSOを行おうとした。</li>
            </ul>
            </td>
            <td>
            <ul>
                <li>1つのセッションで、複数のSAMLリクエストを発行する操作をしないでください。</li>
                <li>IdPの設定を変更し、SP InitiatedなSSOを行ってください。</li>
            </ul>
            </td>
        </tr>
        <tr>
            <td>SLASH_SA03</td>
            <td>リクエストパラメータにSAMLResponseがありません。</td>
            <td>IdPが{{%service%}}に送信したリクエストパラメータに、SAMLResponseがありません。</td>
            <td>SAMLResponseの送信を妨げるものがないか確認してください。</td>
        </tr>
        <tr>
            <td>SLASH_SA04</td>
            <td>SAMLResponseが無効です。</td>
            <td>SAMLResponse内のResponse要素の内容が無効です。</td>
            <td>検証結果がFailedの項目の設定を見直してください。<br />
            次の情報も参考にしてください。<br />
           <a href="#list_saml_saml_errors_30">SAMLResposeの検証結果を確認する</a></td>
        </tr>
        <tr>
            <td>SLASH_SA05</td>
            <td>HTTPメソッドが不正です。HTTPメソッドにPOSTを指定してください。</td>
            <td>HTTP POST Binding以外で、SAMLレスポンスを送信しています。</td>
            <td>
            <ul>
                <li>IdPの設定を変更し、HTTP POST BindingでSAMLレスポンスを送信してください。</li>
                <li>プロキシサーバーなどで、HTTPメソッドがPOST以外のものに変換されていないかどうか確認してください。</li>
            </ul>
            </td>
        </tr>
        <tr>
            <td>SLASH_FA01</td>
            <td>SAMLResponseの処理に失敗しました。</td>
            <td>予期せぬエラーが発生し、SAMLResponseを処理できません。</td>
            <td>お手数ですが{{%CorpName%}}までお問い合わせください。</td>
        </tr>
    </tbody>
</table>

## SAMLResponseの検証結果を確認する {#list_saml_saml_errors_30}

SAMLResponseの検証結果がFailedとなった場合、検証項目ごとに次の対処を行います。

* <b>現在の時刻が、Conditions要素のNotBefore属性とNotOnOrAfter属性で指定した期間内である場合</b><br>
  IdPと{{%service%}}の日時の設定が異なる可能性があります。IdPの設定を変更し、正しい日時を設定します。
* <b>SubjectConfirmationData要素のInResponseTo属性がAuthnRequestのIDと一致する場合</b><br>
  同じWebブラウザーの複数のタブで、SSOを行おうとした可能性があります。タブをひとつだけ開いた状態でログインした場合に、エラーが解消するかどうかを確認します。
* <b>Audience要素に正しい値が指定されている場合</b><br>
  {{%service%}}をSPとして登録する際に、不正なエンティティIDを指定した可能性があります。SPのエンティティIDには、「https://（サブドメイン名）.{{%cybozu_com%}}」を指定します。
* <b>Assertion要素またはResponse要素に署名があり、その署名が有効である場合</b><br>
  公開鍵の証明書が不正な可能性があります。{{%slash%}}共通管理の「ログインのセキュリティ設定」画面で、「Identity Providerが署名に使用する公開鍵の証明書」に正しい証明書を添付します。証明書はRSAかDSAのアルゴリズムで生成した、X.509形式のものを使用します。
