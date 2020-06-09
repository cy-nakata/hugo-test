---
title: "2要素認証の設定に関するログ"
weight: 850
disabled: [JP,CN]
---

2要素認証の設定に関するログは次のとおりです。  

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
  <td>ユーザーによる2要素認証の有効化</td>
  <td>重要</td>
  <td>Authentication</td>
  <td>enable two-factor authentication</td>
  <td>SUCCESS</td>
  <td></td>
  </tr>
  <tr>
  <td>ユーザーによる2要素認証の無効化</td>
  <td>重要</td>
  <td>Authentication</td>
  <td>disable two-factor authentication</td>
  <td>SUCCESS</td>
  <td></td>
  </tr>
  <tr>
  <td>管理者による2要素認証の設定解除</td>
  <td>情報</td>
  <td>Authentication</td>
  <td>disable two-factor authentication by administrator</td>
  <td>SUCCESS</td>
  <td>- &lt;表示名&gt;(id: &lt;ユーザーID&gt;)</td>
  </tr>
  </tbody>
</table>
