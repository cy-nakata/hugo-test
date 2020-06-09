---
title: "ログインできない：次に確認すること"
weight: 500
---

[ログインできない：最初に確認すること](/general/ja/login/troubleshoot_first.html)を実施しても解決できない場合は、下記に該当する現象がないか確認してください。  

## 「不正なリクエストです。」と表示されます。 {#login_troubleshoot_second_10}

{{% enabled JP CN %}}
{{%service%}}のメンテナンス中です。  
しばらく経ってから、再度ログインしてください。  
メンテナンスの進捗は、[メンテナンス情報](https://cs.cybozu.co.jp/maintenance/)で確認できます。  
{{% /enabled %}}

{{% enabled US %}}
{{%service%}}のメンテナンス中です。  
しばらく経ってから、再度ログインを試してください。  
メンテナンスの進捗は、[Satus Page](https://kintone.statuspage.io/)で確認できます。  
{{% /enabled %}}

## Code:404　NotFoundが表示されます。 {#login_troubleshoot_second_20}

ログインURLが間違っているようです。  
URLを確認し、再度ログインを試してください。  
正しいURLは、[ログインURLがわかりません。](/general/ja/login/forgot_url.html)を参照してください。  

## 社外からログインできません。 {#login_troubleshoot_second_40}

{{% enabled JP CN %}}
IPアドレス制限やセキュアアクセスが設定されています。  
社外からのアクセスが必要な場合は、管理者による設定が必要です。  
管理者が設定を完了するまでは、社外から{{%service%}}にアクセスできません。  
管理者が行う作業の詳細は、[よりセキュリティを高める設定](/general/ja/admin/list_security/list_access.html)を参照してください。  
{{% /enabled %}}

{{% enabled US %}}
IPアドレス制限が設定されています。  
社外からアクセスが必要な場合は、次の両方の作業が必要です。  

* 管理者がIPアドレス制限を無効にする
* ユーザーが2要素認証を設定する  
  詳細は、[2要素認証を設定する](/general/ja/user/list_personal/two_factor_authentication.html)を参照してください。  

{{% /enabled %}}

## ログイン画面の上部に、別の認証画面が表示されます。 {#login_troubleshoot_second_30}

{{% enabled JP US %}}
下記のような画面が表示されていますか？
{{< screen src="/general/img-ja/troubleshoot_second_img02.png"  alt="Basic認証の画面例">}}
Basic認証が設定されています。  
Basic認証のログイン情報は、管理者のみ{{%store%}}で確認できます。  
管理者にログイン情報を問い合わせてください。  
{{% /enabled %}}

{{% enabled US %}}
{{% warning %}}
Basic認証は、[AWSに移行](https://www.kintone.com/aws-migration/)したお客様にはご利用いただけません。[ドメインID](/general/ja/admin/list_old/domainid.html)が「y」で始まるお客様が該当します。
{{% /warning %}}
{{% /enabled %}}

{{% enabled CN %}}
下記のような画面が表示されていますか？
{{< screen src="/general/img-ja/troubleshoot_second_img02.png"  alt="Basic認証の画面例">}}
Basic認証が設定されています。  
Basic認証のログイン情報は、{{%CorpName%}}に[お問い合わせ](https://www.cybozu.cn/free.html)ください。  
{{% /enabled %}}

## 昨日までログインできていたのに、急にログインできなくなりました。 {#login_troubleshoot_second_50}

下記のいずれかに該当していないか確認してください。  

* <b>パスワードの有効期限が切れていませんか？</b>  
  {{%service%}}の初期設定では、パスワードの有効期間は1年間に設定されています。  
  有効期間を過ぎたパスワードではログインできません。  
  <br>
  * <b>パスワードの再設定画面が表示される場合：</b>  
    ユーザー自身で新しいパスワードを設定し、ログインしてください。  
  * <b>パスワードの有効期間の確認方法：</b>  
    管理者のみ確認できます。  
    {{%slash%}}共通管理の「ログインのセキュリティ設定」画面で確認できます。  
    {{< screen src="/general/img-ja/troubleshoot_second_img03.png"  alt="クライアント証明書の有効期限を示す画像">}}  

* <b>SAML認証、または、別のサービスとのシングルサインオンが設定されていませんか？</b>  
  ログインに必要な情報は、管理者に確認してください。  
<br>

* <b>管理者によって、ログイン名やパスワードが変更されていませんか？</b>  
  ユーザーに新しいログイン情報を連絡してください。  

{{% disabled US %}}

* <b>クライアント証明書が再発行されていませんか？</b>  
  新しいクライアント証明書が発行されると、古いクライアント証明書は利用できなくなります。  
  新しいクライアント証明書を発行した場合は、ユーザーに連絡してください。  
  クライアント証明書を差し替える手順は、[クライアント証明書の登録方法](/ja/settings/browser/certificate.html)を参照してください。  
<br>

{{% /disabled %}}

{{% disabled US %}}

## 「アクセスにはクライアント証明書が必要です。」と表示されます。 {#login_troubleshoot_second_60}

次のようなメッセージですか？
{{< screen src="/general/img-ja/troubleshoot_second_img06_jp.png"  alt="ログイン画面に表示されるメッセージ">}}  

URLに「.s」が含まれていないか確認してください。  

* **「.s」が含まれているURL：**  
  https://（サブドメイン名）**.s**.{{%cybozu_com%}}/  
* **「.s」を除いたURL：**  
  https://（サブドメイン名）.{{%cybozu_com%}}/

セキュアアクセスを利用しない場合は、「.s」を除いたURLからログインします。  
セキュアアクセスを利用する場合は、使用するWebブラウザーやモバイル端末にクライアント証明書がインストールされているかどうかを確認してください。  
詳細は、[「Code: 496 No Cert」と表示される場合](/general/ja/admin/list_security/list_secureaccess/login_flow.html#list_secureaccess_login_flow_10)を参照してください。

## 「アクセスするには認証が必要です。」と表示されます。 {#login_troubleshoot_second_110}

次のようなメッセージですか？
{{< screen src="/general/img-ja/troubleshoot_second_img07_jp.png"  alt="ログイン画面に表示されるメッセージ">}}  

* **セキュアアクセスを利用している場合：**  
  Webブラウザーにクライアント証明書を登録する必要があります。  
  「.s」を含むURL「https://（サブドメイン名）.s.{{%cybozu_com%}}/」にアクセスします。  
* **セキュアアクセスを利用していない：**  
  クライアント証明書は不要です。  
  「.s」を除いたURL「https://（サブドメイン名）.{{%cybozu_com%}}/」にアクセスします。

## クライアント証明書の有効期限に関するメッセージが表示されます。 {#login_troubleshoot_second_70}

次のようなメッセージですか？
{{< screen src="/general/img-ja/troubleshoot_second_img05_jp.png"  alt="ログイン画面に表示されるメッセージ">}}  

クライアント証明書の有効期限が切れると、セキュアアクセスは利用できません。  
有効期限が切れる前に、管理者に新しいクライアント証明書の発行を依頼してください。  
クライアント証明書を差し替える手順は、[クライアント証明書の登録方法](/ja/settings/browser/certificate.html)を参照してください。  

## 「クライアント証明書の有効期限が過ぎています。」と表示されます。 {#login_troubleshoot_second_80}

セキュアアクセスを利用する場合は、有効期限内のクライアント証明書が必要です。  
発行済みのクライアント証明書の有効期限は延長できません。有効期限が過ぎている場合は、管理者が新しいクライアント証明書を発行する必要があります。  
クライアント証明書の有効期限は、{{%slash%}}共通管理画面で確認できます。  

{{< screen src="/general/img-ja/troubleshoot_second_img01_jp.png"  alt="管理画面のメニューを示す画像">}}
{{< screen src="/general/img-ja/troubleshoot_second_img04_jp.png"  alt="クライアント証明書の有効期限を確認する画像">}}

ユーザーは、新しいクライアント証明書をWebブラウザーに登録したあとで、再度ログインを試してください。  
クライアント証明書を差し替える手順は、[クライアント証明書の登録方法](/ja/settings/browser/certificate.html)を参照してください。  

{{% /disabled %}}

## ログイン画面が変わったように見えます。 {#login_troubleshoot_second_90}

SAML認証、または、別のサービスとのシングルサインオンが設定されていませんか？  
ログインに必要な情報は、管理者に確認してください。  

{{% disabled JP CN %}}

## 2要素認証プロセスで問題が発生しています。 {#login_troubleshoot_second_100}

{{% warning %}}
2要素認証は、[AWSに移行](https://www.kintone.com/aws-migration/)したお客様のみご利用いただけます。[ドメインID](/general/ja/admin/list_old/domainid.html)が「y」で始まるお客様が該当します。
{{% /warning %}}

下記のいずれかに該当していないか確認してください。  

* <b>確認コードを入力してもログインできない</b>  
  確認コードは一定の短い期間のみ有効です。新しいコードを試してください。  
<br>

* <b>確認コードが入手できない</b>  
  端末が手元にないなどで確認コードを入手できない場合は、2要素認証の設定を無効にする作業を{{%slash%}}共通管理者に依頼してください。  
  管理者による2要素認証の無効化は「ユーザー情報の編集」画面で行います。詳細は、[ユーザー情報を編集する](/general/ja/admin/list_useradmin/list_user/edit_user.html)を参照してください。  
  管理者が確認コードを入手できない場合は、[Contact US](https://www.kintone.com/support/)からお問い合わせください。  
<br>

* <b>別の問題が発生している</b>  
  [Contact US](https://www.kintone.com/support/)からお問い合わせください。  
<br>

{{% /disabled %}}
