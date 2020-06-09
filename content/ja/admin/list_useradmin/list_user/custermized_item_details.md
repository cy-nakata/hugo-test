---
title: "カスタマイズ項目の設定画面"
weight: 400
---
{{% enabled JP %}}  
カスタマイズ項目は50個まで追加できます。  
画面で、「&ast;」の付いている項目は、必須項目です。  
カスタマイズ項目は、サイボウズ Office、メールワイズには反映されません。   
各項目に、次の内容を入力します。
{{% /enabled %}} 

{{% enabled US CN %}}  
カスタマイズ項目は50個まで追加できます。  
画面で、「&ast;」の付いている項目は、必須項目です。  
各項目に、次の内容を入力します。
{{% /enabled %}} 

{{% enabled JP CN %}}  
<table>
    <thead>
        <tr>
            <th colspan="2" scope="col">項目名</th>
            <th scope="col">説明</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td colspan="2">項目名</td>
            <td>項目の名前を入力します。ユーザー情報の画面に表示されます。</td>
        </tr>
        <tr>
            <td colspan="2">項目コード</td>
            <td>ほかのカスタマイズ項目と重複しない任意の文字列を入力します。<br />
            英数字とアンダースコア（_）のみ使用できます。<br />
            一部、使用できない文字列があります。後述の補足を参照してください。</td>
        </tr>
        <tr>
            <td nowrap="" rowspan="2">タイプ</td>
            <td nowrap="">文字列（1行）</td>
            <td rowspan="1">カスタマイズ項目の値を1行のテキストで入力できます。</td>
        </tr>
        <tr>
            <td nowrap="">ユーザー選択</td>
            <td rowspan="1">カスタマイズ項目の値に{{%slash%}}共通管理に登録されているユーザーから1人を選択して設定できます。上司や代理人などの指定に使用できます。<br />
            Garoonでは「ユーザー選択」は使用できません。</td>
        </tr>
        <tr>
            <td colspan="2">公開/非公開</td>
            <td>すべてのユーザーにカスタマイズ項目の値を公開する場合は、チェックボックスを選択します。<br />
            非公開にすると、{{%slash%}}共通管理の「ユーザー情報の編集」画面とユーザー本人のプロフィール画面にのみ表示されます。</td>
        </tr>
        <tr>
            <td colspan="2">ユーザーによる変更</td>
            <td>ユーザー本人に項目の値の変更を許可する場合は、チェックボックスを選択します。</td>
        </tr>
    </tbody>
</table>
<br />
{{% /enabled %}} 

{{% enabled US %}}
<table border="1" cellspacing="1" cellpadding="1">
    <thead>
        <tr>
            <th scope="col" colspan="2">項目名</th>
            <th scope="col">説明</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td colspan="2">項目名</td>
            <td>項目の名前を入力します。ユーザー情報の画面に表示されます。</td>
        </tr>
        <tr>
            <td colspan="2">項目コード</td>
            <td>ほかのカスタマイズ項目と重複しない任意の文字列を入力します。<br />
            英数字とアンダースコア（_）のみ使用できます。<br />
            一部、使用できない文字列があります。後述の補足を参照してください。</td>
        </tr>
        <tr>
            <td nowrap="" rowspan="2">タイプ</td>
            <td nowrap="">文字列（1行）</td>
            <td rowspan="1">カスタマイズ項目の値を1行のテキストで入力できます。</td>
        </tr>
        <tr>
            <td nowrap="">ユーザー選択</td>
            <td rowspan="1">カスタマイズ項目の値に{{%slash%}}共通管理に登録されているユーザーから1人を選択して設定できます。上司や代理人などの指定に使用できます。</td>
        </tr>
        <tr>
            <td colspan="2">公開/非公開</td>
            <td>すべてのユーザーにカスタマイズ項目の値を公開する場合は、チェックボックスを選択します。<br />
            非公開にすると、{{%slash%}}共通管理の「ユーザー情報の編集」画面とユーザー本人のプロフィール画面にのみ表示されます。</td>
        </tr>
        <tr>
            <td colspan="2">ユーザーによる変更</td>
            <td>ユーザー本人に項目の値の変更を許可する場合は、チェックボックスを選択します。</td>
        </tr>
    </tbody>
</table>
<br />
{{% /enabled %}}

{{% note %}}
項目コードには、次の文字列は使用できません。

  * display_name
  * display_name_language
  * nickname
  * foreign_key
  * locale
  * base
  * usergroups
  * primary_group
  * attendee
  * sort_key
  * email_address
  * description
  * post
  * telephone_number
  * url
  * image

{{% /note %}}
