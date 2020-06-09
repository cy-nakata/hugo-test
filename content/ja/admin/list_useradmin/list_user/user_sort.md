---
title: "ユーザーの表示優先度を設定する"
weight: 1100
---
{{% enabled CN %}}
{{%slash%}}共通管理での一覧表示や、Garoon、{{%kintone%}}でのユーザー選択画面などに表示するユーザーの順番を指定できます。
{{% /enabled %}}

{{% enabled JP %}}
{{%slash%}}共通管理での一覧表示や、Garoon、{{%kintone%}}でのユーザー選択画面などに表示するユーザーの順番を指定できます。この機能はサイボウズ Officeとメールワイズには反映されません。
{{% /enabled %}}

{{% enabled US %}}
{{%slash%}}共通管理での一覧表示や、{{%kintone%}}でのユーザー選択画面などに表示するユーザーの順番を指定できます。
{{% /enabled %}}

ここではユーザーの表示優先度をひとりずつ設定する方法を説明します。

{{% note %}}

* CSVファイルを読み込んで表示優先度を一括設定することもできます。  
  [ユーザーを一括で登録、編集する](/general/ja/admin/list_useradmin/list_csv/user.html)方法を参照してください。  
  読み込み用ファイルのフォーマットは、[ユーザー情報のファイルフォーマット](/general/ja/admin/list_useradmin/list_csv/list_format/user.html)を確認してください。

{{% /note %}}

1. 「{{%slash%}}共通管理」画面の「ユーザー管理」の、[組織/ユーザー]をクリックします。  
  {{< screen src="/general/img-ja/user_sort_img01.png"  alt="[組織/ユーザー]が赤枠で囲まれた画像">}}
1. 「組織」欄でユーザーが所属する組織を選択し、表示優先度を変更するユーザーの![アイコン](/general/img/slash_edit_icon.png)をクリックします。  
  新たにユーザーを追加する場合は、[ユーザーの追加]をクリックします。
1. 「表示優先度」の欄に、ユーザーの表示優先度を「0」から「99999999」の間の整数で入力します。  
  表示優先度の数字が小さいユーザーから順に表示されます。
  {{% note %}}
  同じ数字のユーザーが複数存在する、または表示優先度が空の場合は、先に追加したユーザーが上に表示されます。
  {{% /note %}}
  {{< screen src="/general/img-ja/user_sort_img02.png"  alt="表示優先度が赤枠で囲まれた画像">}}
1. [保存]をクリックします。

{{< seealso title="関連する記事" >}}
[ユーザーを追加する](/general/ja/admin/list_useradmin/list_user/add_user.html)
[ユーザー情報を編集する](/general/ja/admin/list_useradmin/list_user/edit_user.html)
{{< /seealso >}}