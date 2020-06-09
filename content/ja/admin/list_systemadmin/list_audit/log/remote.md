---
title: "クライアント証明書に関するログ"
weight: 800
---
クライアント証明書に関するログは次のとおりです。

{{% enabled JP %}}
<table>
  <tbody>
  <tr>
  <th width="120">ログで伝えていること</th>
  <th width="30">レベル</th>
  <th width="100">モジュール</th>
  <th width="100">アクション</th>
  <th>結果</th>
  <th>補足</th>
  </tr>
  <tr>
  <td>証明書のダウンロード</td>
  <td>重要</td>
  <td>System Administration<br>/User Profile</td>
  <td>download certificate</td>
  <td>SUCCESS</td>
  <td>- 対象ユーザーの名前とID</td>
  </tr>
  <tr>
  <td>証明書の発行・更新</td>
  <td>重要</td>
  <td>System Administration</td>
  <td>create certificate</td>
  <td>SUCCESS</td>
  <td>- 対象ユーザーの名前とIDが記載されたリストと、証明書の有効期間</td>
  </tr>
  <tr>
  <td>証明書の一括ダウンロード</td>
  <td>重要</td>
  <td>System Administration</td>
  <td>bulk download certificate</td>
  <td>SUCCESS</td>
  <td>- 対象ユーザーの名前とID</td>
  </tr>
  <tr>
  <td>スマートフォンアプリを利用するための設定ファイルの送信</td>
  <td>重要</td>
  <td>User Profile</td>
  <td>send mobile setting mail</td>
  <td>SUCCESS</td>
  <td>- 送信先メールアドレス</td>
  </tr>
  <tr>
  <td>Webブラウザーでオフィス外からアクセスするための証明書の送信</td>
  <td>重要</td>
  <td>User Profile</td>
  <td>send browser certificate in mail</td>
  <td>SUCCESS</td>
  <td>- 送信先メールアドレス</td>
  </tr>
  </tbody>
</table>
{{% /enabled %}}

{{% enabled US CN %}}
<table>
  <tbody>
  <tr>
  <th width="120">ログで伝えていること</th>
  <th width="30">レベル</th>
  <th width="100">モジュール</th>
  <th width="100">アクション</th>
  <th>結果</th>
  <th>補足</th>
  </tr>
  <tr>
  <td>証明書のダウンロード</td>
  <td>重要</td>
  <td>System Administration<br>/User Profile</td>
  <td>download certificate</td>
  <td>SUCCESS</td>
  <td>- 対象ユーザーの名前とID</td>
  </tr>
  <tr>
  <td>証明書の発行・更新</td>
  <td>重要</td>
  <td>System Administration</td>
  <td>create certificate</td>
  <td>SUCCESS</td>
  <td>- 対象ユーザーの名前とIDが記載されたリストと、証明書の有効期間</td>
  </tr>
  <tr>
  <td>証明書の一括ダウンロード</td>
  <td>重要</td>
  <td>System Administration</td>
  <td>bulk download certificate</td>
  <td>SUCCESS</td>
  <td>- 対象ユーザーの名前とID</td>
  </tr>
  <tr>
  <td>スマートフォンアプリを利用するための設定ファイルの送信</td>
  <td>重要</td>
  <td>User Profile</td>
  <td>send mobile setting mail</td>
  <td>SUCCESS</td>
  <td>- 送信先メールアドレス</td>
  </tr>
  <tr>
  <td>Webブラウザーでオフィス外からアクセスするための証明書の送信</td>
  <td>重要</td>
  <td>User Profile</td>
  <td>send browser certificate in mail</td>
  <td>SUCCESS</td>
  <td>- 送信先メールアドレス</td>
  </tr>
  </tbody>
</table>
{{% /enabled %}}
