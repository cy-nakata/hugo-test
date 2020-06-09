---
title: "ユーザー管理に関するログ"
weight: 300
---
ユーザー管理に関するログは次のとおりです。

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
  <td>ユーザーの追加</td>
  <td>情報</td>
  <td>User Administration</td>
  <td>add user</td>
  <td>SUCCESS</td>
  <td>- ユーザーのidとユーザー名</td>
  </tr>
  <tr>
  <td>ユーザーの変更</td>
  <td>情報</td>
  <td>User Administration</td>
  <td>update user</td>
  <td>SUCCESS</td>
  <td>- ユーザーのidとユーザー名</td>
  </tr>
  <tr>
  <td>ユーザーの削除</td>
  <td>情報</td>
  <td>User Administration</td>
  <td>delete user</td>
  <td>SUCCESS</td>
  <td>- ユーザーのidとユーザー名</td>
  </tr>
  <tr>
  <td>ユーザーの書き出し</td>
  <td>重要</td>
  <td>User Administration</td>
  <td>export user</td>
  <td>SUCCESS</td>
  <td></td>
  </tr>
  <tr>
  <td>ユーザーの書き出し（API）</td>
  <td>重要</td>
  <td>User Administration</td>
  <td>export user（API %s）</td>
  <td>SUCCESS</td>
  <td>- &quot;%s&quot;はバージョン名</td>
  </tr>
  <tr>
  <td>ユーザーの読み込み</td>
  <td>情報</td>
  <td>User Administration</td>
  <td>import user</td>
  <td>SUCCESS</td>
  <td></td>
  </tr>
  <tr>
  <td>ユーザーの読み込み（API）</td>
  <td>情報</td>
  <td>User Administration</td>
  <td>import user（API %s）</td>
  <td>SUCCESS</td>
  <td>- &quot;%s&quot;はバージョン名</td>
  </tr>
  <tr>
  <td>ユーザーの取得（API）</td>
  <td>重要</td>
  <td>User Information</td>
  <td>get user（API %s）</td>
  <td>SUCCESS</td>
  <td>- ユーザーのidとユーザー名のリスト<br>- &quot;%s&quot;はバージョン名</td>
  </tr>
  <tr>
  <td>ユーザの所属組織の取得（API）</td>
  <td>重要</td>
  <td>User Information</td>
  <td>get user organizations（API %s）</td>
  <td>SUCCESS</td>
  <td>- ユーザのidとユーザー名<br>- &quot;%s&quot;はバージョン名</td>
  </tr>
  <tr>
  <td>ユーザの所属グループの取得（API）</td>
  <td>重要</td>
  <td>User Information</td>
  <td>get user groups（API %s）</td>
  <td>SUCCESS</td>
  <td>- ユーザのidとユーザー名<br>- &quot;%s&quot;はバージョン名</td>
  </tr>
  <tr>
  <td>複数ユーザーの追加（API）</td>
  <td>重要</td>
  <td>User Administration</td>
  <td>add users（API %s）</td>
  <td>SUCCESS</td>
  <td>- ユーザのidとユーザー名<br>- &quot;%s&quot;はバージョン名</td>
  </tr>
  <tr>
  <td>複数ユーザーの更新（API）<br> / 複数ユーザーのコード更新（API）</td>
  <td>重要</td>
  <td>User Administration</td>
  <td>update users（API %s）</td>
  <td>SUCCESS</td>
  <td>- ユーザのidとユーザー名<br>- &quot;%s&quot;はバージョン名</td>
  </tr>
  <tr>
  <td>複数ユーザーの削除（API）</td>
  <td>重要</td>
  <td>User Administration</td>
  <td>delete users（API %s）</td>
  <td>SUCCESS</td>
  <td>- ユーザのidとユーザー名<br>- &quot;%s&quot;はバージョン名</td>
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
  <td>ユーザーの追加</td>
  <td>情報</td>
  <td>User Administration</td>
  <td>add user</td>
  <td>SUCCESS</td>
  <td>- ユーザーのidとユーザー名</td>
  </tr>
  <tr>
  <td>ユーザーの変更</td>
  <td>情報</td>
  <td>User Administration</td>
  <td>update user</td>
  <td>SUCCESS</td>
  <td>- ユーザーのidとユーザー名</td>
  </tr>
  <tr>
  <td>ユーザーの削除</td>
  <td>情報</td>
  <td>User Administration</td>
  <td>delete user</td>
  <td>SUCCESS</td>
  <td>- ユーザーのidとユーザー名</td>
  </tr>
  <tr>
  <td>ユーザーの書き出し</td>
  <td>重要</td>
  <td>User Administration</td>
  <td>export user</td>
  <td>SUCCESS</td>
  <td></td>
  </tr>
  <tr>
  <td>ユーザーの書き出し（API）</td>
  <td>重要</td>
  <td>User Administration</td>
  <td>export user（API %s）</td>
  <td>SUCCESS</td>
  <td>- &quot;%s&quot;はバージョン名</td>
  </tr>
  <tr>
  <td>ユーザーの読み込み</td>
  <td>情報</td>
  <td>User Administration</td>
  <td>import user</td>
  <td>SUCCESS</td>
  <td></td>
  </tr>
  <tr>
  <td>ユーザーの読み込み（API）</td>
  <td>情報</td>
  <td>User Administration</td>
  <td>import user（API %s）</td>
  <td>SUCCESS</td>
  <td>- &quot;%s&quot;はバージョン名</td>
  </tr>
  <tr>
  <td>ユーザーの取得（API）</td>
  <td>重要</td>
  <td>User Information</td>
  <td>get user（API %s）</td>
  <td>SUCCESS</td>
  <td>- ユーザーのidとユーザー名のリスト<br>- &quot;%s&quot;はバージョン名</td>
  </tr>
  <tr>
  <td>ユーザの所属組織の取得（API）</td>
  <td>重要</td>
  <td>User Information</td>
  <td>get user organizations（API %s）</td>
  <td>SUCCESS</td>
  <td>- ユーザのidとユーザー名<br>- &quot;%s&quot;はバージョン名</td>
  </tr>
  <tr>
  <td>ユーザの所属グループの取得（API）</td>
  <td>重要</td>
  <td>User Information</td>
  <td>get user groups（API %s）</td>
  <td>SUCCESS</td>
  <td>- ユーザのidとユーザー名<br>- &quot;%s&quot;はバージョン名</td>
  </tr>
  </tbody>
</table>
{{% /enabled %}}
