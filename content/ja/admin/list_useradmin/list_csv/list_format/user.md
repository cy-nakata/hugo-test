---
title: "ユーザー情報のファイルフォーマット"
weight: 300
---
ユーザー情報の追加や編集を行うためのファイルのフォーマットについて説明します。  
ファイルの読み込み手順は、[ユーザーを一括で登録、編集する](/general/ja/admin/list_useradmin/list_csv/user.html)を参照してください。  

## CSVファイル作成時に気を付けること {#list_format_user_10}

* 情報を変更しない項目には、「\*」（アスタリスク）を指定します。
* 新規ユーザーのパスワードに「\*」は使用できません。
* ユーザーにパスワードとログイン方法をメールで通知する機能は利用できません。

## フォーマットの入力項目 {#list_format_user_20}

1行ごとに、1人のユーザーの情報を記入します。

<table cellspacing="0" cellpadding="0" style="width:100%">
    <caption>CSVファイルの作成例</caption>
    <thead>
        <tr>
            <th width="71" scope="col">ログイン名</th>
            <th width="66" scope="col">表示名</th>
            <th width="57" scope="col">新ログイン名</th>
            <th width="48" scope="col">パスワード</th>
            <th width="50" scope="col">姓</th>
            <th width="50" scope="col">名</th>
            <th width="77" scope="col">よみがな (姓)</th>
            <th width="57" scope="col">よみがな (名)</th>
            <th width="90" scope="col">別言語での表示名</th>
            <th scope="col">別言語の名前を表示する言語</th>
            <th width="16" scope="col">&hellip;</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td width="71">takahashi</td>
            <td width="66">高橋 健太</td>
            <td width="57">&ast;</td>
            <td width="48">xxxxx</td>
            <td width="50">高橋</td>
            <td width="50">健太</td>
            <td width="77">たかはし</td>
            <td width="57">けんた</td>
            <td width="90">Kenta Takahashi</td>
            <td>en</td>
            <td width="16">&hellip;</td>
        </tr>
        <tr>
            <td width="71">kato</td>
            <td width="66">加藤 美咲</td>
            <td width="57">&ast;</td>
            <td width="48">xxxxx</td>
            <td width="50">加藤</td>
            <td width="50">美咲</td>
            <td width="77">かとう</td>
            <td width="57">みさき</td>
            <td width="90">Misaki Kato</td>
            <td>en</td>
            <td width="16">&hellip;</td>
        </tr>
        <tr>
            <td width="71">suzuki</td>
            <td width="66">鈴木 拓也</td>
            <td width="57">&ast;</td>
            <td width="48">xxxxx</td>
            <td width="50">鈴木</td>
            <td width="50">拓也</td>
            <td width="77">すずき</td>
            <td width="57">たくや</td>
            <td width="90">Takuya Suzuki</td>
            <td>en</td>
            <td width="16">&hellip;</td>
        </tr>
    </tbody>
</table>

