---
title: "パスワードの有効期間について"
weight: 450
---

パスワードの有効期間に関するFAQを案内します。  

## パスワードの有効期間が適用されるタイミング {#list_login_pw_date_10}

パスワードの有効期間は、管理者が設定を変更した日付ではなく、ユーザーがパスワードを変更した日付から計算されます。  

* 例：  
  ユーザーAが3月10日にパスワードを変更した。  
  その後、{{%slash%}}共通管理者が3月25日にパスワードの有効期間を「30日」に変更した。
  この場合、ユーザーAのパスワードは、3月10日から数えて30日後の4月9日に期限が切れる。  

## パスワードの有効期間が近づいたら {#list_login_pw_date_20}

パスワードの有効期間の5日前になると、有効期間までの残りの日数と、パスワードの変更を促すメッセージがログイン後の画面に表示されます。  
メッセージをクリックすると、パスワードを変更できます。  

{{% note %}}
{{% enabled JP CN %}}
KUNAI、または{{%kintone%}}モバイルでアクセスする場合、パスワードの有効期間までの残りの日数はアプリに通知されません。
{{% /enabled %}}
{{% enabled US %}}
{{%kintone%}}モバイルでアクセスする場合、パスワードの有効期間までの残りの日数はアプリに通知されません。
{{% /enabled %}}
{{% /note %}}

## パスワードの有効期間が過ぎたら {#list_login_pw_date_30}

有効期間を過ぎたパスワードではログインできません。  
ログインしようとすると、パスワードの再設定画面が表示されます。新しいパスワードを設定すると、{{%service%}}にログインできます。  

{{% enabled JP CN %}}

## クライアントツールを使用している場合 {#list_login_pw_date_40}

下記のクライアントツールを使用している場合、パスワードの有効期間が過ぎると、クライアントツールを使用できなくなります。  
{{%cybozu_com%}}でパスワードを変更した後、クライアントツールに設定しているパスワードを変更すると、再び使用できるようになります。  

* [Cybozu Desktop 2(Windows版)：接続設定](https://jp.cybozu.help/ja/dt2/win/settings.html)  
* [Cybozu Desktop 2(Mac版)：接続設定](https://jp.cybozu.help/ja/dt2/mac/settings.html)  
* [KUNAI for iPhone：接続設定マニュアル](https://manual.cybozu.co.jp/kunai/ip/setting/index.html)  
* [KUNAI for Android：接続設定マニュアル](https://manual.cybozu.co.jp/kunai/an/setting/index.html)

{{% /enabled %}}

## 特定のユーザーのパスワードを不変にしたい {#list_login_pw_date_50}

役員のアカウントやサービスの管理者アカウントなど、特定のユーザーには有効期間を適用したくない場合には、パスワードの有効期間を「無期限」に変更できます。  
詳細は、[パスワードを個別に変更する](/general/ja/admin/list_useradmin/list_user/edit_userpw.html#list_user_edituserpw_10)の「パスワードは変更せず、有効期間を無期限にする場合」を参照してください。  

ただし、管理者が設定した仮パスワードの変更を求める設定をしている場合は、上記の設定をしていても、仮パスワードの変更が要求されます。  
詳細は、[管理者が設定した仮パスワードの変更を許可する](/general/ja/admin/list_security/list_login/pw_allow.html#list_login_pw_allow_10)を参照してください。

## ユーザーによるパスワード変更を禁止にしている場合 {#list_login_pw_date_60}

ユーザーによるパスワードの変更を禁止にしている場合、パスワードの有効期間は適用されません。  
パスワードの有効期間を適用する場合は、パスワードの変更をユーザーに許可してください。  
詳細は、[プロフィール画面でのパスワード変更を許可する](/general/ja/admin/list_security/list_login/pw_allow.html#list_login_pw_allow_20)を参照してください。  
