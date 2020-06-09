---
title: "ユーザーを追加する"
weight: 100
---
サービスを利用するユーザーを追加します。ここでは、ひとりずつユーザーを追加する方法を説明します。

{{% note %}}
CSVファイルを読み込んでユーザー情報を一括登録することもできます。  
[ユーザーを一括で登録、編集する](/general/ja/admin/list_useradmin/list_csv/user.html)  方法を参照してください。  
一括登録する場合、ユーザーにパスワードとログイン方法をメールで通知する機能はありません。
{{% /note %}}

{{% enabled JP %}}

1. 「{{%slash%}}共通管理」画面の「ユーザー管理」の、[組織/ユーザー]をクリックします。  
    {{< screen src="/general/img-ja/add_user_img01.png" alt="[組織/ユーザー]が赤枠で囲まれた画像">}}

1. 組織のボックスから、ユーザーを追加する組織を選択します。  
  先に[未所属のユーザー]にユーザーを登録し、あとで組織を追加して、ユーザーに設定することもできます。  
  {{< screen src="/general/img-ja/add_user_img02.png" alt="組織とユーザーの設定画面">}}
  組織を追加するには、[組織の追加]をクリックします。詳細は、[組織を追加する](/general/ja/admin/list_useradmin/list_division/add_division.html)を参照してください。  

1. 「ユーザー」欄の[ユーザーの追加]をクリックします。
    {{< screen src="/general/img-ja/add_user_img03.png" alt="[ユーザーの追加]が赤枠で囲まれた画像">}}

1. 必要な項目を設定します。  
  項目の詳細は、[ユーザー情報の設定画面](/general/ja/admin/list_useradmin/list_user/user_details.html)を参照してください。  
  次の項目は、必ず設定してください。
   <table >
      <thead>
          <tr>
              <th width="130" scope="col">項目名</th>
              <th scope="col">内容</th>
          </tr>
      </thead>
      <tbody>
          <tr>
              <td>表示名</td>
              <td>各サービスで表示される名前です。</td>
          </tr>
          <tr>
              <td>ログイン名</td>
              <td>{{%service%}}にログインするためのIDです。<br />
              <ul>
                  <li>他のユーザーと重複するログイン名は使用できません。</li>
                  <li>ログイン名には次の文字を使用できません。<br />
                  \ [ ] &quot; : ; < >, /</li>
                  <li>先頭または最後が半角スペースや全角スペースのログイン名は設定できません。</li>
              </ul>
              </td>
          </tr>
          <tr>
              <td>E-mail</td>
              <td>各サービスでメールの送受信に使用するメールアドレスです。<br />
              このメールアドレスは、パスワードを忘れた際のパスワードリセットに使用されます。複数のユーザーで共有しているメールアドレスは設定しないでください。</td>
          </tr>
          <tr>
              <td>使用状態</td>
              <td>「使用中」になっていることを確認します。<br />
              「停止中」の場合は、サービスを利用できません。</td>
          </tr>
          <tr>
              <td>利用サービス</td>
              <td>契約中、または試用を申し込んでいるサービスの一覧です。<br />
              該当ユーザーの利用するサービスのチェックボックスを選択します。<br />
              <a href="/general/ja/admin/list_useradmin/list_user/service_user.html">ユーザーが利用するサービスを設定する</a></td>
          </tr>
      </tbody>
    </table>

1. [保存]をクリックします。  
  {{< screen src="/general/img-ja/add_user_img04.png" alt="ユーザーの追加画面">}}

1. 「パスワードの設定」ダイアログで、追加したユーザーのパスワードを設定します。

   * パスワードは自動生成か、直接入力で設定します。
   * 「パスワードを表示する」を選択すると、ユーザーのパスワードを確認できます。  
     ただし、Internet Explorer 8ではこのチェックボックスは表示されません。
   * 「このユーザーのパスワードを無期限にする」を選択すると、パスワードポリシーの設定に関わらず、選択したユーザーのパスワードのみ、有効期間を無期限にできます。

    {{< screen src="/general/img-ja/add_user_img05.png" alt="「パスワードの設定」ダイアログの画像">}}

