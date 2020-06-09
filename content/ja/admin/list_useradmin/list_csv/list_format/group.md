---
title: "グループ（ロール）のファイルフォーマット"
weight: 800
---
グループ（ロール）の追加や編集を行うためのファイルのフォーマットを説明します。ファイルを読み込む手順は次の項目を参照してください。  
[グループ（ロール）を一括で登録、編集する](/general/ja/admin/list_useradmin/list_csv/group.html)

1行につき、1つのグループ（ロール）の情報を記入します。

<table cellspacing="1" cellpadding="1">
    <caption>グループ（ロール）を読み込むファイルの作成例</caption>
    <thead>
        <tr>
            <th width="116" scope="col">グループコード</th>
            <th width="98" scope="col">グループ名</th>
            <th width="139" scope="col">新グループコード</th>
            <th width="70" scope="col">タイプ</th>
            <th width="149" scope="col">説明</th>
            <th width="94" scope="col">削除フラグ</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td width="116">grp001</td>
            <td width="98">本社</td>
            <td width="139">&ast;</td>
            <td width="70">static</td>
            <td width="149">本社勤務社員グループ</td>
            <td width="94">&ast;</td>
        </tr>
        <tr>
            <td width="116">grp002</td>
            <td width="98">派遣社員</td>
            <td width="139">&ast;</td>
            <td width="70">dynamic</td>
            <td width="149">派遣社員グループ</td>
            <td width="94">&ast;</td>
        </tr>
    </tbody>
</table>

<table cellspacing="1" cellpadding="1">
    <caption>各入力項目の説明</caption>
    <thead>
        <tr>
            <th width="126" scope="col">項目名</th>
            <th width="65" scope="col">入力必須</th>
            <th scope="col">説明</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td width="126">グループコード</td>
            <td width="65">&#10004;</td>
            <td>登録済みのグループコードを指定すると、グループコードが同じグループの情報が更新されます。<br />
            「&ast;」を指定すると、グループコードが「&ast;」のグループとして追加されます。</td>
        </tr>
        <tr>
            <td width="126">グループ名</td>
            <td width="65">&#10004;</td>
            <td>グループ名は、ほかのグループと重複できません。</td>
        </tr>
        <tr>
            <td width="126">新グループコード</td>
            <td width="65">&#10004;</td>
            <td>「&ast;」を指定すると、「グループコード」と同じ値が入ります。</td>
        </tr>
        <tr>
            <td width="126">タイプ</td>
            <td width="65">&#10004;</td>
            <td>「static」（静的グループ）か「dynamic」（動的グループ）を指定します。</td>
        </tr>
        <tr>
            <td width="126">説明</td>
            <td width="65">&nbsp;</td>
            <td>グループ（ロール）に関する説明を記入します。</td>
        </tr>
        <tr>
            <td width="126">削除</td>
            <td width="65">&nbsp;</td>
            <td>削除する場合は「1」を指定します。<br />
            グループ（ロール）の追加や更新を行う場合は「&ast;」を指定するか、空欄にします。</td>
        </tr>
    </tbody>
</table>

{{% note %}}
情報を変更しない項目には、「&ast;」（アスタリスク）を記述します。
{{% /note %}}
