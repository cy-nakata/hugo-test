---
title: "ファイルの読み込み時にトリムされる項目"
weight: 800
---
ファイルからデータを読み込む時に、入力情報の先頭や末尾の空白文字が削除される（トリムされる）項目があります。ファイルで読み込むデータと、空白文字のトリムの有無は、次のとおりです。

* &#10004;：空白文字がトリムされる項目を示します。
* 空欄：トリムされない項目を示します。

{{% enabled JP %}}
<table cellspacing="1" cellpadding="1">
    <thead>
        <tr>
            <th width="206" scope="col">読み込むデータ</th>
            <th width="283" scope="col">項目名</th>
            <th width="93" scope="col">トリムの有無</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td width="206" rowspan="26">ユーザー</td>
            <td width="283">ログイン名</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">表示名</td>
            <td width="93"></td>
        </tr>
        <tr>
            <td width="283">新ログイン名</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">パスワード</td>
            <td width="93"></td>
        </tr>
        <tr>
            <td width="283">姓</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">名</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">よみがな（姓）</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">よみがな（名）</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">別言語での表示名</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">別言語の名前を表示する言語</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">E-mail</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">使用状態</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">言語</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">タイムゾーン</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">電話番号</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">内線</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">携帯</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">URL</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">従業員ID</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">入社日</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">誕生日</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">メモ</td>
            <td width="93"></td>
        </tr>
        <tr>
            <td width="283">表示優先度</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">Skype名</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">削除</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">カスタマイズ項目</td>
            <td width="93"></td>
        </tr>
        <tr>
            <td width="206" rowspan="2">ユーザーの利用サービス</td>
            <td width="283">ログイン名</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">サービスコード</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="206" rowspan="7">組織</td>
            <td width="283">組織コード</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">表示名</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">新組織コード</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">別言語での表示名</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">別言語の名前を表示する言語</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">親組織コード</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">説明</td>
            <td width="93"></td>
        </tr>
        <tr>
            <td width="206" rowspan="3">ユーザーの所属組織</td>
            <td width="283">ログイン名</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">組織コード</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">役職コード</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="206" rowspan="5">役職</td>
            <td width="283">役職コード</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">役職名</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">新役職コード</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">説明</td>
            <td width="93"></td>
        </tr>
        <tr>
            <td width="283">削除</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="206" rowspan="6">グループ(ロール)</td>
            <td width="283">グループコード</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">グループ名</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">新グループコード</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">タイプ</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">説明</td>
            <td width="93"></td>
        </tr>
        <tr>
            <td width="283">削除</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="206" rowspan="2">ユーザーの所属グループ(ロール)</td>
            <td width="283">ログイン名</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">グループコード</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="206" rowspan="2">メールサーバーのアカウント</td>
            <td width="283">ログイン名</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">アカウント名（メールアドレスの「@」より前の文字列）</td>
            <td width="93">&#10004;</td>
        </tr>
    </tbody>
</table>
<br />
{{% /enabled %}}

{{% enabled US CN %}}
<table cellspacing="1" cellpadding="1">
    <thead>
        <tr>
            <th width="206" scope="col">読み込むデータ</th>
            <th width="283" scope="col">項目名</th>
            <th width="93" scope="col">トリムの有無</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td width="206" rowspan="26">ユーザー</td>
            <td width="283">ログイン名</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">表示名</td>
            <td width="93"></td>
        </tr>
        <tr>
            <td width="283">新ログイン名</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">パスワード</td>
            <td width="93"></td>
        </tr>
        <tr>
            <td width="283">姓</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">名</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">よみがな（姓）</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">よみがな（名）</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">別言語での表示名</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">別言語の名前を表示する言語</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">E-mail</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">使用状態</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">言語</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">タイムゾーン</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">電話番号</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">内線</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">携帯</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">URL</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">従業員ID</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">入社日</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">誕生日</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">メモ</td>
            <td width="93"></td>
        </tr>
        <tr>
            <td width="283">表示優先度</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">Skype名</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">削除</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">カスタマイズ項目</td>
            <td width="93"></td>
        </tr>
        <tr>
            <td width="206" rowspan="2">ユーザーの利用サービス</td>
            <td width="283">ログイン名</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">サービスコード</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="206" rowspan="7">組織</td>
            <td width="283">組織コード</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">表示名</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">新組織コード</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">別言語での表示名</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">別言語の名前を表示する言語</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">親組織コード</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">説明</td>
            <td width="93"></td>
        </tr>
        <tr>
            <td width="206" rowspan="3">ユーザーの所属組織</td>
            <td width="283">ログイン名</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">組織コード</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">役職コード</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="206" rowspan="5">役職</td>
            <td width="283">役職コード</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">役職名</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">新役職コード</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">説明</td>
            <td width="93"></td>
        </tr>
        <tr>
            <td width="283">削除</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="206" rowspan="6">グループ(ロール)</td>
            <td width="283">グループコード</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">グループ名</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">新グループコード</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">タイプ</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">説明</td>
            <td width="93"></td>
        </tr>
        <tr>
            <td width="283">削除</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="206" rowspan="2">ユーザーの所属グループ(ロール)</td>
            <td width="283">ログイン名</td>
            <td width="93">&#10004;</td>
        </tr>
        <tr>
            <td width="283">グループコード</td>
            <td width="93">&#10004;</td>
        </tr>
    </tbody>
</table>
<br />
{{% /enabled %}}
