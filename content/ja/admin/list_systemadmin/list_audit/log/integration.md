---
title: "連携サービスの設定に関するログ"
weight: 1200
---

連携サービスの設定に関するログは次のとおりです。

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
  <td>連携サービスの有効化</td>
  <td>重要</td>
  <td>System Administration</td>
  <td>enable integration</td>
  <td>SUCCESS</td>
  <td>- 連携サービス名とid</td>
  </tr>
  <tr>
  <td>連携サービスの無効化</td>
  <td>重要</td>
  <td>System Administration</td>
  <td>disable integration</td>
  <td>SUCCESS</td>
  <td>- 連携サービス名とid</td>
  </tr>
  <tr>
  <td>連携サービスの認可</td>
  <td>情報</td>
  <td>Integrations</td>
  <td>authorize integration</td>
  <td>SUCCESS</td>
  <td>- 連携サービス名とidとscopeの一覧</td>
  </tr>
  <tr>
  <td>連携サービスの利用ユーザーの設定</td>
  <td>重要</td>
  <td>System Administration</td>
  <td>update permitted users</td>
  <td>SUCCESS</td>
  <td>- 連携サービス名とid</td>
  </tr>
  <tr>
  <td>クライアントの登録</td>
  <td>重要</td>
  <td>System Administration</td>
  <td>add oauth client</td>
  <td>SUCCESS</td>
  <td>- クライアント名とclient_id</td>
  </tr>
  <tr>
  <td>クライアントの変更</td>
  <td>重要</td>
  <td>System Administration</td>
  <td>update oauth client</td>
  <td>SUCCESS</td>
  <td>- 変更後のクライアント名とclient_id</td>
  </tr>
  <tr>
  <td>クライアントの削除</td>
  <td>重要</td>
  <td>System Administration</td>
  <td>delete oauth client</td>
  <td>SUCCESS</td>
  <td>- 削除したクライアント名とclient_id</td>
  </tr>
  <tr>
  <td>Slack連携の設定を変更する</td>
  <td>重要</td>
  <td>System Administration</td>
  <td>update slack setting</td>
  <td>SUCCESS</td>
  <td>- Enable or Disable</td>
  </tr>
  </tbody>
</table>
