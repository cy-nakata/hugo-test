---
title: "{{%service%}}全般のログ"
weight: 100
---
{{%service%}}全般のログは次のとおりです。

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
  <td>「ログインのセキュリティ設定」の変更</td>
  <td>重要</td>
  <td>System Administration</td>
  <td>configure security setting</td>
  <td>SUCCESS</td>
  <td>
  - <a href="/general/ja/admin/list_systemadmin/list_audit/log/general.html#log_general_10" target="_blank">「configure security setting」のプロパティ</a>を参照してください。</td>
  </tr>
  <tr>
  <td>管理者によるパスワードの更新</td>
  <td>情報</td>
  <td>User Administration</td>
  <td>update user password</td>
  <td>SUCCESS</td>
  <td>- &lt;表示名&gt;(id: &lt;ユーザーID&gt;)</td>
  </tr>
  <tr>
  <td>パスワードメールの送信</td>
  <td>重要</td>
  <td>User Administration</td>
  <td>send user account mail</td>
  <td>SUCCESS</td>
  <td>- email: &lt;メールアドレス&gt;, &lt;表示名&gt;(id:&lt;ユーザーID&gt;)</td>
  </tr>
  <tr>
  <td>パスワードの変更</td>
  <td>情報</td>
  <td>User Profile</td>
  <td>change password</td>
  <td>SUCCESS</td>
  <td>- ユーザー操作</td>
  </tr>
  <tr>
  <td>パスワード再設定メールの送信</td>
  <td>重要</td>
  <td>Authentication</td>
  <td>send password reset mail</td>
  <td>SUCCESS</td>
  <td>- email:（メールアドレス）、ユーザーのidとユーザー名</td>
  </tr>
  <tr>
  <td>パスワード再設定メールの送信</td>
  <td>重要</td>
  <td>Authentication</td>
  <td>send password reset mail</td>
  <td>FAILED</td>
  <td>- email:（メールアドレス）、reason:unregisteredまたはduplicated</td>
  </tr>
  <tr>
  <td>パスワードリセット</td>
  <td>重要</td>
  <td>Authentication</td>
  <td>reset password</td>
  <td>SUCCESS</td>
  <td>- ユーザーのidとユーザー名</td>
  </tr>
  <tr>
  <td>「Administrator」グループの所属ユーザーの変更</td>
  <td>重要</td>
  <td>User Administration</td>
  <td>assign administrators</td>
  <td>SUCCESS</td>
  <td>- Administratorグループの所属するユーザーID一覧<br>- Administratorグループの所属ユーザ変更画面に遷移</td>
  </tr>
  <tr>
  <td>仮管理者の追加</td>
  <td>重要</td>
  <td>Authentication</td>
  <td>add provisional Administrator</td>
  <td>SUCCESS</td>
  <td>- &lt;表示名&gt;(id: &lt;ユーザーID&gt;)</td>
  </tr>
  <tr>
  <td>システムメールアカウントの変更</td>
  <td>情報</td>
  <td>System Administration</td>
  <td>configure system mail account</td>
  <td>SUCCESS</td>
  <td>- メールアドレス, 組み込み／外部（ホスト名）</td>
  </tr>
  <tr>
  <td>外部サービスとの連携の設定</td>
  <td>重要</td>
  <td>System Administration</td>
  <td>configure external service security settings</td>
  <td>SUCCESS</td>
  <td>- 更新項目</td>
  </tr>
  <tr>
  <td>組織間のアクセス権の有効化・無効化</td>
  <td>重要</td>
  <td>System Administration</td>
  <td>configure organization access control settings</td>
  <td>SUCCESS</td>
  <td>- true/false</td>
  <tr>
  <td>ユーザー管理権限の設定</td>
  <td>重要</td>
  <td>User Administration</td>
  <td>assign user management admin</td>
  <td>SUCCESS</td>
  <td>- &lt;組織名&gt;(id: &lt;組織ID&gt;) <br>- 権限を割り当てられたユーザ名とユーザーIDの一覧</td>
  <tr>
  <td>監査ログのアーカイブダウンロード</td>
  <td>重要</td>
  <td>System Administration</td>
  <td>download audit log archive</td>
  <td>SUCCESS</td>
  <td>- filename</td>
  </tr>
  <tr>
  <td>監査ログの設定の変更</td>
  <td>重要</td>
  <td>System Administration</td>
  <td>configure audit log setting</td>
  <td>SUCCESS</td>
  <td>- 保存期間</td>
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
  <td>「ログインのセキュリティ設定」の変更</td>
  <td>重要</td>
  <td>System Administration</td>
  <td>configure security settings</td>
  <td>SUCCESS</td>
  <td>
  - <a href="/general/ja/admin/list_systemadmin/list_audit/log/general.html#log_general_10" target="_blank">「configure security setting」のプロパティ</a>を参照してください。</td>
  </tr>
  <tr>
  <td>管理者によるパスワードの更新</td>
  <td>情報</td>
  <td>User Administration</td>
  <td>update user password</td>
  <td>SUCCESS</td>
  <td>- &lt;表示名&gt;(id: &lt;ユーザーID&gt;)</td>
  </tr>
  <tr>
  <td>パスワードメールの送信</td>
  <td>重要</td>
  <td>User Administration</td>
  <td>send user account mail</td>
  <td>SUCCESS</td>
  <td>- email: &lt;メールアドレス&gt;, &lt;表示名&gt;(id:&lt;ユーザーID&gt;)</td>
  </tr>
  <tr>
  <td>パスワードの変更</td>
  <td>情報</td>
  <td>User Profile</td>
  <td>change password</td>
  <td>SUCCESS</td>
  <td>- ユーザー操作</td>
  </tr>
  <tr>
  <td>パスワード再設定メールの送信</td>
  <td>重要</td>
  <td>Authentication</td>
  <td>send password reset mail</td>
  <td>SUCCESS</td>
  <td>- email:（メールアドレス）、ユーザーのidとユーザー名</td>
  </tr>
  <tr>
  <td>パスワード再設定メールの送信</td>
  <td>重要</td>
  <td>Authentication</td>
  <td>send password reset mail</td>
  <td>FAILED</td>
  <td>- email:（メールアドレス）、reason:unregisteredまたはduplicated</td>
  </tr>
  <tr>
  <td>パスワードリセット</td>
  <td>重要</td>
  <td>Authentication</td>
  <td>reset password</td>
  <td>SUCCESS</td>
  <td>- ユーザーのidとユーザー名</td>
  </tr>
  <tr>
  <td>「Administrator」グループの所属ユーザーの変更</td>
  <td>重要</td>
  <td>User Administration</td>
  <td>assign administrators</td>
  <td>SUCCESS</td>
  <td>- Administratorグループの所属するユーザーID一覧<br>- Administratorグループの所属ユーザ変更画面に遷移</td>
  </tr>
  <tr>
  <td>仮管理者の追加</td>
  <td>重要</td>
  <td>Authentication</td>
  <td>add provisional Administrator</td>
  <td>SUCCESS</td>
  <td>- &lt;表示名&gt;(id: &lt;ユーザーID&gt;)</td>
  </tr>
  <tr>
  <td>システムメールアカウントの変更</td>
  <td>情報</td>
  <td>System Administration</td>
  <td>configure system mail account</td>
  <td>SUCCESS</td>
  <td>- メールアドレス, 組み込み／外部（ホスト名）</td>
  </tr>
  <tr>
  <td>外部サービスとの連携の設定</td>
  <td>重要</td>
  <td>System Administration</td>
  <td>configure external service security settings</td>
  <td>SUCCESS</td>
  <td>- 更新項目</td>
  </tr>
  <tr>
  <td>組織間のアクセス権の有効化・無効化</td>
  <td>重要</td>
  <td>System Administration</td>
  <td>configure organization access control settings</td>
  <td>SUCCESS</td>
  <td>- true/false</td>
  <tr>
  <td>ユーザー管理権限の設定</td>
  <td>重要</td>
  <td>User Administration</td>
  <td>assign user management admin</td>
  <td>SUCCESS</td>
  <td>- &lt;組織名&gt;(id: &lt;組織ID&gt;) <br>- 権限を割り当てられたユーザ名とユーザーIDの一覧</td>
  <tr>
  <td>監査ログのアーカイブダウンロード</td>
  <td>重要</td>
  <td>System Administration</td>
  <td>download audit log archive</td>
  <td>SUCCESS</td>
  <td>- filename</td>
  </tr>
  <tr>
  <td>監査ログの設定の変更</td>
  <td>重要</td>
  <td>System Administration</td>
  <td>configure audit log setting</td>
  <td>SUCCESS</td>
  <td>- 保存期間</td>
  </tr>
  </tbody>
