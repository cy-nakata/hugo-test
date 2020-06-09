---
title: "管理者がアカウントやパスワードを忘れた場合"
weight: 600
---

{{% enabled CN %}}

* {{%slash%}}共通管理者が複数いる場合：  
  自分以外の管理者に、自分のパスワード変更を依頼します。  
  操作の詳細は、[パスワードを変更する](/general/ja/admin/list_useradmin/list_user/edit_userpw.html)を参照してください。  
* {{%slash%}}共通管理者が1人しかいない場合：  
  パスワードを忘れるなどしてログインできない場合は、[お問い合わせ](https://www.cybozu.cn/free.html)ください。

{{% /enabled %}}

{{% disabled CN %}}
管理者がログインできない場合は、方法1から順に試してください。  

## 方法1 パスワードをリセットする {#login_admin_account_10}

{{% enabled JP %}}

1. ログイン画面の[ログインでお困りですか？]をクリックします。
  {{< screen src="/general/img-ja/admin_account_img03.png"  alt="ログイン画面">}}

1. {{%service%}}のユーザー情報に登録されているメールアドレスを入力し、[パスワードリセット]をクリックします。  
  <br>
  下記の状況の場合は、[方法2 一時的な管理者を作成する](#login_admin_account_20)に進みます。  

    * ログイン名が分からない
    * メールアドレスの入力画面が表示されない
    * パスワードのリセットに必要なメールアドレスが分からない
  {{< screen src="/general/img-ja/admin_account_img02.png"  alt="メールアドレスの入力画面">}}  
  上記の画面が表示されない場合は、[パスワードをリセットできません。](/general/ja/login/cannot_reset_pw.html)を参照してください。  

1. パスワードリセットを案内するメールを受信します。  

1. メールに記載されている[パスワード再設定URL]をクリックします。  

1. 新しいパスワードを設定します。  
  [保存]をクリックすると、ログイン画面が表示されます。  

1. 変更後のパスワードでログインできることを確認します。  

{{% /enabled %}}

{{% enabled US %}}

1. ログイン画面の[ログインでお困りですか？]をクリックします。  
  {{< screen src="/general/img-ja/admin_account_img01_us.png"  alt="ログイン画面">}}  

1. {{%service%}}のユーザー情報に登録されているメールアドレスを入力し、[パスワードリセット]をクリックします。  
  {{< screen src="/general/img-ja/admin_account_img02.png"  alt="メールアドレスの入力画面">}}  
  メールアドレスの入力画面が表示されない場合や、入力するメールアドレスが分からない場合は、[ドメインIDを確認](/general/ja/admin/list_old/domainid.html)してから下記の対処をします。  

    * <b>[AWSへの移行](https://www.kintone.com/aws-migration/)が完了したお客様</b>（ドメインIDが「y」で始まるお客様）  
      [Contact Us](https://www.kintone.com/support/)からお問い合わせください。  

    * <b>[AWSへの移行](https://www.kintone.com/aws-migration/)が完了していないお客様</b>（ドメインIDが「c」で始まるお客様）  
      [方法2 一時的な管理者を作成する](#login_admin_account_20)に進みます。  

1. パスワードリセットを案内するメールを受信します。  

1. メールに記載されている[パスワード再設定URL]をクリックします。  

1. 新しいパスワードを設定します。  
  [保存]をクリックすると、ログイン画面が表示されます。  

1. 変更後のパスワードでログインできることを確認します。  

  {{% /enabled %}}

## 方法2 一時的な管理者を作成する {#login_admin_account_20}

{{% enabled US %}}
{{% warning %}}
一時的な管理者は、[AWSに移行](https://www.kintone.com/aws-migration/)したお客様は作成できません。[ドメインID](/general/ja/admin/list_old/domainid.html)が「y」で始まるお客様が該当します。

**[AWSへの移行](https://www.kintone.com/aws-migration/)が完了したお客様（ドメインIDが「y」で始まるお客様）**  
{{%slash%}}共通管理者がログイン名を忘れるなどしてログインできない場合は、[サイボウズにお問い合わせ](https://www.kintone.com/support/)ください。
{{% /warning %}}
{{% /enabled %}}

{{%store%}}管理者が「一時的な管理者」を作成することで、新たな管理者を設定できます。  
詳細は、[一時的な管理者を作成する](/general/ja/login/admin_temp.html)を参照してください。  

## 方法3 {{%CorpName%}}に問い合わせ {#login_admin_account_30}

{{% enabled JP %}}
方法1や方法2でも解決しない場合は、管理者から{{%CorpName%}}にお問い合わせください。  

* [お問い合わせフォーム](https://r.cybozu.com/store/jp/inquiry/common.html)

{{% /enabled %}}

{{% enabled US %}}
方法1や方法2でも解決しない場合は、管理者から{{%CorpName%}}にお問い合わせください。  

* [Contact Us](https://www.kintone.com/support/)

{{% /enabled %}}

{{% /disabled %}}
