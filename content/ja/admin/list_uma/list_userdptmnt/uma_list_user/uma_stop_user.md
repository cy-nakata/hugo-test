---
title: "[組織の管理者]ユーザーを使用停止にする／使用を再開する"
weight: 400
---
組織の管理者は、次のユーザーの使用状態を変更できます。

* 自分が管理権限を持つ組織に所属しているユーザー
* 組織に未所属のユーザー

## ユーザーを使用停止にする

ユーザーの退職や休職などによりサービスへのアクセスを禁止する場合に、ユーザー情報を削除せず、使用停止にできます。使用停止中のユーザーは、次の状態になります。

* サービスの利用ユーザーにカウントされません。
* サービスにログインできません。
* 使用停止にした段階で、発行済みのクライアント証明書は破棄されます。

{{% warning %}}
{{% subtitle %}}
セキュアアクセス利用ユーザーを使用停止にする場合の注意
{{% /subtitle %}}
ユーザーを使用停止にする前に、ユーザーがセキュアアクセスを使用しているか確認してください。セキュアアクセスに関する設定ができるのは{{%slash%}}共通管理者のみで、組織の管理者はクライアント証明書を発行できません。セキュアアクセスを利用しているユーザーを使用停止にし、その後、使用を再開する場合、クライアント証明書の発行を{{%slash%}}共通管理者に依頼する必要があります。  
{{% enabled US %}}セキュアアクセスは、[AWSに移行](https://www.kintone.com/aws-migration/)したお客様にはご利用いただけません。[ドメインID](/general/ja/admin/list_old/domainid.html)が「y」で始まるお客様が該当します。{{% /enabled %}}
{{% /warning %}}

1. {{%slash%}}共通管理画面で「ユーザー管理」の[組織/ユーザー]をクリックします。  
  {{< screen src="/general/img-ja/usermanagement_uma_stop_user_ja_01.png"  alt="[組織/ユーザー]が赤枠で囲まれた画像">}}
1. 左側の一覧で組織を選択し、使用停止するユーザーの ![アイコン](/general/img/slash_edit_icon.png) をクリックします。
  {{< screen src="/general/img-ja/uma_stop_user_img02.png"  alt="組織とユーザーを選択する画像">}}
1. 使用状態の[使用中]をクリックし、[停止中]に変わったら、[保存]をクリックします。
  {{< screen src="/general/img-ja/uma_stop_user_img03.png"  alt="使用状態を[停止中]にする画像">}}

{{% warning %}}
{{% subtitle %}}
使用停止中のユーザーのプロフィール閲覧
{{% /subtitle %}}
使用停止中のユーザーのプロフィールは、ほかのユーザーが閲覧できます。プロフィールを表示しないようにするには、次のどちらかの操作をします。

* ユーザー情報を編集して、不要な情報を削除する<br>
  [ユーザー情報を編集する](/general/ja/admin/list_useradmin/list_user/edit_user.html)
* ユーザーを完全に削除する<br>
  [ユーザーを削除する](/general/ja/admin/list_uma/list_userdptmnt/uma_list_user/add_user.html#ユーザーを削除する)
{{% /warning %}}

{{% enabled JP %}}
{{% warning %}}
{{% subtitle %}}
ユーザーの使用停止と、契約ユーザー数の関係
{{% /subtitle %}}
ユーザーを使用停止にしただけでは、契約ユーザー数は変わりません。{{%service%}}の課金は、{{%store%}}での契約ユーザー数を基準にします。契約ユーザー数を減らすには、{{%store%}}で契約内容を変更します。
契約内容の変更方法は、次のページを参照してください。<br>
[「購入方法」の「ユーザー数の追加など、契約内容を変更する」](https://www.cybozu.com/jp/buy/add/)
{{% /warning %}}
{{% /enabled %}}

{{% enabled CN %}}
{{% warning %}}
{{% subtitle %}}
ユーザーの使用停止と、契約ユーザー数の関係
{{% /subtitle %}}
ユーザーを使用停止にしただけでは、契約ユーザー数は変わりません。使用停止中のユーザーも、引き続き課金の対象になります。
{{% /warning %}}
{{% /enabled %}}

{{% enabled US %}}
{{% warning %}}
{{% subtitle %}}
ユーザーの使用停止と、契約ユーザー数の関係
{{% /subtitle %}}
ユーザーを使用停止にしただけでは、契約ユーザー数は変わりません。使用停止中のユーザーも、引き続き課金の対象になります。契約ユーザー数を減らすには、次の手続きをしてください。  

* **[AWSへの移行](https://www.kintone.com/aws-migration/)が完了していないお客様**（[ドメインID](/general/ja/admin/list_old/domainid.html)が「c」で始まるお客様）  
  [{{%store%}}](https://store.{{%cybozu_com%}}/)で契約内容を変更してください。  
* **[AWSへの移行](https://www.kintone.com/aws-migration/)が完了したお客様**（[ドメインID](/general/ja/admin/list_old/domainid.html)が「y」で始まるお客様）  
  [サイボウズにお問い合わせ](https://www.kintone.com/support/)ください。  
{{% /warning %}}
{{% /enabled %}}

## ユーザーの使用を再開する

使用停止中のユーザーの使用を再開する手順は次のとおりです。

1. {{%slash%}}共通管理画面で「ユーザー管理」の[組織/ユーザー]をクリックします。
  {{< screen src="/general/img-ja/usermanagement_uma_stop_user_ja_01.png"  alt="[組織/ユーザー]が赤枠で囲まれた画像">}}
1. 左側の一覧で組織を選択し、使用を再開するユーザーの ![アイコン](/general/img/slash_edit_icon.png) をクリックします。
  {{< screen src="/general/img-ja/uma_stop_user_img02.png"  alt="組織とユーザーを選択する画像">}}
1. 使用状態の[停止中]をクリックし、[使用中]に変わったら、[保存]をクリックします。
  {{< screen src="/general/img-ja/uma_stop_user_img04.png"  alt="使用状態を[使用中]にする画像">}}

{{% note %}}
{{% subtitle %}}
セキュアアクセスを使用していたユーザーの使用再開
{{% /subtitle %}}

使用停止にする前にセキュアアクセスを使用していたユーザーは、クライアント証明書が無効になっています。使用再開に伴い、セキュアアクセスの使用も再開する場合、クライアント証明書の再発行を{{%slash%}}共通管理者に依頼してください。  
{{% enabled US %}}セキュアアクセスは、[AWSに移行](https://www.kintone.com/aws-migration/)したお客様にはご利用いただけません。[ドメインID](/general/ja/admin/list_old/domainid.html)が「y」で始まるお客様が該当します。{{% /enabled %}}
{{% /note %}}
