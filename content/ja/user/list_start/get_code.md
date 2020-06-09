---
title: "2要素認証の確認コードを入手するには"
weight: 450
disabled: [JP,CN]
---
{{% warning %}}
この記事は、[AWSへの移行](https://www.kintone.com/aws-migration/)が完了したお客様向けです。[ドメインID](/general/ja/admin/list_old/domainid.html)が「y」で始まるお客様が該当します。
{{% /warning %}}

2要素認証を有効にしている場合、{{%cybozu_com%}}へのログイン時に、「ログイン名とパスワード」を入力したあとに、2要素認証の確認コードの入力が求められます。  
{{< screen src="/general/img-ja/get_code_01.png"  alt="入力画面">}}

## 確認コードの入手方法 {#list_start_get_code_10}

1. お使いのモバイル端末で、2要素認証の設定時にインストールした「Google認証システム」アプリを起動します。

1. 表示される6桁の確認コードを、{{%cybozu_com%}}の入力画面に入力します。  
  {{< screen src="/general/img-ja/get_code_02.png"  alt="確認コード表示画面">}}

1. [ログイン]をクリックします。

{{% note %}}
確認コードは一定時間が経過すると新しいものに変わります。「Google認証システム」画面の確認コードが変わった場合は、新しく表示された確認コードを入力してください。  
{{% /note %}}

## 確認コードが入手できない場合 {#list_start_get_code_20}

モバイル端末の不具合や、端末が手元にないなどの問題で確認コードが入手できない場合は、{{%slash%}}共通管理者に依頼し、2要素認証の設定を一時的に無効にしてもらう必要があります。  

管理者による2要素認証の無効化は「ユーザー情報の編集」画面で行います。  
詳細は、[ユーザー情報を編集する](/general/ja/admin/list_useradmin/list_user/edit_user.html)を参照してください。  

管理者が端末の紛失などのために確認コードを入手できない場合は、[Contact Us](https://www.kintone.com/support/)までお問い合わせください。  

{{% reference %}}

* [2要素認証とは](/general/ja/admin/list_security/list_access/2fa.html)
* [2要素認証を有効にする](/general/ja/user/list_personal/two_factor_authentication.html)

{{% /reference %}}
