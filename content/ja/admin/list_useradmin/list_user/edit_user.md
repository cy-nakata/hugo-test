---
title: "ユーザー情報を編集する"
weight: 200
---
ユーザー名や所属する組織などのユーザー情報を、管理者が個別に編集する手順を説明します。  
パスワードの変更手順は、[ユーザーのパスワードを変更する](/general/ja/admin/list_useradmin/list_user/edit_userpw.html)を参照してください。  

{{% note %}}
CSVファイルを読み込んでユーザー情報を一括で変更することもできます。  
[ユーザーを一括で登録、編集する](/general/ja/admin/list_useradmin/list_csv/user.html)  
{{% /note %}}

1. 「{{%slash%}}共通管理」画面の「ユーザー管理」の、[組織/ユーザー]をクリックします。
  {{< screen src="/general/img-ja/edit_user_img01.png"  alt="[組織/ユーザー]が赤枠で囲まれた画像">}}

1. 「組織」欄でユーザーが所属する組織を選択し、ユーザー情報を変更するユーザーの![アイコン](/general/img/slash_edit_icon.png)をクリックします。  
  検索ボックスにユーザーの表示名またはログイン名を入力し、ユーザーを検索することもできます。  
  {{< screen src="/general/img-ja/edit_user_img05.png"  alt="組織とユーザーを選択する画像">}}

1. 必要な項目を変更し、[保存]をクリックします。  
  各項目の詳細は、[ユーザー情報の設定画面](/general/ja/admin/list_useradmin/list_user/user_details.html)を参照してください。  
  {{% enabled JP CN %}}
  {{< screen src="/general/img-ja/edit_user_img04.png"  alt="ユーザー情報の編集画面">}}
  {{% /enabled %}}
  {{% enabled US %}}
  {{< screen src="/general/img-ja/edit_user_img04_us.png"  alt="ユーザー情報の編集画面">}}
  {{% /enabled %}}
  {{% enabled JP %}}

  {{% note %}}

  * ログイン名には次の文字を使用できません。  
    \ [ ] &quot; : ; < >, /
  * 先頭または最後が半角スペースや全角スペースのログイン名は設定できません。
  * サイボウズ Officeとメールワイズには、次の項目は反映されません。
    * 別言語での表示名
    * 「その他」のすべての項目
  * 「優先する組織」は、サイボウズ Officeでは使用しません。
  {{% /note %}}
  {{% /enabled %}}
  {{% enabled US CN %}}
  {{% note %}}
  * ログイン名には次の文字を使用できません。  
    \ [ ] &quot; : ; < >, /
  * 先頭または最後が半角スペースや全角スペースのログイン名は設定できません。
  
  {{% /note %}}
  {{% /enabled %}}
