---
title: "自動ログインできません。"
weight: 520
---

自動ログインを有効にするには、[管理者の設定](/general/ja/admin/list_security/list_login/simplifiy.html#list_login_simplifiy_3010)と[ユーザーの操作](/general/ja/admin/list_security/list_login/simplifiy.html#list_login_simplifiy_3020)の両方が必要です。

## 管理者の設定は完了しているが、自動ログインできない場合 {#login_auto_login_10}

[管理者の設定](/general/ja/admin/list_security/list_login/simplifiy.html#list_login_simplifiy_3010)が完了していても、自動ログインが有効にならない場合、次の原因が考えられます。  

* ログアウトしている
* ログイン画面で「ログイン名を保存する」を選択していない

1. {{%service%}}にログインしたままの状態で、Webブラウザーの[&times;]をクリックします。
  {{< screen src="/general/img-ja/login_auto_login_img01.png"  alt="Webブラウザーの閉じるボタンを示す画像">}}
  自動ログインの設定にかかわらず、ログアウトしてしまうと、ログイン情報のcookieが破棄されてしまいます。  
  自動ログイン機能を利用する場合は、ログアウトはしないでください。  

1. ログイン画面を表示します。

1. 「ログイン名を保存する」を選択します。
  {{< screen src="/general/img-ja/login_auto_login_img02.png"  alt="ログイン画面">}}

1. ログイン名とパスワードを入力し、ログインします。

## 管理者が自動ログインを許可していない場合 {#login_auto_login_20}

自動ログインは、{{%slash%}}共通管理者が利用を許可している場合にのみ利用できます。  
管理者が自動ログインを許可せずに、[ユーザーの操作](/general/ja/admin/list_security/list_login/simplifiy.html#list_login_simplifiy_3020)だけ実施した場合、ログイン名のみWebブラウザーに保存されます。自動ログインはできません。
