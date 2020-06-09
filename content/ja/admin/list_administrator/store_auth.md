---
title: "契約情報やアクセス制限の設定変更の権限を{{%slash%}}共通管理者に付与する"
weight: 500
disabled: [CN]
---
{{% enabled US %}}
{{% warning %}}
この記事は、[AWSへの移行](https://www.kintone.com/aws-migration/)が完了していないお客様向けです。ドメインIDが「c」で始まるお客様が該当します。ドメインIDを確認するには「[ドメインIDの確認方法](/general/ja/admin/list_old/domainid.html)」を参照してください。
{{% /warning %}}
{{% /enabled %}}

{{% disabled US CN %}}
{{%slash%}}共通管理者に契約情報やアクセス制限の設定変更権限を付与すると、{{%slash%}}共通管理者は次の操作ができるようになります。

* 「契約状況」画面からの、サービスの見積、購入、解約、試用の申し込み
* 「契約状況」画面の[詳細な契約状況]からの、ドメイン名、会社情報、および月額サービスの支払方法の変更
* 「アクセス制限の設定」画面からの、IPアドレス制限とBasic認証の設定

{{% /disabled %}}

{{% disabled JP CN %}}
{{%slash%}}共通管理者に契約情報やアクセス制限の設定変更権限を付与すると、{{%slash%}}共通管理者は次の操作ができるようになります。

* 「契約状況」画面からの、サービスの見積、購入、解約、試用の申し込み
* 「契約状況」画面の[詳細な契約状況]からの、ドメイン名や会社情報の変更
* 「アクセス制限の設定」画面からの、IPアドレス制限とBasic認証の設定

{{% /disabled %}}

{{% disabled US CN %}}
<br>
<b>権限が付与されている場合の「契約状況」画面：</b>
{{< screen src="/general/img-ja/store_auth_jp_ja01.png"  alt="権限が付与されている場合の「契約状況」画面">}}

<b>権限が付与されていない場合の「契約状況」画面：</b>
{{< screen src="/general/img-ja/store_auth_jp_ja02.png"  alt="権限が付与されていない場合の「契約状況」画面">}}

2014年11月8日までに作成された環境の場合、初期状態では{{%slash%}}共通管理者は契約情報やアクセス制限の設定を変更できません。{{%slash%}}共通管理者に契約情報やアクセス制限の設定変更権限を付与するには、{{%store%}}で設定を変更します。

1. {{%store%}}の管理者で、{{%store%}}にログインします。  
  [{{%store%}}](https://store.cybozu.com/login?)
1. [アカウント管理]をクリックし、「管理権限の付与」の右側の[変更]をクリックします。
1. チェックボックスを選択し、[保存]をクリックします。  
  権限を外す場合は、チェックボックスの選択を外し、[保存]をクリックします。

{{% note %}}
{{%store%}}管理者のメールアドレスやパスワードがわからない場合は、[{{%store%}}にログインできません。](/general/ja/login/store_account.html)を参照してください。  
{{% /note %}}
{{% /disabled %}}

{{% disabled JP CN %}}

1. {{%store%}}の管理者で、{{%store%}}にログインします。  
  [{{%store%}}](https://store.kintone.com/login?)
1. [Accounts]をクリックし、「Permissions for Domain Administrators」の右側の[Change]をクリックします。
1. チェックボックスを選択し、[Save]をクリックします。  
  権限を外す場合は、チェックボックスの選択を外し、[Save]をクリックします。

{{% /disabled %}}