{{% enabled JP %}}
<table cellspacing="0" cellpadding="0">
    <caption>各入力項目の説明</caption>
    <thead>
        <tr>
            <th width="137" nowrap="" scope="col">項目名</th>
            <th width="74" scope="col">入力必須</th>
            <th scope="col">説明</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td width="137">ログイン名</td>
            <td width="74" style="text-align:center;">&#10004;</td>
            <td>
            <ul>
            <li><b>既存ユーザーを編集する場合：</b><br>
            サービスに登録済のログイン名を指定します。そのログイン名のユーザー情報がCSVファイルにあわせて更新されます。</li>
            <li><b>新規ユーザーを登録する場合：</b><br>
            既存ユーザーのログイン名と重複しない文字列を、新規ユーザーのログイン名として指定します。</li>
            </ul>
            </td>
        </tr>
        <tr>
            <td width="137">表示名</td>
            <td width="74" style="text-align:center;">&#10004;</td>
            <td>&nbsp;</td>
        </tr>
        <tr>
            <td width="137">新ログイン名</td>
            <td width="74" style="text-align:center;">&#10004;</td>
            <td>
            <ul>
            <li><b>既存ユーザーのログイン名を変更する場合：</b><br>
            変更後のログイン名を指定します。</li>
            <li><b>既存ユーザーのログイン名を変更しない場合：</b><br>
            「&ast;」を指定します。</li>
            </ul>
            </td>
        </tr>
        <tr>
            <td width="137">パスワード</td>
            <td width="74" style="text-align:center;">&#10004;</td>
            <td>
            <ul>
            <li><b>既存ユーザーのパスワードの場合：</b><br>
            使用中のパスワードを変更しない場合は「&ast;」を入力します。<br>
            パスワードを変更する場合は、新しいパスワードを入力します。
            </li>
            <li><b>新規ユーザーのパスワードの場合：</b><br>
            <a href="/general/ja/admin/list_useradmin/list_user/edit_userpw.html#list_user_edituserpw_30">パスワードの条件</a>を参照し、新しいパスワードを入力します。ただし、「&ast;」は使用できません。</li>
            新規ユーザーのパスワードに「&ast;」を指定すると、ユーザーがログインできなくなる可能性があります。
            </ul>
            </td>
        </tr>
        <tr>
            <td width="137">姓</td>
            <td width="74">&nbsp;</td>
            <td>&nbsp;</td>
        </tr>
        <tr>
            <td width="137">名</td>
            <td width="74">&nbsp;</td>
            <td>&nbsp;</td>
        </tr>
        <tr>
            <td width="137">よみがな(姓)</td>
            <td width="74">&nbsp;</td>
            <td>&nbsp;</td>
        </tr>
        <tr>
            <td width="137">よみがな(名)</td>
            <td width="74">&nbsp;</td>
            <td>&nbsp;</td>
        </tr>
        <tr>
            <td width="137">別言語での表示名</td>
            <td width="74">&nbsp;</td>
            <td>「別言語での表示名」を指定する場合、「別言語の名前を表示する言語」の指定は必須です。</td>
        </tr>
        <tr>
            <td width="137">別言語の名前を表示する言語</td>
            <td width="74">&nbsp;</td>
            <td>次のいずれかを指定します。<br />
            <ul>
                <li>日本語:ja</li>
                <li>英語:en</li>
                <li>中国語:zh</li>
            </ul>
            </td>
        </tr>
        <tr>
            <td width="137">E-mail</td>
            <td width="74">&nbsp;</td>
            <td>&nbsp;</td>
        </tr>
        <tr>
            <td width="137">使用状態</td>
            <td width="74">&nbsp;</td>
            <td>
            <ul>
            <li>サービスを使用するユーザー：<br>
            「1」を指定します。</li>
            <li>使用停止にするユーザー：<br>
            「0」を指定します。</li>
            </ul>
            </td>
        </tr>
        <tr>
            <td width="137">言語</td>
            <td width="74">&nbsp;</td>
            <td>次のいずれかを指定します。<br />
            <ul>
                <li>日本語:ja</li>
                <li>英語:en</li>
                <li>中国語:zh</li>
                <li>Webブラウザーの設定に従う:auto<br>
                Webブラウザーの言語の設定で、日本語・英語・中国語以外の言語を指定している場合は、{{%service%}}の画面は英語で表示されます。</li>
            </ul>
            空欄の場合は、「Webブラウザーの設定に従う」が設定されます。</td>
        </tr>
        <tr>
            <td width="137">タイムゾーン</td>
            <td width="74">&nbsp;</td>
            <td><a href="/general/ja/admin/list_systemadmin/list_system_time/timezone.html">タイムゾーンの一覧</a>を参照して、タイムゾーンのIDを指定します。<br />
            空欄の場合は、システムタイムゾーンで設定されているタイムゾーンが登録されます。</td>
        </tr>
        <tr>
            <td width="137">電話番号</td>
            <td width="74">&nbsp;</td>
            <td>&nbsp;</td>
        </tr>
        <tr>
            <td width="137">内線</td>
            <td width="74">&nbsp;</td>
            <td>&nbsp;</td>
        </tr>
        <tr>
            <td width="137">携帯</td>
            <td width="74">&nbsp;</td>
            <td>&nbsp;</td>
        </tr>
        <tr>
            <td width="137">URL</td>
            <td width="74">&nbsp;</td>
            <td>&nbsp;</td>
        </tr>
        <tr>
            <td width="137">従業員ID</td>
            <td width="74">&nbsp;</td>
            <td>&nbsp;</td>
        </tr>
        <tr>
            <td width="137">入社日</td>
            <td width="74">&nbsp;</td>
            <td>「YYYY-MM-DD」か「YYYY/MM/DD」の形式の文字列で指定します。</td>
        </tr>
        <tr>
            <td width="137">誕生日</td>
            <td width="74">&nbsp;</td>
            <td>「YYYY-MM-DD」か「YYYY/MM/DD」の形式の文字列で指定します。</td>
        </tr>
        <tr>
            <td width="137">コメント</td>
            <td width="74">&nbsp;</td>
            <td>&nbsp;</td>
        </tr>
        <tr>
            <td width="137">表示優先度</td>
            <td width="74">&nbsp;</td>
            <td>「0」から「99999999」の間の整数を指定します。<br>
            サイボウズ Officeとメールワイズには反映されません。</td>
        </tr>
        <tr>
            <td width="137">Skype名</td>
            <td width="74">&nbsp;</td>
            <td></td>
        </tr>
        <tr>
            <td width="137">削除</td>
            <td width="74">&nbsp;</td>
            <td>
            <ul>
            <li>ユーザーを削除する場合：<br>
            「1」を指定します。</li>
            <li>ユーザーを追加または更新する場合：<br>
            「&ast;」を指定するか、空欄にします。</li>
            </ul>
            </td>
        </tr>
    </tbody>
