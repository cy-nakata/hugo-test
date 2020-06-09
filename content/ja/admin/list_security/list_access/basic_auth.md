---
title: "Basic認証とは"
weight: 300
disabled: [CN]
---

{{% enabled US %}}
{{% warning %}}
Basic認証は、[AWSに移行](https://www.kintone.com/aws-migration/)したお客様（[ドメインID](/general/ja/admin/list_old/domainid.html)が「y」で始まるお客様）にはご利用いただけません。
{{% /warning %}}
{{% /enabled %}}

Basic認証とは、各ユーザーのログイン名やパスワードでの認証とは別に、管理者が指定した認証情報の入力をユーザーに要求する機能です。  
ただし、Basic認証は簡単な認証機能のため、セキュリティのレベルは低いです。  

Basic認証を設定するには、IPアドレス制限も合わせて設定する必要があります。  
{{< screen src="/general/img-ja/list_access_basic_auth_img10.png"  alt="Basic認証のイメージ">}}

## Basic認証を設定すると {#list_access_basic_auth_10}

Basic認証を設定すると、IPアドレス制限で許可されていない場所から{{%service%}}にアクセスする際に、ユーザーは下記のように2段階の認証を求められます。  
IPアドレス制限で許可された場所からアクセスする際は、STEP2の認証だけ求められます。  

* **STEP1：Basic認証のユーザー名とパスワードを入力する**  
  このユーザー名とパスワードは、すべてのユーザーで共通です。  
  入力画面は、OSやWebブラウザーにより異なります。
  {{< screen src="/general/img-ja/list_access_basic_auth_img02.png"  alt="">}}
* **STEP2：{{%service%}}のユーザー名とパスワードを入力する**
  {{< screen src="/general/img-ja/list_access_basic_auth_img01.png"  alt="">}}

## Basic認証を設定できるユーザー {#list_access_basic_auth_20}

* {{%store%}}の管理者
* アクセス制限を設定する権限が付与された、{{%slash%}}共通管理者

管理者の詳細は、[管理者の種類](/general/ja/admin/list_administrator/list_type_of_administrator/administrator.html)を参照してください。

## 設定方法 {#list_access_basic_auth_30}

Basic認証の設定方法は下記のとおりです。

### {{%store%}}の管理者が設定する場合 {#list_access_basic_auth_3010}

1. [{{%store%}}](https://store.{{%cybozu_com%}}/login)にアクセスします。  

1. {{%store%}}の管理者のメールアドレス、パスワードを入力してログインします。
  {{< screen src="/general/img-ja/list_access_basic_auth_img03.png"  alt="ログイン画面">}}
  ログイン情報を忘れてしまった場合は、[{{%store%}}にログインできません。](/general/ja/login/store_account.html)を参照してください。

1. [ドメイン管理]をクリックします。

1. 「セキュリティと認証」タブをクリックします。  
  複数のドメインを所有している場合は、設定するドメインをドロップダウンリストから選択します。
  {{< screen src="/general/img-ja/list_access_basic_auth_img04.png"  alt="ドメイン管理の画面">}}

1. IPアドレス制限を設定します。  
  詳細は、[IPアドレス制限とは](/general/ja/admin/list_security/list_access/ip_restrictions.html)を参照してください。

1. 「Basic認証」欄の[変更]をクリックします。  
  IPアドレス制限が設定されていないと、[変更]は表示されません。
  {{< screen src="/general/img-ja/list_access_basic_auth_img05.png"  alt="ドメイン管理の画面">}}

1. Basic認証のユーザー名とパスワードを入力し、[保存]をクリックします。
  {{< screen src="/general/img-ja/list_access_basic_auth_img06.png"  alt="ドメイン管理の画面">}}
    * ユーザー名：  
      半角英数字、ハイフン（-）およびアンダースコア（_）を使用できます。  
      入力できる文字数は127文字までです。  
      大文字と小文字は区別されます。  
    * パスワード：  
      半角英数字と半角記号を使用できます。  
      入力できる文字数は5文字から64文字までです。  
      大文字と小文字は区別されます。  

設定が完了すると、{{%store%}}の管理者のメールアドレス宛にメールが送信されます。

### {{%slash%}}共通管理者が設定する場合 {#list_access_basic_auth_3020}

アクセス制限の設定が許可されている場合、次の手順でBasic認証を設定できます。  

1. {{%slash%}}共通管理画面にアクセスします。

1. 「セキュリティ」の[アクセス制限]をクリックします。
  {{< screen src="/general/img-ja/list_access_basic_auth_img07.png"  alt="[アクセス制限]が赤枠で囲まれた画像">}}

1. [{{%store%}}へ]をクリックします。  
  {{< screen src="/general/img-ja/list_access_basic_auth_img08.png"  alt="アクセス制限の設定画面">}}

1. これ以降の手順は、[{{%store%}}の管理者が設定する場合](#list_access_basic_auth_3010)と同じです。
