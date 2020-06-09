---
title: "ログイン時にSAML認証だけを使うように制限する"
weight: 200
---

SAML認証を設定している場合は、{{%service%}}のログイン時にSAML認証だけを使うように制限できます。  
この制限を有効にすると、{{%service%}}標準の認証によるログインはできなくなります。  

この制限の初期値は、無効に設定されています。  
この制限が無効の場合、SAML認証を設定した環境でも、{{%service%}}標準の認証を併用できる状態になります。

{{% note %}}

* {{%service%}}標準の認証とは、{{%service%}}にログインする際に、{{%slash%}}共通管理に登録しているログイン名とパスワードを入力する認証方式を指します。

{{% /note %}}

## 制限を有効にした際に利用できなくなるサービスやモバイルアプリ {#list_saml_saml_restriction_10}

ログイン時にSAML認証だけを使う制限を有効にすると、{{%service%}}標準の認証を使うサービスやモバイルアプリは利用できなくなります。  
下記のサービスやモバイルアプリのうち、1つでも継続して利用する場合は、この制限は無効のままにしてください。  

{{% enabled JP %}}

* {{%CorpName%}}の公式API  
  公式APIの詳細は、[cybozu developer network](https://developer.cybozu.io/hc/ja)を参照してください。  
* [セキュアアクセス](https://www.cybozu.com/jp/service/option/)
* [Cybozu Desktop 2](https://cybozu.co.jp/info/desktop2/)
* モバイルアプリ
  * [KUNAI](https://products.cybozu.co.jp/kunai/)
  * [サイボウズ Office 新着通知](https://products.cybozu.co.jp/office/ver10/product/mobile/notice/)
  * [メールワイズ モバイル](https://mailwise.cybozu.co.jp/functions/mobile/)

{{% /enabled %}}

{{% enabled US %}}

* {{%CorpName%}}の公式API  
  公式APIの詳細は、[{{%kintone%}} Developer Program](https://developer.kintone.io/hc/en-us)を参照してください。  
* [セキュアアクセス](https://www.cybozu.com/jp/service/option/)  

{{% note %}}
セキュアアクセスは、[AWSへの移行](https://www.kintone.com/aws-migration/)が完了していないお客様だけが利用できるサービスです。ドメインIDが「c」で始まるお客様が該当します。ドメインIDを確認するには「[ドメインIDの確認方法](/general/ja/admin/list_old/domainid.html)」を参照してください。
{{% /note %}}

{{% /enabled %}}

{{% enabled CN %}}

* {{%CorpName%}}の公式API  
  公式APIの詳細は、[cybozu developer network](https://cybozudev.kf5.com/hc/)を参照してください。  
* [セキュアアクセス](https://www.cybozu.com/jp/service/option/)
* [Cybozu Desktop 2](https://cybozu.co.jp/info/desktop2/)
* モバイルアプリ  
  * [KUNAI](https://products.cybozu.co.jp/kunai/)

{{% /enabled %}}

{{% note %}}

* {{%kintone%}}モバイルではSAML認証を利用できます。  
  ただし、モバイルアプリのインストール時にSAML認証のログイン情報を入力する必要があります。  
  詳細は、次のページを参照してください。  
  * [iOSのモバイルアプリを利用する](/k/ja/user/mobile_access/ios/mobileapp_ios.html)
  * [Androidのモバイルアプリを利用する](/k/ja/user/mobile_access/android/mobileapp_android.html)
* {{%kintone%}}のゲストユーザーは、SAML認証の対象外です。  
  ログイン時にSAML認証だけを使う制限を有効にしても、{{%kintone%}}のゲストユーザーは、{{%service%}}標準の認証でログインします。  

{{% /note %}}

## {{%slash%}}共通管理者だけが使える機能 {#list_saml_saml_restriction_20}

ログイン時にSAML認証だけを使う制限を有効にしていても、{{%slash%}}共通管理者だけは、下記URLから{{%service%}}標準の認証を利用して、{{%service%}}にログインできます。  
下記URLからログインする際は、{{%slash%}}共通管理に登録しているログイン名とパスワードを入力します。  

|SAML認証を無効にするURL |
|---|
|https://（サブドメイン名）.{{%cybozu_com%}}/login?saml=off  |

{{% note %}}
  
* この機能は、SAML認証に失敗した場合に、{{%service%}}に誰もログインできなくなってしまう状況を回避するためのものです。無効にはできません。  
* {{%slash%}}共通管理者以外のユーザーにも、上記URLの利用を許可する場合は、ログイン時にSAML認証だけを使う制限を無効にする必要があります。

{{% /note %}}  

## ログイン時にSAML認証だけを使う制限を有効にする {#list_saml_saml_restriction_30}

1. SAML認証を設定します。  
  詳細は、[{{%service%}}でSAML認証を設定する](/general/ja/admin/list_externalservices/list_saml/saml_settings.html#list_saml_saml_settings_2020)を参照してください。  
  SAML認証の設定が完了していない場合は、手順2に進めません。  

1. 「{{%slash%}}共通管理共通管理」画面の「セキュリティ」の[ログイン]をクリックします。
  {{< screen src="/general/img-ja/saml_restriction_img01.png"  alt="左ナビの「ログイン」を矩形で囲んでいる画像">}}

1. 「SAML認証を有効にする」が有効であることを確認します。  

1. 「SAML認証の使用を必須にする」を選択します。  
  {{< screen src="/general/img-ja/saml_restriction_img02.png"  alt="「SAML認証の使用を必須にする」を有効にした画像">}}

1. {{%service%}}のログイン時にSAML IdPのログイン情報を入力する旨を、ユーザーに連絡します。  