1. ユーザーへパスワードとログインの仕方を通知する方法を選びます。  

    1. **メールで通知する場合**  
      [設定してメールを送信]をクリックし、手順8に進みます。  
      メールで通知する場合、[管理者が設定した仮パスワードの変更を許可する](/general/ja/admin/list_security/list_login/pw_allow.html#list_login_pw_allow_10)ことを推奨します。
      初期設定では有効になっています。  
    1. **メールで通知しない場合**  
      [設定]をクリックし、ユーザー情報を保存します。  
      サービスを利用するユーザーに次の情報を伝えます。  
      * 利用するサービスのアクセスURL  
        例：https://（サブドメイン名）.{{%cybozu_com%}}/
      * ログイン名
      * パスワード  

1. 「パスワードとログイン方法をメールで送信」ダイアログで、宛先欄のメールアドレスを確認し、必要に応じて本文を編集します。

1. [送信]をクリックします。  
  追加したユーザーに、[{{%service%}}の使用開始までの流れ（ユーザー向け）](/general/ja/user/list_start/start.html)を参照するよう連絡してください。

{{% /enabled %}}

{{% enabled US CN %}}

1. 「{{%slash%}}共通管理」画面の「ユーザー管理」の、[組織/ユーザー]をクリックします。  
    {{< screen src="/general/img-ja/add_user_img01.png" alt="[組織/ユーザー]が赤枠で囲まれた画像">}}

1. 組織のボックスから、ユーザーを追加する組織を選択します。  
  先に[未所属のユーザー]にユーザーを登録し、あとで組織を追加して、ユーザーに設定することもできます。  
  {{< screen src="/general/img-ja/add_user_img02.png" alt="組織とユーザーの設定画面">}}
  組織を追加するには、[組織の追加]をクリックします。詳細は、[組織を追加する](/general/ja/admin/list_useradmin/list_division/add_division.html)を参照してください。  

1. 「ユーザー」欄の[ユーザーの追加]をクリックします。
    {{< screen src="/general/img-ja/add_user_img03.png" alt="[ユーザーの追加]が赤枠で囲まれた画像">}}

1. 必要な項目を設定します。  
  項目の詳細は、[ユーザー情報の設定画面](/general/ja/admin/list_useradmin/list_user/user_details.html)を参照してください。  
  次の項目は、必ず設定してください。
    <table>
      <thead>
          <tr>
              <th width="130" scope="col">項目名</th>
              <th scope="col">内容</th>
          </tr>
      </thead>
      <tbody>
          <tr>
              <td>表示名</td>
              <td>各サービスで表示される名前です。</td>
          </tr>
          <tr>
              <td>ログイン名</td>
              <td>{{%service%}}にログインするためのIDです。<br />
              <ul>
                  <li>他のユーザーと重複するログイン名は使用できません。</li>
                  <li>ログイン名には次の文字を使用できません。<br />
                  \ [ ] &quot; : ; < >, /</li>
                  <li>先頭または最後が半角スペースや全角スペースのログイン名は設定できません。</li>
              </ul>
              </td>
          </tr>
          <tr>
              <td>E-mail</td>
              <td>各サービスでメールの送受信に使用するメールアドレスです。</td>
          </tr>
          <tr>
              <td>使用状態</td>
              <td>「使用中」になっていることを確認します。<br />
              「停止中」の場合は、サービスを利用できません。</td>
          </tr>
          <tr>
              <td>利用サービス</td>
              <td>契約中、または試用を申し込んでいるサービスの一覧です。<br />
              該当ユーザーの利用するサービスのチェックボックスを選択します。<br />
              <a href="/general/ja/admin/list_useradmin/list_user/service_user.html">ユーザーが利用するサービスを設定する</a></td>
          </tr>
      </tbody>
    </table>

1. [保存]をクリックします。  
  {{< screen src="/general/img-ja/add_user_img04.png" alt="画像">}}

1. 「パスワードの設定」ダイアログで、追加したユーザーのパスワードを設定します。
   * パスワードは自動生成か、直接入力で設定します。
   * 「パスワードを表示する」を選択すると、ユーザーのパスワードを確認できます。  
     ただし、Internet Explorer 8ではこのチェックボックスは表示されません。
   * 「このユーザーのパスワードを無期限にする」を選択すると、パスワードポリシーの設定に関わらず、選択したユーザーのパスワードのみ、有効期間を無期限にできます。
    {{< screen src="/general/img-ja/add_user_img05.png" alt="「パスワードの設定」ダイアログの画像">}}

1. ユーザーへパスワードとログインの仕方を通知する方法を選びます。  
    1. **メールで通知する場合**  
      [設定してメールを送信]をクリックし、手順8に進みます。  
      メールで通知する場合、[管理者が設定した仮パスワードの変更を許可する](/general/ja/admin/list_security/list_login/pw_allow.html#list_login_pw_allow_10)ことを推奨します。
      初期設定では有効になっています。  
    1. **メールで通知しない場合**  
      [設定]をクリックし、ユーザー情報を保存します。  
      サービスを利用するユーザーに次の情報を伝えます。  
      * 利用するサービスのアクセスURL  
        例：https://（サブドメイン名）.{{%cybozu_com%}}/
      * ログイン名
      * パスワード  

1. 「パスワードとログイン方法をメールで送信」ダイアログで、宛先欄のメールアドレスを確認し、必要に応じて本文を編集します。

1. [送信]をクリックします。  
  追加したユーザーに、[{{%service%}}の使用開始までの流れ（ユーザー向け）](/general/ja/user/list_start/start.html)を参照するよう連絡してください。

{{% /enabled %}}

{{% enabled JP %}}

{{% note %}}
{{% subtitle %}}「&lt;サービス名&gt;のユーザー数が上限を超えています。」と表示される場合{{% /subtitle %}}
契約ユーザー数が不足しています。[{{%store%}}](https://store.cybozu.com/manage/)で契約内容を変更してから、{{%slash%}}共通管理でユーザーを追加してください。  
詳細は[ユーザー数の追加など、契約内容を変更する](https://www.cybozu.com/jp/buy/add/)方法を参照してください。
{{% /note %}}

{{% /enabled %}}

{{% enabled US %}}
{{% note %}}
{{% subtitle %}}「&lt;サービス名&gt;のユーザー数が上限を超えています。」と表示される場合 {{% /subtitle %}}

契約ユーザー数が不足しています。必要に応じて購入してください。  

* **[AWSへの移行](https://www.kintone.com/aws-migration/)が完了していないお客様**（[ドメインID](/general/ja/admin/list_old/domainid.html)が「c」で始まるお客様）  
  [{{%store%}}](https://store.{{%cybozu_com%}}/)で契約内容を変更してから、{{%slash%}}共通管理でユーザーを追加してください。
* **[AWSへの移行](https://www.kintone.com/aws-migration/)が完了したお客様**（[ドメインID](/general/ja/admin/list_old/domainid.html)が「y」で始まるお客様）  
  {{%slash%}}共通管理で「契約状況」画面を表示し、[購入状況]をクリックして契約内容を変更してから、ユーザーを追加してください。  
{{% /note %}}

{{% /enabled %}}

{{< seealso title="関連する記事" >}}  
[ユーザー情報の設定画面](/general/ja/admin/list_useradmin/list_user/user_details.html) 
{{< /seealso >}}