</table>

{{% /enabled %}}

{{% enabled US CN %}}
<table cellspacing="0" cellpadding="0">
    <caption>各入力項目の説明</caption>
    <thead>
        <tr>
            <th width="137" nowrap="" scope="col">項目名</th>
            <th width="74" scope="col">入力必須</th>
            <th scope="col">説明</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td width="137">ログイン名</td>
            <td width="74" style="text-align:center;">&#10004;</td>
            <td>
            <ul>
            <li><b>既存ユーザーを編集する場合：</b><br>
            サービスに登録済のログイン名を指定します。そのログイン名のユーザー情報がCSVファイルにあわせて更新されます。</li>
            <li><b>新規ユーザーを登録する場合：</b><br>
            既存ユーザーのログイン名と重複しない文字列を、新規ユーザーのログイン名として指定します。</li>
            </ul>
            </td>
        </tr>
        <tr>
            <td width="137">表示名</td>
            <td width="74" style="text-align:center;">&#10004;</td>
            <td>&nbsp;</td>
        </tr>
        <tr>
            <td width="137">新ログイン名</td>
            <td width="74" style="text-align:center;">&#10004;</td>
            <td>
            <ul>
            <li><b>既存ユーザーのログイン名を変更する場合：</b><br>
            変更後のログイン名を指定します。</li>
            <li><b>既存ユーザーのログイン名を変更しない場合：</b><br>
            「&ast;」を指定します。</li>
            </ul>
            </td>
        </tr>
        <tr>
            <td width="137">パスワード</td>
            <td width="74" style="text-align:center;">&#10004;</td>
            <td>
            <ul>
            <li><b>既存ユーザーのパスワードの場合：</b><br>
            使用中のパスワードを変更しない場合は「&ast;」を入力します。<br>
            パスワードを変更する場合は、新しいパスワードを入力します。
            </li>
            <li><b>新規ユーザーのパスワードの場合：</b><br>
            <a href="/general/ja/admin/list_useradmin/list_user/edit_userpw.html#list_user_edituserpw_30">パスワードの条件</a>を参照し、新しいパスワードを入力します。ただし、「&ast;」は使用できません。</li>
            新規ユーザーのパスワードに「&ast;」を指定すると、ユーザーがログインできなくなる可能性があります。
            </ul>
            </td>
        </tr>
        <tr>
            <td width="137">姓</td>
            <td width="74">&nbsp;</td>
            <td>&nbsp;</td>
        </tr>
        <tr>
            <td width="137">名</td>
            <td width="74">&nbsp;</td>
            <td>&nbsp;</td>
        </tr>
        <tr>
            <td width="137">よみがな(姓)</td>
            <td width="74">&nbsp;</td>
            <td>&nbsp;</td>
        </tr>
        <tr>
            <td width="137">よみがな(名)</td>
            <td width="74">&nbsp;</td>
            <td>&nbsp;</td>
        </tr>
        <tr>
            <td width="137">別言語での表示名</td>
            <td width="74">&nbsp;</td>
            <td>「別言語での表示名」を指定する場合、「別言語の名前を表示する言語」の指定は必須です。</td>
        </tr>
        <tr>
            <td width="137">別言語の名前を表示する言語</td>
            <td width="74">&nbsp;</td>
            <td>次のいずれかを指定します。<br />
            <ul>
                <li>日本語:ja</li>
                <li>英語:en</li>
                <li>中国語:zh</li>
            </ul>
            </td>
        </tr>
        <tr>
            <td width="137">E-mail</td>
            <td width="74">&nbsp;</td>
            <td>&nbsp;</td>
        </tr>
        <tr>
            <td width="137">使用状態</td>
            <td width="74">&nbsp;</td>
            <td>
            <ul>
            <li>サービスを使用するユーザー：<br>
            「1」を指定します。</li>
            <li>使用停止にするユーザー：<br>
            「0」を指定します。</li>
            </ul>
            </td>
        </tr>
        <tr>
            <td width="137">言語</td>
            <td width="74">&nbsp;</td>
            <td>次のいずれかを指定します。<br />
            <ul>
                <li>日本語:ja</li>
                <li>英語:en</li>
                <li>中国語:zh</li>
                <li>Webブラウザーの設定に従う:auto<br>
                Webブラウザーの言語の設定で、日本語・英語・中国語以外の言語を指定している場合は、{{%service%}}の画面は英語で表示されます。</li>
            </ul>
            空欄の場合は、「Webブラウザーの設定に従う」が設定されます。</td>
        </tr>
        <tr>
            <td width="137">タイムゾーン</td>
            <td width="74">&nbsp;</td>
            <td>タイムゾーンのIDを指定します。<br />
            <a href="/general/ja/admin/list_systemadmin/list_system_time/timezone.html">タイムゾーンの一覧</a><br />
            空欄の場合は、システムタイムゾーンで設定されているタイムゾーンが登録されます。</td>
        </tr>
        <tr>
            <td width="137">電話番号</td>
            <td width="74">&nbsp;</td>
            <td>&nbsp;</td>
        </tr>
        <tr>
            <td width="137">内線</td>
            <td width="74">&nbsp;</td>
            <td>&nbsp;</td>
        </tr>
        <tr>
            <td width="137">携帯</td>
            <td width="74">&nbsp;</td>
            <td>&nbsp;</td>
        </tr>
        <tr>
            <td width="137">URL</td>
            <td width="74">&nbsp;</td>
            <td>&nbsp;</td>
        </tr>
        <tr>
            <td width="137">従業員ID</td>
            <td width="74">&nbsp;</td>
            <td>&nbsp;</td>
        </tr>
        <tr>
            <td width="137">入社日</td>
            <td width="74">&nbsp;</td>
            <td>「YYYY-MM-DD」か「YYYY/MM/DD」の形式の文字列で指定します。</td>
        </tr>
        <tr>
            <td width="137">誕生日</td>
            <td width="74">&nbsp;</td>
            <td>「YYYY-MM-DD」か「YYYY/MM/DD」の形式の文字列で指定します。</td>
        </tr>
        <tr>
            <td width="137">コメント</td>
            <td width="74">&nbsp;</td>
            <td>&nbsp;</td>
        </tr>
        <tr>
            <td width="137">表示優先度</td>
            <td width="74">&nbsp;</td>
            <td>「0」から「99999999」の間の整数を指定します。</td>
        </tr>
        <tr>
            <td width="137">Skype名</td>
            <td width="74">&nbsp;</td>
            <td></td>
        </tr>
        <tr>
            <td width="137">削除</td>
            <td width="74">&nbsp;</td>
            <td>
            <ul>
            <li>ユーザーを削除する場合：<br>
            「1」を指定します。</li>
            <li>ユーザーを追加または更新する場合：<br>
            「&ast;」を指定するか、空欄にします。</li>
            </ul>
            </td>
        </tr>
    </tbody>
