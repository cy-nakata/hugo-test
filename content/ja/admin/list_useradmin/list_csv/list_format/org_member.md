---
title: "ユーザーの所属組織のファイルフォーマット"
weight: 600
---
ユーザーの所属組織の追加や編集を行うためのファイルのフォーマットを説明します。ファイルを読み込む手順は次の項目を参照してください。  
[ユーザーの所属組織を一括で登録、編集する](/general/ja/admin/list_useradmin/list_csv/org_member.html)

1行ごとに、1人のユーザーの情報を記入します。1つの「組織コード」に対して、「役職コード」を1つ指定します。

<table cellspacing="1" cellpadding="1">
    <caption>ユーザーの所属組織を読み込むファイルの作成例</caption>
    <thead>
        <tr>
            <th width="124" scope="col">ログイン名</th>
            <th width="124" scope="col">組織コード1</th>
            <th width="124" scope="col">役職コード1</th>
            <th width="124" scope="col">組織コード2</th>
            <th width="124" scope="col">役職コード2</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td width="124">takahashi</td>
            <td width="124">org001</td>
            <td width="124">director</td>
            <td width="124">org002</td>
            <td width="124">manager</td>
        </tr>
        <tr>
            <td width="124">kato</td>
            <td width="124">org001</td>
            <td width="124">&nbsp;</td>
            <td width="124">org002</td>
            <td width="124">&nbsp;</td>
        </tr>
    </tbody>
</table>

<table cellspacing="1" cellpadding="1">
    <caption>各入力項目の説明</caption>
    <thead>
        <tr>
            <th scope="col">項目名</th>
            <th scope="col">入力必須</th>
            <th scope="col">説明</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>ログイン名</td>
            <td style="text-align:center;">&#10004;</td>
            <td>&nbsp;</td>
        </tr>
        <tr>
            <td>組織コード</td>
            <td>&nbsp;</td>
            <td>複数の組織に所属する場合は、1列につき、 組織コードを1つ記入します。</td>
        </tr>
        <tr>
            <td>役職コード</td>
            <td>&nbsp;</td>
            <td>空欄の場合は「役職なし」が設定されます。<br />
            組織コード1における役職は、役職コード1に記載します。</td>
        </tr>
    </tbody>
</table>

{{% note %}}

* 「組織コード1」に指定した組織が、そのユーザーの「優先する組織」になります。
* ファイルにログイン名を記述していないユーザーの所属組織情報は、ファイルを読み込んでも変更されません。
* ユーザーが所属している組織の組織コードを指定しないと、そのユーザーは組織の所属から外れます。
* 組織コードを1つも指定しない場合、そのユーザーのすべての所属組織情報を削除します。

{{% /note %}}
