---
title: "組織のファイルフォーマット"
weight: 500
---
組織の追加や編集を行うためのファイルのフォーマットについて説明します。1行ごとに1つの組織の情報を記入します。

{{% warning %}}
**登録済みの組織が読み込むファイルに記載されていない場合、組織が削除されます。**  
既存の組織をファイルに書き出して、読み込み用ファイルを作成することを推奨します。  
ファイルの読み込み手順は次の項目を参照してください。  
[組織を一括で登録、編集する](/general/ja/admin/list_useradmin/list_csv/org.html)
{{% /warning %}}

<table cellspacing="1" cellpadding="1">
    <caption>組織を読み込むファイルの作成例</caption>
    <thead>
        <tr>
            <th width="88" scope="col">組織コード</th>
            <th width="94" scope="col">表示名</th>
            <th width="57" scope="col">新組織<br />
            コード</th>
            <th width="112" scope="col">別言語での<br />
            表示名</th>
            <th width="96" scope="col">別言語の<br />
            名前を表示<br />
            する言語</th>
            <th width="58" scope="col">親組織<br />
            コード</th>
            <th width="158" scope="col">説明</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td width="88">org001</td>
            <td width="94">営業本部</td>
            <td width="57">&ast;</td>
            <td width="112">Sales Department</td>
            <td width="96">en</td>
            <td width="58">&nbsp;</td>
            <td width="158">&nbsp;</td>
        </tr>
        <tr>
            <td width="88">org002</td>
            <td width="94">第一営業部</td>
            <td width="57">&ast;</td>
            <td width="112">Sales Dept#1</td>
            <td width="96">en</td>
            <td width="58">org001</td>
            <td width="158">担当業界：製造</td>
        </tr>
        <tr>
            <td width="88">org003</td>
            <td width="94">第ニ営業部</td>
            <td width="57">&ast;</td>
            <td width="112">Sales Dept#2</td>
            <td width="96">en</td>
            <td width="58">org001</td>
            <td width="158">担当業界：金融</td>
        </tr>
    </tbody>
</table>
<br />
<table cellspacing="1" cellpadding="1">
    <caption>各入力項目の説明</caption>
    <thead>
        <tr>
            <th width="135" scope="col">項目名</th>
            <th width="70" scope="col">入力必須</th>
            <th scope="col">説明</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td width="135">組織コード</td>
            <td width="70" style="text-align:center;">&#10004;</td>
            <td>登録済みの組織コードを指定すると、同じ組織コードの情報が更新されます。<br />
            組織コードを変更しない場合は現在の組織コードを指定し、「新組織コード」に「&ast;」を指定してください。<br>
            新たに組織を追加する場合は、ほかの組織と重複しない任意の文字列を入力してください。</td>
        </tr>
        <tr>
            <td width="135">表示名</td>
            <td width="70" style="text-align:center;">&#10004;</td>
            <td>&nbsp;</td>
        </tr>
        <tr>
            <td width="135">新組織コード</td>
            <td width="70" style="text-align:center;">&#10004;</td>
            <td>「&ast;」を指定すると、「組織コード」と同じ値が入ります。</td>
        </tr>
        <tr>
            <td width="135">別言語での表示名</td>
            <td width="70">&nbsp;</td>
            <td>「別言語での表示名」を指定した場合、「別言語の名前を表示する言語」の指定は必須です。</td>
        </tr>
        <tr>
            <td width="135">別言語の名前を表示する言語</td>
            <td width="70">&nbsp;</td>
            <td>次のいずれかを指定します。
            <ul>
                <li>日本語：ja</li>
                <li>英語：en</li>
                <li>中国語：zh</li>
            </ul>
            </td>
        </tr>
        <tr>
            <td width="135">親組織コード</td>
            <td width="70">&nbsp;</td>
            <td>空欄の場合は、最上位階層の組織として配置されます。<br />
            子組織として配置する場合は、親組織の「組織コード」を記述します。親組織は、子組織よりも上の行に記載します。</td>
        </tr>
        <tr>
            <td width="135">説明</td>
            <td width="70">&nbsp;</td>
            <td>組織に関する説明を記入します。</td>
        </tr>
    </tbody>
</table>

{{% note %}}

* 「表示名」「新組織コード」「別言語での表示名」「別言語の名前を表示する言語」「説明」を変更しない場合は、「&ast;」（アスタリスク）を記述します。

{{% /note %}}
