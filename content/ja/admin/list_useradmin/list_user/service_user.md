---
title: "ユーザーが利用するサービスを設定する"
weight: 1000
---
{{% enabled US %}}
{{% warning %}}
この記事は、[AWSへの移行](https://www.kintone.com/aws-migration/)が完了していないお客様向けです。[ドメインID](/general/ja/admin/list_old/domainid.html)が「c」で始まるお客様が該当します。
{{% /warning %}}
{{% /enabled %}}

ユーザーごとに設定する方法と、サービスごとに設定する方法があります。

## ユーザーごとに設定する

1. 「{{%slash%}}共通管理」画面の「ユーザー管理」の、[組織/ユーザー]をクリックします。  
  {{< screen src="/general/img-ja/service_user_img01.png" alt="[組織/ユーザー]が赤枠で囲まれた画像">}}
1. 組織を選択し、利用サービスを設定するユーザーの ![編集アイコン](/general/img/slash_edit_icon.png) をクリックします。  
  目的のユーザーが組織に属していない場合、[未所属のユーザー]を選択します。
  {{< screen src="/general/img-ja/service_user_img02.png" alt="組織とユーザーを選択する画像">}}
1. 「ユーザー情報の編集」画面で、「利用するサービス」のチェックボックスを選択します。
  {{< screen src="/general/img-ja/service_user_img03.png" alt="利用する複数のサービスが選択された画像">}}
1. [保存]をクリックします。
  {{< screen src="/general/img-ja/service_user_img04.png" alt="[保存]が赤枠で囲まれた画像">}}

## サービスごとに設定する

1. 「{{%slash%}}共通管理」画面の「ユーザー管理」の、[サービスの利用ユーザー]をクリックします。
  {{< screen src="/general/img-ja/service_user_img05.png" alt="[サービスの利用ユーザー]が赤枠で囲まれている画面">}}
1. 利用ユーザーを設定するサービスを選択します。
1. 組織を選択し、ユーザーを選択します。ユーザーは複数選択できます。  
  目的のユーザーが組織に属していない場合、[未所属のユーザー]を選択します。
  {{< screen src="/general/img-ja/service_user_img06.png" alt="組織と複数のユーザーが選択された画像">}}
1. [追加&gt;]をクリックして、「（サービス名）を利用するユーザー」にユーザーを追加します。  
  {{< screen src="/general/img-ja/service_user_img07.png" alt="サービスを利用するユーザーを追加する画像">}}
  利用ユーザーから外す場合は、「（サービス名）を利用するユーザー」でユーザーを選択し、[&lt;解除]をクリックします。
  {{< screen src="/general/img-ja/service_user_img08.png" alt="複数のユーザーをサービスの利用ユーザーから外す画像">}}
1. [保存]をクリックします。
  {{< screen src="/general/img-ja/service_user_img09.png" alt="サービスの利用ユーザーの設定画面">}}

{{% warning %}}
{{% subtitle %}}1つのサービスの利用者に、10,000人を超えるユーザーを設定する場合{{% /subtitle %}}
CSVファイルを使用して一括登録してください。画面での操作でサービスの利用者に設定できるユーザーの数は、サービスごとに10,000人までです。  
CSVファイルを読み込んでユーザーの利用サービスを一括登録する手順は、  [ユーザーの利用サービスを一括で登録、編集する](/general/ja/admin/list_useradmin/list_csv/service.html)方法を参照してください。  
{{% /warning %}}

{{% note %}}
試用するサービスを追加すると、すべての{{%slash%}}共通管理者が、追加したサービスの利用ユーザーに設定されます。
{{% /note %}}
