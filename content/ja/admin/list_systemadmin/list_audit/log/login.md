---
title: "ログインとログアウトに関するログ"
weight: 200
---
ログインとログアウトに関するログは次のとおりです。

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
  <td>ログイン成功</td>
  <td>情報</td>
  <td>Authentication</td>
  <td>login</td>
  <td>SUCCESS</td>
  <td></td>
  </tr>
  <tr>
  <td>ログイン失敗</td>
  <td>情報</td>
  <td>Authentication</td>
  <td>login</td>
  <td>FAILED</td>
  <td>- アカウント名：アカウントがロックアウトされた場合は&quot;lockout&quot;と表示される。</td>
  </tr>
  <tr>
  <td>ログイン失敗（API）</td>
  <td>情報</td>
  <td>Authentication</td>
  <td>login API(%s)</td>
  <td>FAILED</td>
  <td>- アカウント名：アカウントがロックアウトされた場合は&quot;lockout&quot;と表示される。<br>
- &quot;%s&quot;はバージョン名</td>
  </tr>
  <tr>
  <td>ログイン成功（SAML）</td>
  <td>情報</td>
  <td>Authentication</td>
  <td>login (SAML)</td>
  <td>SUCCESS</td>
  <td></td>
  </tr>
  <tr>
  <td>ログイン失敗（SAML）</td>
  <td>情報</td>
  <td>Authentication</td>
  <td>login (SAML)</td>
  <td>FAILED</td>
  <td></td>
  </tr>
  <tr>
  <td>ログイン成功（Session Less）</td>
  <td>情報</td>
  <td>Authentication</td>
  <td>login (session-less)</td>
  <td>SUCCESS</td>
  <td>- サイボウズ Officeへの認証を必要とするアプリケーションなどが共通APIを利用した場合に記録される。</td>
  </tr>
  <tr>
  <td>ログイン失敗（Session Less）</td>
  <td>情報</td>
  <td>Authentication</td>
  <td>login (session-less)</td>
  <td>FAILED</td>
  <td>- サイボウズ Officeへの認証を必要とするアプリケーションなどが共通APIを利用した場合に記録される。</td>
  </tr>
  <tr>
  <td>ログアウト</td>
  <td>情報</td>
  <td>Authentication</td>
  <td>logout</td>
  <td>SUCCESS</td>
  <td></td>
  </tr>
  <tr>
  <td>ログアウト（SAML）</td>
  <td>情報</td>
  <td>Authentication</td>
  <td>logout</td>
  <td>SUCCESS</td>
  <td></td>
  </tr>
  </tbody>
</table>
{{% /enabled %}}

{{% enabled CN US %}}
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
  <td>ログイン成功</td>
  <td>情報</td>
  <td>Authentication</td>
  <td>login</td>
  <td>SUCCESS</td>
  <td></td>
  </tr>
  <tr>
  <td>ログイン失敗</td>
  <td>情報</td>
  <td>Authentication</td>
  <td>login</td>
  <td>FAILED</td>
  <td>- アカウント名：アカウントがロックアウトされた場合は&quot;lockout&quot;と表示される。</td>
  </tr>
  <tr>
  <td>ログイン失敗（API）</td>
  <td>情報</td>
  <td>Authentication</td>
  <td>login API(%s)</td>
  <td>FAILED</td>
  <td>- アカウント名：アカウントがロックアウトされた場合は&quot;lockout&quot;と表示される。<br>
- &quot;%s&quot;はバージョン名</td>
  </tr>
  <tr>
  <td>ログイン成功（SAML）</td>
  <td>情報</td>
  <td>Authentication</td>
  <td>login (SAML)</td>
  <td>SUCCESS</td>
  <td></td>
  </tr>
  <tr>
  <td>ログイン失敗（SAML）</td>
  <td>情報</td>
  <td>Authentication</td>
  <td>login (SAML)</td>
  <td>FAILED</td>
  <td></td>
  </tr>
  <tr>
  <td>ログイン成功（Session Less）</td>
  <td>情報</td>
  <td>Authentication</td>
  <td>login (session-less)</td>
  <td>SUCCESS</td>
  <td>- サービスへの認証を必要とするアプリケーションなどが共通APIを利用した場合に記録される。</td>
  </tr>
  <tr>
  <td>ログイン失敗（Session Less）</td>
  <td>情報</td>
  <td>Authentication</td>
  <td>login (session-less)</td>
  <td>FAILED</td>
  <td>- サービスへの認証を必要とするアプリケーションなどが共通APIを利用した場合に記録される。</td>
  </tr>
  <tr>
  <td>ログアウト</td>
  <td>情報</td>
  <td>Authentication</td>
  <td>logout</td>
  <td>SUCCESS</td>
  <td></td>
  </tr>
  <tr>
  <td>ログアウト（SAML）</td>
  <td>情報</td>
  <td>Authentication</td>
  <td>logout</td>
  <td>SUCCESS</td>
  <td></td>
  </tr>
  </tbody>
</table>
{{% /enabled %}}