</table>

{{% /enabled %}}

## ユーザー情報にカスタマイズ項目がある場合 {#list_format_user_30}

ユーザー情報に下記図のようなカスタマイズ項目を追加している場合、読み込むCSVファイルにも該当の項目を含める必要があります。  
{{< screen src="/general/img-ja/list_format_user_img01.png"  alt="カスタマイズ項目を追加した画面">}}
追加したカスタマイズ項目がCSVファイルに存在しないと、CSVファイルの読み込み時にエラーが発生します。CSVファイルには、カスタマイズ項目も含めたすべての項目を含めてください。  

{{% note %}}

* カスタマイズ項目の詳細は、[ユーザー情報の項目を追加する（カスタマイズ項目）](/general/ja/admin/list_useradmin/list_user/custermized_item.html)を参照してください。
* カスタマイズ項目の「公開/非公開」や「ユーザーによる変更を許可」の設定値は、ファイルで読み込めません。「{{%slash%}}共通管理」画面で「ユーザー管理」の[組織/ユーザー]をクリックし、[カスタマイズ項目の設定]をクリックして、目的のカスタマイズ項目の設定を変更してください。

{{% /note %}}

### ファイルでのカスタマイズ項目の入力位置 {#list_format_user_3010}

カスタマイズ項目の情報は、ユーザー情報の「削除」項目のあとの列に入力します。  
カスタマイズ項目が複数ある場合は、カスタマイズ項目の表示順にそって記載します。

<table cellspacing="0" cellpadding="0">
    <caption>カスタマイズ項目の表示順の1番目が「拠点情報」、2番目が「座席情報」の場合の例</caption>
    <thead>
        <tr>
            <th width="87" scope="col">ログイン名</th>
            <th width="91" scope="col">表示名</th>
            <th width="113" scope="col">新ログイン名</th>
            <th width="25" scope="col">&hellip;</th>
            <th width="96" scope="col">Skype名</th>
            <th width="40" scope="col">削除</th>
            <th width="91" scope="col">拠点情報</th>
            <th width="87" scope="col">座席情報</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td width="87">takahashi</td>
            <td width="91">高橋 健太</td>
            <td width="113">&ast;</td>
            <td width="25">&hellip;</td>
            <td width="96">k_takahashi</td>
            <td width="40">&ast;</td>
            <td width="91">本社</td>
            <td width="87">20階</td>
        </tr>
    </tbody>
</table>
