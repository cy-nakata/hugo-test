---
title: "役職のファイルフォーマット"
weight: 700
---
役職の追加や編集を行うためのファイルのフォーマットを説明します。ファイルを読み込む手順は次の項目を参照してください。  
[役職を一括で登録、編集する](/general/ja/admin/list_useradmin/list_csv/title.html)

1行ごとに、1つの役職の情報を記入します。

<table cellspacing="1" cellpadding="1">
    <caption>役職を読み込むファイルの作成例</caption>
    <thead>
        <tr>
            <th width="134" scope="col">役職コード1</th>
            <th width="125" scope="col">役職名</th>
            <th width="133" scope="col">新役職コード</th>
            <th width="87" scope="col">説明</th>
            <th width="93" scope="col">削除</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td width="134">director</td>
            <td width="125">本部長</td>
            <td width="133">&ast;</td>
            <td width="87">&nbsp;</td>
            <td width="93">&ast;</td>
        </tr>
        <tr>
            <td width="134">manager</td>
            <td width="125">マネージャー</td>
            <td width="133">&ast;</td>
            <td width="87">&nbsp;</td>
            <td width="93">&ast;</td>
        </tr>
    </tbody>
</table>

<table cellspacing="1" cellpadding="1">
    <caption>各入力項目の説明</caption>
    <thead>
        <tr>
            <th width="99" scope="col">項目名</th>
            <th width="69" scope="col">入力必須</th>
            <th scope="col">説明</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td width="99">役職コード</td>
            <td width="69">&#10004;</td>
            <td>登録済みの役職コードを指定すると、同じ役職コードの情報が更新されます。<br />
            「&ast;」を指定すると、役職コードが「&ast;」の役職として追加されます。</td>
        </tr>
        <tr>
            <td width="99">役職名</td>
            <td width="69">&#10004;</td>
            <td>&nbsp;</td>
        </tr>
        <tr>
            <td width="99">新役職コード</td>
            <td width="69">&#10004;</td>
            <td>「&ast;」を指定すると、「役職コード」と同じ値が入ります。</td>
        </tr>
        <tr>
            <td width="99">説明</td>
            <td width="69">&nbsp;</td>
            <td>役職に関する説明を記入します。</td>
        </tr>
        <tr>
            <td width="99">削除</td>
            <td width="69">&nbsp;</td>
            <td>削除する役職には「1」を指定します。<br />
            役職の追加や更新を行う場合は「&ast;」を指定するか、空欄にします。</td>
        </tr>
    </tbody>
</table>

{{% note %}}
情報を変更しない項目には、「&ast;」（アスタリスク）を記述します。
{{% /note %}}
