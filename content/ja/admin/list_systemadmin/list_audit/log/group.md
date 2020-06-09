---
title: "グループに関するログ"
weight: 500
---
グループに関するログは次のとおりです。

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
  <td>グループの追加</td>
  <td>情報</td>
  <td>User Administration</td>
  <td>add group</td>
  <td>SUCCESS</td>
  <td>- グループ名とid</td>
  </tr>
  <tr>
  <td>グループの変更</td>
  <td>情報</td>
  <td>User Administration</td>
  <td>update group</td>
  <td>SUCCESS</td>
  <td>- グループ名とid</td>
  </tr>
  <tr>
  <td>グループの削除</td>
  <td>情報</td>
  <td>User Administration</td>
  <td>delete group</td>
  <td>SUCCESS</td>
  <td>- グループ名とid</td>
  </tr>
  <tr>
  <td>グループの書き出し</td>
  <td>情報</td>
  <td>User Administration</td>
  <td>export group</td>
  <td>SUCCESS</td>
  <td></td>
  </tr>
  <tr>
  <td>グループの書き出し（API）</td>
  <td>情報</td>
  <td>User Administration</td>
  <td>export group（API %s）</td>
  <td>SUCCESS</td>
  <td>- &quot;%s&quot;はバージョン名</td>
  </tr>
  <tr>
  <td>グループの読み込み</td>
  <td>情報</td>
  <td>User Administration</td>
  <td>import group</td>
  <td>SUCCESS</td>
  <td></td>
  </tr>
  <tr>
  <td>グループの読み込み（API）</td>
  <td>情報</td>
  <td>User Administration</td>
  <td>import group（API %s）</td>
  <td>SUCCESS</td>
  <td>- &quot;%s&quot;はバージョン名</td>
  </tr>
  <tr>
  <td>動的グループの所属ユーザー条件の変更</td>
  <td>重要</td>
  <td>User Administration</td>
  <td>update group condition</td>
  <td>SUCCESS</td>
  <td>- 条件式</td>
  </tr>
  <tr>
  <td>グループの所属ユーザーの変更</td>
  <td>情報</td>
  <td>User Administration</td>
  <td>update user group</td>
  <td>SUCCESS</td>
  <td>- グループのid、グループ名</td>
  </tr>
  <tr>
  <td>グループの所属ユーザーの書き出し</td>
  <td>重要</td>
  <td>User Administration</td>
  <td>export user group</td>
  <td>SUCCESS</td>
  <td>  </td>
  </tr>
  <tr>
  <td>グループの所属ユーザーの書き出し（API）</td>
  <td>重要</td>
  <td>User Administration</td>
  <td>export user group（API %s）</td>
  <td>SUCCESS</td>
  <td>- &quot;%s&quot;はバージョン名</td>
  </tr>
  <tr>
  <td>グループの所属ユーザーの読み込み</td>
  <td>情報</td>
  <td>User Administration</td>
  <td>import user group</td>
  <td>SUCCESS</td>
  <td></td>
  </tr>
  <tr>
  <td>グループの所属ユーザーの読み込み（API）</td>
  <td>情報</td>
  <td>User Administration</td>
  <td>import user group（API %s）</td>
  <td>SUCCESS</td>
  <td>- &quot;%s&quot;はバージョン名</td>
  </tr>
  <tr>
  <td>グループの取得（API）</td>
  <td>重要</td>
  <td>User Information</td>
  <td>get group（API %s）</td>
  <td>SUCCESS</td>
  <td>- グループのidとグループ名のリスト<br>- &quot;%s&quot;はバージョン名</td>
  </tr>
  <tr>
  <td>グループの所属ユーザの取得（API）</td>
  <td>重要</td>
  <td>User Information</td>
  <td>get group users（API %s）</td>
  <td>SUCCESS</td>
  <td>- 指定グループのidとグループ名<br>- &quot;%s&quot;はバージョン名</td>
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
  <td>グループの追加</td>
  <td>情報</td>
  <td>User Administration</td>
  <td>add group</td>
  <td>SUCCESS</td>
  <td>- グループ名とid</td>
  </tr>
  <tr>
  <td>グループの変更</td>
  <td>情報</td>
  <td>User Administration</td>
  <td>update group</td>
  <td>SUCCESS</td>
  <td>- グループ名とid</td>
  </tr>
  <tr>
  <td>グループの削除</td>
  <td>情報</td>
  <td>User Administration</td>
  <td>delete group</td>
  <td>SUCCESS</td>
  <td>- グループ名とid</td>
  </tr>
  <tr>
  <td>グループの書き出し</td>
  <td>情報</td>
  <td>User Administration</td>
  <td>export group</td>
  <td>SUCCESS</td>
  <td></td>
  </tr>
  <tr>
  <td>グループの書き出し（API）</td>
  <td>情報</td>
  <td>User Administration</td>
  <td>export group（API %s）</td>
  <td>SUCCESS</td>
  <td>- &quot;%s&quot;はバージョン名</td>
  </tr>
  <tr>
  <td>グループの読み込み</td>
  <td>情報</td>
  <td>User Administration</td>
  <td>import group</td>
  <td>SUCCESS</td>
  <td></td>
  </tr>
  <tr>
  <td>グループの読み込み（API）</td>
  <td>情報</td>
  <td>User Administration</td>
  <td>import group（API %s）</td>
  <td>SUCCESS</td>
  <td>- &quot;%s&quot;はバージョン名</td>
  </tr>
  <tr>
  <td>動的グループの所属ユーザー条件の変更</td>
  <td>重要</td>
  <td>User Administration</td>
  <td>update group condition</td>
  <td>SUCCESS</td>
  <td>- 条件式</td>
  </tr>
  <tr>
  <td>グループの所属ユーザーの変更</td>
  <td>情報</td>
  <td>User Administration</td>
  <td>update user group</td>
  <td>SUCCESS</td>
  <td>- グループのid、グループ名</td>
  </tr>
  <tr>
  <td>グループの所属ユーザーの書き出し</td>
  <td>重要</td>
  <td>User Administration</td>
  <td>export user group</td>
  <td>SUCCESS</td>
  <td>  </td>
  </tr>
  <tr>
  <td>グループの所属ユーザーの書き出し（API）</td>
  <td>重要</td>
  <td>User Administration</td>
  <td>export user group（API %s）</td>
  <td>SUCCESS</td>
  <td>- &quot;%s&quot;はバージョン名</td>
  </tr>
  <tr>
  <td>グループの所属ユーザーの読み込み</td>
  <td>情報</td>
  <td>User Administration</td>
  <td>import user group</td>
  <td>SUCCESS</td>
  <td></td>
  </tr>
  <tr>
  <td>グループの所属ユーザーの読み込み（API）</td>
  <td>情報</td>
  <td>User Administration</td>
  <td>import user group（API %s）</td>
  <td>SUCCESS</td>
  <td>- &quot;%s&quot;はバージョン名</td>
  </tr>
  <tr>
  <td>グループの取得（API）</td>
  <td>重要</td>
  <td>User Information</td>
  <td>get group（API %s）</td>
  <td>SUCCESS</td>
  <td>- グループのidとグループ名のリスト<br>- &quot;%s&quot;はバージョン名</td>
  </tr>
  <tr>
  <td>グループの所属ユーザの取得（API）</td>
  <td>重要</td>
  <td>User Information</td>
  <td>get group users（API %s）</td>
  <td>SUCCESS</td>
  <td>- 指定グループのidとグループ名<br>- &quot;%s&quot;はバージョン名</td>
  </tr>
  </tbody>
</table>
{{% /enabled %}}
