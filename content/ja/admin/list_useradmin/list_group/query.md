---
title: "動的グループの抽出条件について"
weight: 500
---
グループ（ロール）に動的グループを設定する場合の、グループの抽出条件について説明します。  
動的グループには、ログイン名や所属する組織などのユーザー情報の条件を、次のような特定の書式で設定します。

```bash
(キー)+半角スペース+(演算子)+半角スペース+(キーの値)
```

<br>

* <b>組織コードが「sales」の組織に所属するユーザーを抽出する場合の例：</b>  
  <table>
    <tbody>
        <tr>
            <td>organization in (&quot;sales&quot;)</td>
        </tr>
    </tbody>
  </table>

<br>
複数のキーの値を入力する場合は、「,（カンマ）」で区切ります。  

* <b>役職コードが「manager」または「chief」の役職に所属するユーザーを抽出する場合の例：</b>  
  <table>
    <tbody>
        <tr>
            <td>title in (&ldquo;manager&rdquo;, &quot;chief&quot;)</td>
        </tr>
    </tbody>
  </table>

<br>
複数の条件を、and や or で組み合わせることもできます。  

* <b>次の条件をすべて満たすユーザーを抽出する場合の例：</b>  
  * 組織コードが「sales」の組織、またはその配下の組織に所属する
  * 役職コードが「manager」の役職に所属する
  <table>
    <tbody>
        <tr>
            <td>organization <= &quot;sales&quot; and title in (&quot;manager&quot;)</td>
        </tr>
    </tbody>
  </table>

<br>
優先度を付けて条件を組み合わせる場合は、優先する組み合わせを「()」（カッコ）で囲みます。

* <b>次の条件をすべて満たすユーザーを抽出する場合の例：</b>  
  * 組織コードが「sales」の組織に所属する、またはログイン名が「sato」である
  * 役職コードが「manager」の役職に所属する
  <table>
    <tbody>
        <tr>
            <td>(organization in (&quot;sales&quot;) or user in (&quot;sato&quot;)) and title in (&quot;manager&quot;)</td>
        </tr>
    </tbody>
  </table>

## 抽出条件の組み合わせ {#list_group_query_10}

抽出条件は、ほかにも次の組み合わせで指定できます。

### キーが「user」の場合 {#list_group_query_1010}

<table>
  <tbody>
  <tr>
  <th>演算子</th>
  <th>キーの値</th>
  <th>抽出されるユーザー</th>
  </tr>
  <tr>
  <td>in</td>
  <td>(ログイン名, ログイン名, ・・・) </td>
  <td>指定したいずれかのログイン名のユーザー</td>
  </tr>
  <tr>
  <td>not in </td>
  <td>(ログイン名, ログイン名, ・・・)</td>
  <td>指定したいずれのログイン名でもないユーザー</td>
  </tr>
  </tbody>
</table>

### キーが「organization」の場合 {#list_group_query_1020}

<table>
  <tbody>
  <tr>
  <th>演算子</th>
  <th>キーの値</th>
  <th>抽出されるユーザー</th>
  </tr>
  <tr>
  <td>in</td>
  <td>(組織コード, 組織コード, ・・・, 組織コード) </td>
  <td>指定したいずれかの組織に所属するユーザー</td>
  </tr>
  <tr>
  <td>not in </td>
  <td>(組織コード, 組織コード, ・・・, 組織コード)</td>
  <td>指定したいずれの組織にも所属しないユーザー</td>
  </tr>
  <tr>
  <td>&lt; </td>
  <td>組織コード</td>
  <td>指定した組織の配下の組織に所属するユーザー</td>
  </tr>
  <tr>
  <td>&lt;= </td>
  <td>組織コード</td>
  <td>指定した組織またはその配下の組織に所属するユーザー</td>
  </tr>
  </tbody>
</table>

### キーが「group」の場合 {#list_group_query_1030}

