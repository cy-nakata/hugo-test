---
title: "管理者が退職したため、{{%service%}}の管理画面にアクセスできません。"
weight: 800
disabled: [JP]
---

{{% reference %}}
関連ページです。関連ページです。関連ページです。
* [リンク名](URL)
* [リンク名](URL)
{{% /reference %}}

{{% seealso title="関連する記事" %}}
[リンク名](URL)
{{% /seealso %}}

{{% enabled CN %}}

前任の管理者の退職などで、{{%service%}}の管理画面にアクセスできない場合は、[お問い合わせ](https://www.cybozu.cn/free.html)ください。

{{% /enabled %}}

{{% enabled US %}}

<!-- 下記はyakumo向けの内容です -->

前任の管理者の退職などで、{{%service%}}の管理画面にアクセスできなくなった場合の対処を案内します。  

## 前任の管理者のアカウントが分かる場合 {#login_admin_retire_10}

前任の管理者のメールアカウントと{{%service%}}のログイン名が分かる場合は、パスワードリセットを試してください。  

1. ログイン画面の[ログインでお困りですか？]をクリックします。  
  {{< screen src="/general/img-ja/admin_retire_img01_us.png"  alt="ログイン画面">}}  

1. 前任の管理者のメールアドレスを入力し、[パスワードリセット]をクリックします。  
  メールアドレスの入力画面が表示されない場合は、[前任の管理者のアカウントが分からない場合](#login_admin_retire_20)に進みます。  
  {{< screen src="/general/img-ja/admin_retire_img02.png"  alt="メールアドレスの入力画面">}}  

1. パスワードリセットを案内するメールを受信します。  
  メールを受信できない場合は、[前任の管理者のアカウントが分からない場合](#login_admin_retire_20)に進みます。  

1. メールに記載されている[パスワード再設定URL]をクリックします。  

1. 新しいパスワードを設定します。  
  [保存]をクリックすると、ログイン画面が表示されます。  

1. 前任の管理者のログイン名と変更後のパスワードで、{{%service%}}にログインします。  

1. 新しい管理者を登録します。  
  管理者がログインできない事態を回避できるよう、複数人設定することをおすすめします。  
  詳細は、[{{%slash%}}共通管理者の設定](/general/ja/admin/list_administrator/list_type_of_administrator/list_domain_auth.html)を参照してください。  

1. {{%service%}}からログアウトします。  

1. 新しく登録した管理者で{{%service%}}にログインします。  

1. 前任の管理者のアカウントを使用停止にします。  
  詳細は、[ユーザーを使用停止にする／使用を再開する](/general/ja/admin/list_useradmin/list_user/stop_user.html)を参照してください。  

1. 前任の管理者のアカウントを削除しても問題ないかを確認します。  
  詳細は、[ユーザーを削除した場合に削除されるデータについて](/general/ja/admin/list_useradmin/list_user/deleted_data.html)を参照してください。  

1. 必要に応じて、前任の管理者のアカウントを削除します。  
  詳細は、[ユーザーを削除する](/general/ja/admin/list_useradmin/list_user/delete_user.html)を参照してください。  

## 前任の管理者のアカウントが分からない場合 {#login_admin_retire_20}

[Contact Us](https://www.kintone.com/support/)からお問い合わせください。  

{{< seealso title="関連する記事" >}}

* [ログインできない：最初に確認すること](/general/ja/login/troubleshoot_first.html)
* [ログインできない：次に確認すること](/general/ja/login/troubleshoot_second.html)
* [管理者がアカウントやパスワードを忘れた場合](/general/ja/login/admin_account.html)

{{< /seealso >}}

{{% /enabled %}}
