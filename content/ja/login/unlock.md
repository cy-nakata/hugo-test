---
title: "アカウントがロックされたら"
weight: 900
---

ユーザーのログイン失敗回数が、管理者が設定した値を超えると、そのユーザーは{{%service%}}にログインできなくなります。  
アカウントのロックを解除するには、方法1または方法2で対処します。  

## 方法1：{{%slash%}}共通管理者にロック解除を依頼する {#login_unlock_10}

{{%slash%}}共通管理者が、ユーザーのパスワードを変更するとロックを解除できます。  

### 管理者の操作 {#login_unlock_1010}

1. {{%slash%}}共通管理画面にアクセスします。

1. 「ユーザー管理」の[組織/ユーザー]をクリックします。
  {{< screen src="/general/img-ja/login_unlock_img01.png"  alt="組織とユーザーの設定画面">}}

1. パスワードを変更するユーザーの ![画像](/general/img/slash_edit_icon.png)をクリックします。
 {{< screen src="/general/img-ja/login_unlock_img02.png"  alt="組織とユーザーを選択する画面">}}

1. 画面右上の[パスワードの変更]をクリックします。
 {{< screen src="/general/img-ja/login_unlock_img03.png"  alt="ユーザー情報の編集画面">}}

1. 新しいパスワードを設定し、[変更してメールを送信]または[変更]をクリックします。  
  詳細は、[ユーザーのパスワードを変更する](/general/ja/admin/list_useradmin/list_user/edit_userpw.html#list_user_edituserpw_10)を参照してください。
 {{< screen src="/general/img-ja/login_unlock_img04.png"  alt="「パスワードの変更」ダイアログ">}}

1. 問題なくログインできるかを、ユーザーに確認します。

1. 必要に応じて、アカウントロックの設定を見直します。  
  詳細は、[ログイン失敗回数の上限を設定する](/general/ja/admin/list_security/list_login/account_lock.html)を参照してください。

## 方法2：「アカウントロックアウト解除までの時間」が経過するのを待つ {#login_unlock_20}

{{%slash%}}共通管理者が「アカウントロックアウト解除までの時間」に特定の時間を設定していれば、その時間が経過すればロックは解除されます。  
{{% enabled JP CN %}}
初期設定は「解除しない」になっています。
{{% /enabled %}}
{{% enabled US %}}
初期設定は「3分」です。  
{{% /enabled %}}

「アカウントロックアウト解除までの時間」の設定箇所は、[ログイン失敗回数の上限を設定する](/general/ja/admin/list_security/list_login/account_lock.html)を参照してください。

### 設定時間が「解除しない」の場合 {#login_unlock_2010}

「アカウントロックアウト解除までの時間」が「解除しない」に設定されていると、時間が経過してもロックは解除されません。  
この場合、[方法1：{{%slash%}}共通管理者にロック解除を依頼する](/general/ja/login/unlock.html#login_unlock_10)で対処してください。  

## 管理者がロックアウトされた場合 {#login_unlock_30}

{{% enabled JP %}}

{{%slash%}}共通管理者がロックアウトされた場合、{{%store%}}で一時的な管理者を作成してから自分のパスワードを変更します。  

1. [{{%store%}}](https://store.{{%cybozu_com%}}/login)にアクセスします。  
1. [一時的な管理者を作成](/general/ja/login/admin_temp.html)します。  
1. 手順2で作成した一時的な管理者のアカウントでログインします。
1. {{%slash%}}共通管理画面にアクセスします。  
1. 「ユーザー管理」の[組織/ユーザー]をクリックします。  
1. ロックされた管理者のユーザー情報を表示し、パスワードを変更します。  
1. ログアウトします。  
1. 管理者自身のアカウントでログインできるか確認します。  
1. 不要になった「一時的な管理者」を使用停止にします。  
  詳細は、[ユーザーを使用停止にする](/general/ja/admin/list_useradmin/list_user/stop_user.html#list_user_stop_user_10)を参照してください。

{{% /enabled %}}

{{% enabled CN %}}
[{{%CorpName%}}にお問い合わせ](https://www.cybozu.cn/free.html)ください。
{{% /enabled %}}

{{% enabled US %}}
[{{%CorpName%}}にお問い合わせ](https://www.kintone.com/support/)ください。
{{% /enabled %}}