<table>
  <tbody>
  <tr>
  <th>演算子</th>
  <th>キーの値</th>
  <th>抽出されるユーザー</th>
  </tr>
  <tr>
  <td>in</td>
  <td>(グループコード, グループコード, ・・・, グループコード) </td>
  <td>指定したいずれかのグループに所属するユーザー</td>
  </tr>
  <tr>
  <td>not in </td>
  <td>(グループコード, グループコード, ・・・, グループコード)</td>
  <td>指定したいずれのグループにも所属しないユーザー</td>
  </tr>
  </tbody>
</table>

### キーが「title」の場合 {#list_group_query_1040}

<table>
  <tbody>
  <tr>
  <th>演算子</th>
  <th>キーの値</th>
  <th>抽出されるユーザー</th>
  </tr>
  <tr>
  <td>in</td>
  <td>(役職コード, 役職コード, ・・・, 役職コード) </td>
  <td>指定したいずれかの役職が設定されているユーザー</td>
  </tr>
  <tr>
  <td>not in </td>
  <td>(役職コード, 役職コード, ・・・, 役職コード)</td>
  <td>指定したいずれの役職も設定されていないユーザー</td>
  </tr>
  <tr>
  <td>= </td>
  <td>&quot;no title&quot;</td>
  <td>役職が設定されていないユーザー</td>
  </tr>
  </tbody>
</table>

### キーが「employeeNumber」の場合 {#list_group_query_1050}

<table>
  <tbody>
  <tr>
  <th>演算子</th>
  <th>キーの値</th>
  <th>抽出されるユーザー</th>
  </tr>
  <tr>
  <td>in</td>
  <td>(従業員ID, 従業員ID, ・・・, 従業員ID) </td>
  <td>指定したいずれかの従業員IDのユーザー</td>
  </tr>
  <tr>
  <td>not in </td>
  <td>(従業員ID, 従業員ID, ・・・, 従業員ID)</td>
  <td>指定したいずれの従業員IDでもないユーザー</td>
  </tr>
  </tbody>
</table>

### キーが「birthDate」の場合 {#list_group_query_1060}

<table>
  <tbody>
  <tr>
  <th>演算子</th>
  <th>キーの値</th>
  <th>抽出されるユーザー</th>
  </tr>
  <tr>
  <td>= </td>
  <td>誕生日 </td>
  <td>誕生日が指定した日付のユーザー</td>
  </tr>
  <tr>
  <td>&lt; </td>
  <td>誕生日</td>
  <td>誕生日が指定した日付より前のユーザー</td>
  </tr>
  <tr>
  <td>&lt;= </td>
  <td>誕生日 </td>
  <td>誕生日が指定した日付以前のユーザー</td>
  </tr>
  <tr>
  <td>&gt; </td>
  <td>誕生日</td>
  <td>誕生日が指定した日付より後のユーザー</td>
  </tr>
  <tr>
  <td>&gt;= </td>
  <td>誕生日</td>
  <td>誕生日が指定した日付以降のユーザー</td>
  </tr>
  </tbody>
</table>

### キーが「joinDate」の場合 {#list_group_query_1070}

<table>
  <tbody>
  <tr>
  <th>演算子</th>
  <th>キーの値</th>
  <th>抽出されるユーザー</th>
  </tr>
  <tr>
  <td>= </td>
  <td>入社日 </td>
  <td>入社日が指定した日付のユーザー</td>
  </tr>
  <tr>
  <td>&lt; </td>
  <td>入社日</td>
  <td>入社日が指定した日付より前のユーザー</td>
  </tr>
  <tr>
  <td>&lt;= </td>
  <td>入社日 </td>
  <td>入社日が指定した日付以前のユーザー</td>
  </tr>
  <tr>
  <td>&gt; </td>
  <td>入社日</td>
  <td>入社日が指定した日付より後のユーザー</td>
  </tr>
  <tr>
  <td>&gt;= </td>
  <td>入社日</td>
  <td>入社日が指定した日付以降のユーザー</td>
  </tr>
  </tbody>
</table>
