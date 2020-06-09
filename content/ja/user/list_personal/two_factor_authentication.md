---
title: "2要素認証を有効にする"
weight: 250
disabled: [JP,CN]
---
{{% warning %}}
この記事は、[AWSへの移行](https://www.kintone.com/aws-migration/)が完了したお客様向けです。[ドメインID](/general/ja/admin/list_old/domainid.html)が「y」で始まるお客様が該当します。
{{% /warning %}}

2要素認証を使用し、{{%cybozu_com%}}へログインする際の認証を二重化することで、セキュリティを高めることができます。

## 2要素認証の概要 {#list_personal_two_factor_authentication_10}

[2要素認証とは](/general/ja/admin/list_security/list_access/2fa.html)を参照してください。

## 2要素認証を有効にするには {#list_personal_two_factor_authentication_20}

1. アカウント設定を表示します。  
  画面右上のユーザー名の右の![▼アイコン](/general/img/dropdown_jp_cn.png)をクリックし、ドロップダウンリストの[アカウント設定]をクリックします。  
  {{< screen src="/general/img-ja/two_factor_authentication_01.png"  alt="[アカウント設定]が赤枠で赤枠で囲まれた画像">}}  
1. [ログイン名とパスワード]をクリックします。  
   {{< screen src="/general/img-ja/two_factor_authentication_02.png"  alt="[ログイン名とパスワード]が赤枠で囲まれた画像">}}  
1. 2要素認証の項目の[有効にする]をクリックします。2要素認証の登録ダイアログが開きます。
1. お使いのモバイル端末に、Apple App StoreまたはGoogle Playから、Googleの「認証システム」アプリをダウンロードし、インストールします。
1. インストールした「認証システム」アプリで、画面に表示されているQRコードをスキャンします。  
1. 「認証システム」アプリが生成する6桁の確認コードを、登録ダイアログの入力欄に入力します。  
1. [有効にする]をクリックします。  

## トラブルシューティング {#list_personal_two_factor_authentication_30}

### 端末の紛失など {#list_personal_two_factor_authentication_3010}

モバイル端末の紛失などのために確認コードを入手できない場合は、管理者に依頼して2要素認証の設定を無効にしてもらう必要があります。  
管理者による2要素認証の無効化は「ユーザー情報の編集」画面で行います。  
詳細は、[ユーザー情報を編集する](/general/ja/admin/list_useradmin/list_user/edit_user.html)を参照してください。  

{{% note %}}
管理者が端末の紛失などのために確認コードを入手できない場合は、[Contact Us](https://www.kintone.com/support/)からお問い合わせください。
{{% /note %}}

### 端末の機種変更 {#list_personal_two_factor_authentication_3020}

以下の手順を行ってください。

1. 機種変更前のモバイル端末で確認コードを入手し、{{%cybozu_com%}}にログインします。
1. [2要素認証を有効にするには](#list_personal_two_factor_authentication_20)の手順1と2にしたがい、「ログイン名とパスワード」画面を表示します。
1. 2要素認証を無効にしたあと、再度有効にします。
1. 2要素認証の登録ダイアログが表示されたら、新しいモバイル端末で[2要素認証を有効にするには](#list_personal_two_factor_authentication_20)の手順4以降を行います。

{{% reference %}}

* [2要素認証とは](/general/ja/admin/list_security/list_access/2fa.html)
* [2要素認証の確認コードを入手するには](/general/ja/user/list_start/get_code.html)

{{% /reference %}}
