---
title: "ユーザー情報の設定画面"
weight: 1300
---
{{% enabled US %}}
{{% warning %}}
この記事は、[AWSに移行](https://www.kintone.com/aws-migration/)したお客様向けです。ドメインIDが「y」で始まるお客様が該当します。AWSへの移行が未完了のお客様は、[ユーザー情報の設定画面（AWSへの移行が未完了のお客様向け）](/general/ja/admin/list_old/user_details_old.html)をお読みください。  

ドメインIDを確認するには「[ドメインIDの確認方法](/general/ja/admin/list_old/domainid.html)」を参照してください。
{{% /warning %}}
{{% /enabled %}}

「ユーザー情報の編集」画面で設定できる項目について説明します。  
この画面は次の操作をする場合に表示されます。  

* [ユーザーを追加する](/general/ja/admin/list_useradmin/list_user/add_user.html)
* [ユーザー情報を編集する](/general/ja/admin/list_useradmin/list_user/edit_user.html)

## ユーザー情報の基本項目 {#list_user_user_details_10}

画面で「&ast;」のついている項目は、必須項目です。

{{% enabled JP CN %}}
{{< screen src="/general/img-ja/user_details_img01.png" alt="ユーザー情報の編集画面">}}
{{% /enabled %}}

{{% enabled US %}}
{{< screen src="/general/img-ja/user_details_img01_us.png" alt="ユーザー情報の編集画面">}}
{{% /enabled %}}

{{% enabled JP %}}
<table>
    <caption>ユーザー情報の各項目の説明</caption>
    <thead>
        <tr>
            <th width="130" scope="col">項目名</th>
            <th scope="col">説明</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>画像</td>
            <td>サイズが800KB以内の画像ファイルを選択します。<br />
            使用できる画像のファイル形式は、次のとおりです。<br />
            <ul>
                <li>gif</li>
                <li>jpeg</li>
                <li>png</li>
                <li>bmp</li>
            </ul>
            </td>
        </tr>
        <tr>
            <td width="26">名前</td>
            <td>
            <ul>
            <li>表示名</li>
            各サービスで表示されるユーザーの名前を入力します。
            <li>姓、名</li>
            ユーザーの名前の姓名を漢字で入力します。
            <li>よみがな（姓）、（名）</li>
            ユーザーの名前の姓名のよみがなを入力します。
            </ul>
            </td>
        </tr>
        <tr>
            <td >ログイン名</td>
            <td>
            {{%service%}}にログインするためのIDです。
            <ul> 
                <li>128文字以下で設定してください。</li>
                <li>他のユーザーと重複するログイン名は使用できません。</li>
                <li>ログイン名には次の文字を使用できません。<br />
                \ [ ] &quot; : ; &lt; &gt;, /</li>
                <li>先頭または最後が半角スペースや全角スペースのログイン名は設定できません。</li>
            </ul>
            </td>
        </tr>
        <tr>
            <td >E-mail</td>
            <td>ユーザーが使用するメールアドレスです。<br />
            サービスから送信されるメール通知や、パスワードを忘れた際のパスワードリセットに使用されます。共有のメールアドレスは設定しないでください。</td>
        </tr>
        <tr>
            <td>使用状態</td>
            <td>「使用中」のユーザーは、サービスを利用できます。<br />
            クリックすると、「使用中」と「停止中」が切り替わります。</td>
        </tr>
        <tr>
            <td>利用するサービス</td>
            <td>契約中、または試用を申し込んでいるサービスが表示されます。<br />
            ユーザーに利用を許可するサービスのチェックボックスを選択します。<br />
            <a href="/general/ja/admin/list_useradmin/list_user/service_user.html">ユーザーが利用するサービスを設定する</a></td>
        </tr>
        <tr>
            <td >所属組織</td>
            <td>ユーザーが所属する組織と役職を設定します。組織と役職はあらかじめ設定します。設定方法は次の項目を参照してください。<br />
            <ul>
             <li><a href="/general/ja/admin/list_useradmin/list_division.html">組織の設定</a></li>
             <li><a href="/general/ja/admin/list_useradmin/list_title.html">役職の設定</a></li>
            </ul>
            </td>
        </tr>
        <tr>
            <td >優先する組織</td>
            <td>複数の組織に所属する場合に、ユーザー画面で優先的に表示される組織を選択します。<br />
            この項目はサイボウズ Officeでは使用しません。</td>
        </tr>
        <tr>
            <td >クライアント証明書</td>
            <td>セキュアアクセスのクライアント証明書を発行したユーザーに表示されます。<br />
            「クライアント証明書」のリンクをクリックすると証明書をダウンロードできます。「再発行」ボタンをクリックするとクライアント証明書が再発行されます。発行済みのクライアント証明書は使用できなくなります。</td>
        </tr>
        <tr>
            <td >電話番号</td>
            <td>電話番号を入力します。</td>
        </tr>
        <tr>
            <td>URL</td>
            <td>WebページのURLを入力します。</td>
        </tr>
    </tbody>
</table>
{{% /enabled %}}

{{% enabled CN %}}
<table border="1">
    <caption>ユーザー情報の各項目の説明</caption>
    <thead>
        <tr>
            <th width="130" scope="col">項目名</th>
            <th scope="col">説明</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>画像</td>
            <td>サイズが800KB以内の画像ファイルを選択します。<br />
            使用できる画像のファイル形式は、次のとおりです。<br />
            <ul>
                <li>gif</li>
                <li>jpeg</li>
                <li>png</li>
                <li>bmp</li>
            </ul>
            </td>
        </tr>
        <tr>
            <td width="26">名前</td>
            <td>
            <ul>
            <li>表示名</li>
            各サービスで表示されるユーザーの名前を入力します。
            <li>姓、名</li>
            ユーザーの名前の姓名を漢字で入力します。
            <li>よみがな（姓）、（名）</li>
            ユーザーの名前の姓名のよみがなを入力します。
            </ul>
            </td>
        </tr>
        <tr>
            <td >ログイン名</td>
            <td>
            {{%service%}}にログインするためのIDです。
            <ul> 
                <li>128文字以下で設定してください。</li>
                <li>他のユーザーと重複するログイン名は使用できません。</li>
                <li>ログイン名には次の文字を使用できません。<br />
                \ [ ] &quot; : ; < >, /</li>
                <li>先頭または最後が半角スペースや全角スペースのログイン名は設定できません。</li>
            </ul>
            </td>
        </tr>
        <tr>
            <td>E-mail</td>
            <td>ユーザーが使用するメールアドレスです。<br />
            サービスから送信されるメール通知の送受信などに使用する場合があります。</td>
        </tr>
        <tr>
            <td>使用状態</td>
            <td>「使用中」のユーザーは、サービスを利用できます。<br />
            クリックすると、「使用中」と「停止中」が切り替わります。</td>
        </tr>
        <tr>
            <td>利用するサービス</td>
            <td>契約中、または試用を申し込んでいるサービスが表示されます。<br />
            ユーザーに利用を許可するサービスのチェックボックスを選択します。<br />
            <a href="/general/ja/admin/list_useradmin/list_user/service_user.html">ユーザーが利用するサービスを設定する</a></td>
        </tr>
        <tr>
            <td >所属組織</td>
            <td>ユーザーが所属する組織と役職を設定します。組織と役職はあらかじめ設定します。設定方法は次の項目を参照してください。<br />
            <ul>
             <li><a href="/general/ja/admin/list_useradmin/list_division.html">組織の設定</a></li>
             <li><a href="/general/ja/admin/list_useradmin/list_title.html">役職の設定</a></li>
            </ul>
            </td>
        </tr>
        <tr>
            <td>優先する組織</td>
            <td>複数の組織に所属する場合に、ユーザー画面で優先的に表示される組織を選択します。</td>
        </tr>
        <tr>
            <td>クライアント証明書</td>
            <td>セキュアアクセスのクライアント証明書を発行したユーザーに表示されます。<br />
            「クライアント証明書」のリンクをクリックすると証明書をダウンロードできます。「再発行」ボタンをクリックするとクライアント証明書が再発行されます。発行済みのクライアント証明書は使用できなくなります。</td>
        </tr>
        <tr>
            <td>電話番号</td>
            <td>電話番号を入力します。</td>
        </tr>
        <tr>
            <td>URL</td>
            <td>WebページのURLを入力します。</td>
        </tr>
    </tbody>
</table>
{{% /enabled %}}

{{% enabled US %}}
<table border="1">
    <caption>ユーザー情報の各項目の説明</caption>
    <thead>
        <tr>
            <th width="130" scope="col">項目名</th>
            <th scope="col">説明</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>画像</td>
            <td>サイズが800KB以内の画像ファイルを選択します。<br />
            使用できる画像のファイル形式は、次のとおりです。<br />
            <ul>
                <li>gif</li>
                <li>jpeg</li>
                <li>png</li>
                <li>bmp</li>
            </ul>
            </td>
        </tr>
        <tr>
            <td width="26">名前</td>
            <td>
            <ul>
            <li>表示名</li>
            各サービスで表示されるユーザーの名前を入力します。
            <li>姓、名</li>
            ユーザーの名前の姓名を漢字で入力します。
            <li>よみがな（姓）、（名）</li>
            ユーザーの名前の姓名のよみがなを入力します。
            </ul>
            </td>
        </tr>
        <tr>
            <td >ログイン名</td>
            <td>
            {{%service%}}にログインするためのIDです。
            <ul> 
                <li>128文字以下で設定してください。</li>
                <li>他のユーザーと重複するログイン名は使用できません。</li>
                <li>ログイン名には次の文字を使用できません。<br />
                \ [ ] &quot; : ; < >, /</li>
                <li>先頭または最後が半角スペースや全角スペースのログイン名は設定できません。</li>
            </ul>
            </td>
        </tr>
        <tr>
            <td>E-mail</td>
            <td>ユーザーが使用するメールアドレスです。<br />
            サービスから送信されるメール通知の送受信などに使用する場合があります。</td>
        </tr>
        <tr>
            <td>使用状態</td>
            <td>「使用中」のユーザーは、サービスを利用できます。<br />
            クリックすると、「使用中」と「停止中」が切り替わります。</td>
        </tr>
        <tr>
            <td>利用するサービス</td>
            <td>契約中、または試用を申し込んでいるサービスが表示されます。<br />
            ユーザーに利用を許可するサービスのチェックボックスを選択します。<br />
            <a href="/general/ja/admin/list_useradmin/list_user/service_user.html">ユーザーが利用するサービスを設定する</a></td>
        </tr>
        <tr>
            <td >所属組織</td>
            <td>ユーザーが所属する組織と役職を設定します。組織と役職はあらかじめ設定します。設定方法は次の項目を参照してください。<br />
            <ul>
             <li><a href="/general/ja/admin/list_useradmin/list_division.html">組織の設定</a></li>
             <li><a href="/general/ja/admin/list_useradmin/list_title.html">役職の設定</a></li>
            </ul>
            </td>
        </tr>
        <tr>
            <td>優先する組織</td>
            <td>複数の組織に所属する場合に、ユーザー画面で優先的に表示される組織を選択します。</td>
        </tr>
        <tr>
            <td>2要素認証</td>
            <td>2要素認証の設定の状況が表示されます。有効化したユーザーのみ、[無効にする]ボタンが表示されます。<br />
            モバイル端末の紛失等のために管理者がユーザーの2要素認証を無効化する必要がある場合、[無効にする]をクリックしてください。再度有効にする場合はユーザーがプロフィール画面から設定を行う必要があります。<br /><a href="/general/ja/user/list_personal/two_factor_authentication.html">2要素認証を設定する</a></td>
        </tr>
        <tr>
            <td>電話番号</td>
            <td>電話番号を入力します。</td>
        </tr>
        <tr>
            <td>URL</td>
            <td>WebページのURLを入力します。</td>
        </tr>
    </tbody>
</table>
{{% /enabled %}}

## ユーザー情報のその他の項目 {#list_user_user_details_20}

「その他」で設定できる項目を説明します。

{{% enabled JP %}}
「その他」の項目は、「サイボウズ Office」と「メールワイズ」では使用できません。  
{{% /enabled %}}

{{< screen src="/general/img-ja/user_details_img02.png" alt="ユーザー情報の編集画面の「その他」の画面">}}

<table border="1">
    <caption>ユーザー情報の「その他」項目の説明</caption>
    <thead>
        <tr>
            <th width="130">項目名</th>
            <th>説明</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>連絡先</td>
            <td>内線番号や携帯電話の番号を入力します。</td>
        </tr>
        <tr>
            <td>Skype名</td>
            <td>Skype名を登録しておくとプロフィール画面のリンクから、Skypeを起動できます。</td>
        </tr>
        <tr>
            <td>言語</td>
            <td>各サービスの画面で使用する言語を選択します。</td>
        </tr>
        <tr>
            <td>タイムゾーン</td>
            <td>各サービスで使用するタイムゾーンを選択します。<br />
            詳細は、<a href="/general/ja/admin/list_systemadmin/list_system_time/timezone.html">タイムゾーンの一覧</a>を参照してください。<br />
            </td>
        </tr>
        <tr>
            <td>別言語での表示名</td>
            <td>各サービスでの表示言語を設定しているユーザーの画面で、指定した言語で表示する名前を入力します。</td>
        </tr>
        <tr>
            <td nowrap="">（カスタマイズ項目）</td>
            <td>ユーザー情報にカスタマイズ項目を追加した場合、「別言語での表示名」の次に表示されます。</td>
        </tr>
        <tr>
            <td>従業員ID</td>
            <td>従業員のID番号を入力します。</td>
        </tr>
        <tr>
            <td>入社日</td>
            <td>入社日を入力します。</td>
        </tr>
        <tr>
            <td>誕生日</td>
            <td>誕生日を入力します。</td>
        </tr>
        <tr>
            <td>表示優先度</td>
            <td>ユーザーの表示優先度を0以上の8桁の整数で入力します。<br />
            ユーザー一覧画面で、番号が小さいユーザーが上に表示されます。<br />
            <a href="/general/ja/admin/list_useradmin/list_user/user_sort.html">ユーザーの表示優先度を設定する</a></td>
        </tr>
        <tr>
            <td>メモ</td>
            <td>必要に応じて入力します。</td>
        </tr>
    </tbody>
</table>

{{% note %}}
「その他」の項目は追加できます。  
詳細は、[ユーザー情報の項目を追加する（カスタマイズ項目）](/general/ja/admin/list_useradmin/list_user/custermized_item.html)を参照してください。  
{{% /note %}}
