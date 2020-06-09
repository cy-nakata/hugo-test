---
title: "ログインを簡易にする"
weight: 500
---

{{%service%}}へのログイン認証を簡略化できます。  
ただし、ログイン認証を簡略化すると、セキュリティが低下し、不正なログインを招く恐れがあります。  
セキュリティが低下することをご理解のうえ設定してください。  
各設定の初期値は、[ログイン認証の簡略化に関する初期値](/general/ja/admin/list_security/list_login/overview.html#list_login_overview_10)を参照してください。

{{% disabled US %}}

## ログイン名の自動補完を有効にする {#list_login_simplifiy_10}

ログイン名の入力の自動補完を有効にするかどうかを設定します。  
設定を有効にすると、ログイン画面でログイン名を入力するときに、ログイン名の候補が表示されます。  
{{< screen src="/general/img-ja/list_login_simplifiy_img07.png"  alt="ログイン画面">}}

1. 外部からのアクセスを制限する設定をします。  
  自動補完だけを有効にすると、第三者がログイン名一覧を閲覧するおそれがあります。  
  次のいずれか1つを設定します。
    * [IPアドレス制限とは](/general/ja/admin/list_security/list_access/ip_restrictions.html)
    * [Basic認証とは](/general/ja/admin/list_security/list_access/basic_auth.html)
    * [セキュアアクセスとは](/general/ja/admin/list_security/list_access/secureaccess.html)
    <!-- * [2要素認証](★あとで) -->

1. {{%slash%}}共通管理画面にアクセスします。

1. 「セキュリティ」の[ログイン]をクリックします。
  {{< screen src="/general/img-ja/list_login_simplifiy_img01.png"  alt="[ログイン]が赤枠で囲まれた画像">}}

1. 「ログイン名の入力」セクションで、「自動補完を有効にする」を選択します。  
  {{< screen src="/general/img-ja/list_login_simplifiy_img02.png"  alt="ログインに関するセキュリティの設定画面">}}

1. 画面下部の[保存]をクリックします。  

{{% /disabled %}}

## ログイン名とパスワードのWebブラウザーへの保存を許可する {#list_login_simplifiy_20}

ログイン名とパスワードのWebブラウザーへの保存を許可するかどうかを設定します。  
一部のWebブラウザーでは、Webブラウザーでの設定が優先されます。  

* Google Chromeの例：  
  {{< screen src="/general/img-ja/list_login_simplifiy_img08.png"  alt="Google Chromeの画面例">}}

1. {{%slash%}}共通管理画面にアクセスします。

1. 「セキュリティ」の[ログイン]をクリックします。
  {{< screen src="/general/img-ja/list_login_simplifiy_img01.png"  alt="[ログイン]が赤枠で囲まれた画像">}}

1. 「ログイン名とパスワードの保存」セクションで、「ログイン名とパスワードのWebブラウザーへの保存を許可する」を選択します。  
  {{< screen src="/general/img-ja/list_login_simplifiy_img03.png"  alt="ログインに関するセキュリティの設定画面">}}

1. 画面下部の[保存]をクリックします。  

## 自動ログインを許可する {#list_login_simplifiy_30}

自動ログインとは、Webブラウザーを閉じてもログイン状態を維持できる機能です。  
自動ログインを有効にするには、[管理者の設定](#list_login_simplifiy_3010)と[ユーザーの操作](#list_login_simplifiy_3020)の両方が必要です。  

### 管理者の設定 {#list_login_simplifiy_3010}

1. {{%slash%}}共通管理画面にアクセスします。

1. 「セキュリティ」の[ログイン]をクリックします。
  {{< screen src="/general/img-ja/list_login_simplifiy_img01.png"  alt="[ログイン]が赤枠で囲まれた画像">}}

1. 「自動ログイン」セクションで、「自動ログインをユーザーに許可する」を選択します。  
  {{< screen src="/general/img-ja/list_login_simplifiy_img04.png"  alt="ログインに関するセキュリティの設定画面">}}

1. 自動ログインの有効期間を選択します。  
  ここで指定した期間にのみ、自動ログインが適用されます。
  {{< screen src="/general/img-ja/list_login_simplifiy_img09.png"  alt="ログインに関するセキュリティの設定画面">}}

1. [ログインセッションの有効期間を設定](#list_login_simplifiy_40)します。  
  自動ログインをユーザーに許可する際は、不正なアクセスを防げるよう、ログインセッションの有効期間を設定してください。

1. 画面下部の[保存]をクリックします。  

1. 自動ログイン機能を利用する場合は、[ユーザーの操作](#list_login_simplifiy_3020)をすることをアナウンスします。  

### ユーザーの操作 {#list_login_simplifiy_3020}

1. ログイン画面を表示します。

1. 「ログイン名を保存する」を選択します。
  {{< screen src="/general/img-ja/list_login_simplifiy_img05.png"  alt="ログイン画面">}}

1. ログイン名とパスワードを入力し、ログインします。  
  [管理者の設定](#list_login_simplifiy_3010)で指定された有効期間で、自動ログインが利用できるようになります。  

### 管理者が自動ログインを許可していない場合 {#list_login_simplifiy_3030}

自動ログインを有効にするには、[管理者の設定](#list_login_simplifiy_3010)と[ユーザーの操作](#list_login_simplifiy_3020)の両方が必要です。  
管理者が自動ログインを許可せずに、ユーザーの操作だけ実施した場合、ログイン名のみWebブラウザーに保存されます。自動ログインはできません。

## ログインセッションの有効期間を設定する {#list_login_simplifiy_40}

ここで設定する有効期間とは、{{%service%}}への最後のアクセスからログアウトするまでの期間を指します。  
自動ログインをユーザーに許可する際は、不正なアクセスを防げるよう、ログインセッションの有効期間を設定してください。

1. {{%slash%}}共通管理画面にアクセスします。

1. 「セキュリティ」の[ログイン]をクリックします。
  {{< screen src="/general/img-ja/list_login_simplifiy_img01.png"  alt="[ログイン]が赤枠で囲まれた画像">}}

1. 「セッション」セクションで、有効期間を選択します。  
  {{< screen src="/general/img-ja/list_login_simplifiy_img06.png"  alt="ログインに関するセキュリティの設定画面">}}

1. 画面下部の[保存]をクリックします。  
