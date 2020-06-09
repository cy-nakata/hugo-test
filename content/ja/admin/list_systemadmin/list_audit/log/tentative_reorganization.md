---
title: "組織の事前設定に関するログ"
weight: 1100
disabled: [US]
---

組織の事前設定に関するログは次のとおりです。

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
  <td>組織の追加</td>
  <td>情報</td>
  <td>Sandbox User Administration</td>
  <td>add organization (sandbox)</td>
  <td>SUCCESS</td>
  <td>- 組織のIDと組織名</td>
  </tr>
  <tr>
  <td>組織の変更</td>
  <td>情報</td>
  <td>Sandbox User Administration</td>
  <td>update organization (sandbox)</td>
  <td>SUCCESS</td>
  <td>- 組織のIDと組織名</td>
  </tr>
  <tr>
  <td>組織の削除</td>
  <td>情報</td>
  <td>Sandbox User Administration</td>
  <td>delete organization (sandbox)</td>
  <td>SUCCESS</td>
  <td>- 削除した組織のIDと組織名</td>
  </tr>
  <tr>
  <td>組織の所属ユーザーの変更</td>
  <td>重要</td>
  <td>Sandbox User Administration</td>
  <td>update organization user (sandbox)</td>
  <td>SUCCESS</td>
  <td>- 組織のidと組織名</td>
  </tr>
  <tr>
  <td>役職の追加</td>
  <td>情報</td>
  <td>Sandbox User Administration</td>
  <td>add title (sandbox)</td>
  <td>SUCCESS</td>
  <td>- 役職のIDと役職名</td>
  </tr>
  <tr>
  <td>役職の変更</td>
  <td>情報</td>
  <td>Sandbox User Administration</td>
  <td>update title (sandbox)</td>
  <td>SUCCESS</td>
  <td>- 役職のIDと役職名</td>
  </tr>
  <tr>
  <td>役職の削除</td>
  <td>情報</td>
  <td>Sandbox User Administration</td>
  <td>delete title (sandbox)</td>
  <td>SUCCESS</td>
  <td>- 役職のIDと役職名</td>
  </tr>
  <tr>
  <td>ユーザーの変更</td>
  <td>情報</td>
  <td>Sandbox User Administration</td>
  <td>update user (sandbox)</td>
  <td>SUCCESS</td>
  <td>- ユーザーのidとユーザー名</td>
  </tr>
  <tr>
  <td>サンドボックスの作成</td>
  <td>重要</td>
  <td>Sandbox Administration</td>
  <td>create sandbox</td>
  <td>SUCCESS</td>
  <td>- </td>
  </tr>
  <tr>
  <td>サンドボックスの破棄</td>
  <td>重要</td>
  <td>Sandbox Administration</td>
  <td>discard sandbox</td>
  <td>SUCCESS</td>
  <td>- </td>
  </tr>
  <tr>
  <td>サンドボックスの反映</td>
  <td>重要</td>
  <td>Sandbox Administration</td>
  <td>apply sandbox</td>
  <td>SUCCESS</td>
  <td>次のユーザーが表示される。
  <br>- 即時反映：操作を行ったユーザーのログイン名
  <br>- 時間を指定した反映：Administrator</td>
  </tr>
  <tr>
  <td>サンドボックス反映日時の設定</td>
  <td>重要</td>
  <td>Sandbox Administration</td>
  <td>preset sandbox application date</td>
  <td>SUCCESS</td>
  <td>- 反映予定の日時</td>
  </tr>
  <tr>
  <td>サンドボックス反映日時の取消</td>
  <td>情報</td>
  <td>Sandbox Administration</td>
  <td>cancel sandbox application date</td>
  <td>SUCCESS</td>
  <td>- </td>
  </tr>
  </tbody>
</table>