</table>
{{% /enabled %}}

## 「configure security setting」のプロパティ {#log_general_10}

ログインのセキュリティ設定のログ（アクション：configure security setting）の補足で表示されるプロパティは次のとおりです。  

<table>
  <tbody>
  <tr>
  <th width="100">プロパティ</th>
  <th width="100">意味</th>
  <th width="180">表示される値</th>
  </tr>
  <tr>
  <td>autoComplete</td>
  <td>ログイン名の自動補完の設定</td>
  <td>次のどちらかの値が表示されます。
  <ul>
  <li>true</li>
  <li>false</li>
  </ul>
  </td>
  </tr>
  <tr>
  <td>browserCache</td>
  <td>ログイン名とパスワードのWebブラウザーへの保存を許可する設定</td>
  <td>次のどちらかの値が表示されます。
  <ul>
  <li>true</li>
  <li>false</li>
  </ul>
  </td>
  </tr>
  <tr>
  <td>autologin</td>
  <td>自動ログインをユーザーに許可する設定</td>
  <td>次のどちらかの値が表示されます。
  <ul>
  <li>true <br>
  自動ログインの有効期間（valid time）が一緒に表示されます。</li>
  <li>false</li>
  </ul>
  </td>
  </tr>
  <tr>
  <td>force change password</td>
  <td>管理者が設定した仮パスワードの変更をユーザーに要求する設定</td>
  <td>次のどちらかの値が表示されます。
  <ul>
  <li>true</li>
  <li>false</li>
  </ul>
  </td>
  </tr>
  <tr>
  <td>password policyの<br>「min. length」</td>
  <td>ユーザーパスワードの最低文字数</td>
  <td>数値</td>
  </tr>
  <tr>
  <td>password policyの<br>「min. length[admin]」</td>
  <td>管理者パスワードの最低文字数</td>
  <td>数値</td>
  </tr>
  <tr>
  <td>password policyの<br>「history size」</td>
  <td>パスワード再利用の制限回数</td>
  <td>数値</td>
  </tr>
  <tr>
  <td>password policyの<br>「complexity」</td>
  <td>パスワードの複雑さ</td>
  <td>ALPHA_NUMなどの種別</td>
  </tr>
  <tr>
  <td>password policyの<br>「joe password」</td>
  <td>ログイン名と同じパスワードの使用をユーザーに許可する設定</td>
  <td>次のどちらかの値が表示されます。
  <ul>
  <li>true</li>
  <li>false</li>
  </ul>
  </td>
  </tr>
  <tr>
  <td>password policyの<br>「expire time」</td>
  <td>パスワードの有効期間</td>
  <td>ONE_YEARなどの種別</td>
  </tr>
  <tr>
  <td>password policyの<br>「mutable」</td>
  <td>パスワードの変更をユーザーに許可する設定</td>
  <td>次のどちらかの値が表示されます。
  <ul>
  <li>true</li>
  <li>false</li>
  </ul>
  </td>
  </tr>
  <tr>
  <td>lockout attempts</td>
  <td>アカウントロックアウトまでのログイン失敗回数</td>
  <td>数値</td>
  </tr>
  <tr>
  <td>lockout period</td>
  <td>アアカウントロックアウト解除までの時間</td>
  <td>FOREVERなどの種別</td>
  </tr>
  <tr>
  <td>session lifetime seconds</td>
  <td>セッションの有効期間</td>
  <td>数値</td>
  </tr>
  <tr>
  <td>saml enabled</td>
  <td>SAML認証の設定</td>
  <td>次のどちらかが表示されます。
  <ul>
  <li>SAML認証が有効の場合： saml enabled</li>
  <li>SAML認証が無効の場合： saml disabled</li>
  </ul>
  </td>
  </tr>
  <tr>
  <td>require saml authentication</td>
  <td>SAML認証の使用を必須にする設定</td>
  <td>次のどちらかの値が表示されます。
  <ul>
  <li>true</li>
  <li>false</li>
  </ul>
  </td>
  </tr>
  <tr>
  <td>saml login url</td>
  <td>SAML認証のログインURL</td>
  <td>URL</td>
  </tr>
  <tr>
  <td>saml logout url</td>
  <td>SAML認証のログアウトURL</td>
  <td>URL</td>
  </tr>
  <tr>
  <td>set new saml certificate</td>
  <td>新しい証明書の登録の有無</td>
  <td>次のどちらかの値が表示されます。
  <ul>
  <li>true</li>
  <li>false</li>
  </ul>
  </td>
  </tr>
  <tr>
  <td>allow access even if client certificate user does not match password authenticated user</td>
  <td>クライアント証明書に紐づくユーザーと、パスワード認証に登録されているユーザーが異なっていても、セキュアアクセスを許可する設定</td>
  <td>次のどちらかの値が表示されます。
  <ul>
  <li>true</li>
  <li>false</li>
  </ul>
  </td>
  </tr>
  <tr>
  <td>login failure message</td>
  <td>ログイン失敗時のメッセージの有無と、各言語のエラーメッセージ</td>
  <td>
  <b>ログイン失敗時のメッセージの有無について</b><br>
  次のどちらかの値が表示されます。
  <ul>
  <li>empty=true</li>
  <li>empty=false</li>
  </ul>
  <b>各言語のエラーメッセージについて</b><br>
  設定されていない場合は、メッセージ部分が空で表示されます。
  <ul>
  <li>en=メッセージ</li>
  <li>ja=メッセージ</li>
  <li>zh=メッセージ</li>
  </ul>
  </td>
  </tr>
  </tbody>
</table>
