---
title: "ユーザーの所属グループ（ロール）のファイルフォーマット"
weight: 900
---
ユーザーの所属グループ（ロール）の追加や編集を行うためのファイルのフォーマットを説明します。ファイルを読み込む手順は次の項目を参照してください。  
[ユーザーの所属グループ（ロール）を一括で登録、編集する](/general/ja/admin/list_useradmin/list_csv/group_member.html)

1行ごとに、1人のユーザーの情報を記入します。

<table cellspacing="1" cellpadding="1" border="0">
<caption>ユーザーの所属グループ（ロール）を読み込むファイルの作成例</caption>
    <thead>
        <tr>
            <th scope="col">ログイン名</th>
            <th scope="col">グループコード1</th>
            <th scope="col">グループコード2</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>takahashi</td>
            <td>grp001</td>
            <td>grp021</td>
        </tr>
        <tr>
            <td>kato</td>
            <td>grp001</td>
            <td>&nbsp;</td>
        </tr>
    </tbody>
</table>

<table cellspacing="1" cellpadding="1" border="0">
<caption>各入力項目の説明</caption>
    <thead>
        <tr>
            <th width="107" scope="col">項目名</th>
            <th width="74" scope="col">入力必須</th>
            <th scope="col">説明</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td width="107">ログイン名</td>
            <td width="74">&#10004;</td>
            <td>&nbsp;</td>
        </tr>
        <tr>
            <td width="107">グループコード</td>
            <td width="74">&nbsp;</td>
            <td>静的グループのグループコードのみ指定できます。<br />
            複数のグループに所属する場合は、1列につき、グループコードを1つ記入します。</td>
        </tr>
    </tbody>
</table>

{{% note %}}

* ファイルにログイン名を記述していないユーザーの所属情報は、ファイルを読み込んでも変更されません。
* ユーザーが所属するグループ（ロール）のグループコードを指定しないと、そのユーザーはグループ（ロール）の所属から外れます。
* グループコードを1つも指定しない場合、ユーザーのグループ所属情報が削除されます。

{{% /note %}}
