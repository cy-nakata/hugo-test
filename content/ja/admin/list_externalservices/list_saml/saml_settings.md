---
title: "SAML認証を使用したシングルサインオンを設定する"
weight: 100
---
Security Assertion Markup Language（SAML）とは、異なるセキュリティドメイン間で認証情報を連携するための、XMLベースの標準仕様です。  
SAML認証を設定すると、社内のIdentity Provider（IdP）に登録されたユーザーアカウントで、{{%service%}}にシングルサインオン（SSO）できます。  
{{%service%}}はSAML 2.0に対応し、Service Provider（SP）として動作します。

ここではSAML認証を使用したSSOの流れ、および{{%service%}}の設定手順を説明します。

{{% warning %}}

* 本ページでは、構築済みのIdPと{{%service%}}をSAML認証で連携する方法を説明します。
  IdPの構築方法、およびSAML認証で{{%service%}}にログインする端末の設定は、各製品ベンダーにお問い合わせください。
* {{%service%}}をSPとしてSAML認証で連携するには、SAML 2.0に対応したIdPが必要です。

{{% /warning %}}

{{% note %}}

* IdPで設定したSessionNotOnOrAfter属性は、{{%service%}}では無視されます。

{{% /note %}}

## SAML認証を使用したSSOの流れ{#list_saml_saml_settings_10}

SAML認証を有効にすると、{{%service%}}はSP InitiatedなSSOを行います。SAMLリクエストとSAMLレスポンスには、次のバインディングを使用します。

* SAMLリクエスト：HTTP Redirect Binding
* SAMLレスポンス：HTTP POST Binding

{{%service%}}がユーザーを認証する流れは、次のとおりです。

{{% enabled JP %}}
{{< screen src="/general/img-ja/saml_settings_ja_01.png"  alt="SAML認証を使用したSSOの流れを説明する図">}}
{{% /enabled %}}

{{% enabled US %}}
{{< screen src="/general/img-ja/saml_settings_us_ja_01.png"  alt="SAML認証を使用したSSOの流れを説明する図">}}
{{% /enabled %}}

{{% enabled CN %}}
{{< screen src="/general/img-ja/saml_settings_cn_ja_01.png"  alt="SAML認証を使用したSSOの流れを説明する図">}}
{{% /enabled %}}

1. ユーザーが{{%service%}}にアクセスする。
1. {{%service%}}がSAMLリクエストを生成する。
1. ユーザーが、SPからSAMLリクエストを受け取る。
1. IdPがユーザーを認証する。
1. IdPがSAMLレスポンスを生成する。
1. ユーザーが、IdPからSAMLレスポンスを受け取る。
1. {{%service%}}がSAMLレスポンスを受け取り、検証する。
1. SAMLレスポンスの内容に問題がない場合は、ユーザーが{{%service%}}にログインした状態になる。

## Identity Providerと{{%service%}}をSAML認証で連携する{#list_saml_saml_settings_20}

IdPと{{%service%}}をSAML認証で連携するには、IdPと{{%service%}}の両方で設定を行います。

### IdPに{{%service%}}を登録する{#list_saml_saml_settings_2010}

{{%service%}}をSPとして設定するため、IdPに次の情報を登録します。

* {{%service%}}のエンドポイントURL：  
  https://（サブドメイン名）.{{%cybozu_com%}}/saml/acs
* エンティティID：  
  https://（サブドメイン名）.{{%cybozu_com%}}  
  URLの最後に"/"（スラッシュ）をつけないでください。
* ユーザーを識別する要素：NameID
* {{%service%}}をSPとして登録する際に、メタデータファイルを使用することもできます。  
  * メタデータファイルを入手するには：  
    「{{%slash%}}共通管理」の「ログインのセキュリティ設定」画面で「SAML認証を有効にする」を選択し、[Service Providerメタデータのダウンロード」をクリックします。

### {{%service%}}でSAML認証を設定する{#list_saml_saml_settings_2020}

{{%service%}}でSAML認証を有効化し、IdPの情報を設定します。

1. 「{{%slash%}}共通管理」画面の「セキュリティ」の[ログイン]をクリックします。
1. 「SAML認証を有効にする」を選択します。
1. 必要な項目を設定します。
   * Identity ProviderのSSOエンドポイントURL（HTTP-Redirect）  
     SAMLリクエストの送信先を設定します。
   * {{%service%}}からのログアウト後に遷移するURL  
     {{%service%}}からログアウトした後に表示される、IdPのURLを設定します。
   * Identity Providerが署名に使用する公開鍵の証明書  
     RSAかDSAのアルゴリズムで生成された、公開鍵の証明書ファイルを添付します。X.509形式の証明書のみ利用できます。
1. [保存]をクリックします。
1. SAML認証を使用してログインするユーザーのログイン名を確認します。  
  {{%service%}}のユーザーのログイン名に、NameIDに関連付けた値が登録されているかどうかを確認します。
1. SAML認証を使用して{{%service%}}にSSOできるかどうかを確認します。  
   次の操作ができれば、設定は完了です。
    * {{%service%}}にアクセスすると、IdPの認証に成功し、ログイン後の画面が表示される。
    * ログイン後の画面で、右上のユーザー名 > [ログアウト]の順にクリックすると、正常にログアウトできる。  
      {{%kintone%}}の画面を表示している場合は、![画像](/general/img/slash_setting_icon.png)をクリックして、[ログアウト]をクリックします。

{{% note %}}

* {{%service%}}標準の認証を無効にしてSAML認証だけを使う場合は、[ログイン時にSAML認証だけを使うように制限する](/general/ja/admin/list_externalservices/list_saml/saml_restriction.html)を参照してください。

{{% /note %}}

{{< seealso title="関連する記事" >}}
[OASIS > Standards > Security Assertion Markup Language (SAML) v2.0 （英語）](https://www.oasis-open.org/standards#samlv2.0)
{{< /seealso >}}
