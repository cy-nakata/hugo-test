---
title: "ユーザーの利用サービスのファイルフォーマット"
weight: 400
---
ユーザーの利用サービスの追加や編集を行うためのファイルのフォーマットを説明します。ファイルを読み込む手順は次の項目を参照してください。  
[ユーザーの利用サービスを一括で登録、編集する](/general/ja/admin/list_useradmin/list_csv/service.html)

## ユーザーの利用サービスを読み込むファイルの作成例 {#list_format_service_10}

{{% enabled JP CN %}}
1行ごとに、1人のユーザーの情報を記入します。複数のサービスを利用する場合は、1列につき、サービスコードを1つ記入します。

<table>
  <tbody>
  <tr>
  <th>ログイン名</th>
  <th>サービスコード1</th>
  <th>サービスコード2</th>
  <th>サービスコード3</th>
  </tr>
  <tr>
  <td>takahashi</td>
  <td>ki</td>
  <td>gr </td>
  <td>sa</td>
  </tr>
  <tr>
  <td>kato</td>
  <td>ki</td>
  <td>sa</td>
  <td>&nbsp;</td>
  </tr>
  <tr>
  <td>suzuki</td>
  <td>gr</td>
  <td>&nbsp;</td>
  <td>&nbsp;</td>
  </tr>
  </tbody>
</table>

{{% /enabled %}}

{{% enabled US %}}
1行ごとに、1人のユーザーの情報を記入します。1列につき、サービスコードを1つ記入します。

<table>
  <tbody>
  <tr>
  <th>ログイン名</th>
  <th>サービスコード1</th>
  <th>サービスコード2</th>
  </tr>
  <tr>
  <td>takahashi</td>
  <td>ki</td>
  <td>&nbsp; </td>
  </tr>
  <tr>
  <td>kato</td>
  <td>ki</td>
  <td>sa</td>
  </tr>
  </tbody>
</table>

{{% /enabled %}}

## 各入力項目の説明 {#list_format_service_20}

次の点に注意してください。  

* ファイルにログイン名を記述していないユーザーの利用サービス情報は、ファイルを読み込んでも変更されません。
* サービスコードを1つも指定しない場合、そのユーザーのすべての利用サービス情報が削除されます。

{{% enabled JP %}}

<table>
  <tbody>
  <tr>
  <th>項目名</th>
  <th>入力必須</th>
  <th>説明</th>
  </tr>
  <tr>
  <td>ログイン名</td>
  <td>&nbsp; &#10004;</td>
  <td>&nbsp;</td>
  </tr>
  <tr>
  <td>サービスコード</td>
  <td>&nbsp;</td>
  <td>ユーザーが利用するサービスに応じて、次の2文字で指定します。<br>- {{%kintone%}}: ki<br>- Garoon: gr<br>- サイボウズ Office: of<br>- メールワイズ: mw<br>- セキュアアクセス: sa</td>
  </tr>
  </tbody>
</table>

{{% /enabled %}}

{{% enabled US %}}

<table>
  <tbody>
  <tr>
  <th>項目名</th>
  <th>入力必須</th>
  <th>説明</th>
  </tr>
  <tr>
  <td>ログイン名</td>
  <td>&nbsp; &#10004;</td>
  <td>&nbsp;</td>
  </tr>
  <tr>
  <td>サービスコード</td>
  <td>&nbsp;</td>
  <td>ユーザーが利用するサービスに応じて、次の2文字で指定します。<br>- {{%kintone%}}: ki<br>- セキュアアクセス: sa</td>
  </tr>
  </tbody>
</table>

{{% /enabled %}}

{{% enabled CN %}}

<table>
  <tbody>
  <tr>
  <th>項目名</th>
  <th>入力必須</th>
  <th>説明</th>
  </tr>
  <tr>
  <td>ログイン名</td>
  <td>&nbsp; &#10004;</td>
  <td>&nbsp;</td>
  </tr>
  <tr>
  <td>サービスコード</td>
  <td>&nbsp;</td>
  <td>ユーザーが利用するサービスに応じて、次の2文字で指定します。<br>- {{%kintone%}}: ki<br>- Garoon: gr<br>- セキュアアクセス: sa</td>
  </tr>
  </tbody>
</table>

{{% /enabled %}}
