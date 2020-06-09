---
title: "Webブラウザーからサービスにアクセスする"
weight: 100
---
{{% enabled US %}}
{{% warning %}}
この記事は、[AWSへの移行](https://www.kintone.com/aws-migration/)が完了していないお客様向けです。ドメインIDが「c」で始まるお客様が該当します。ドメインIDを確認するには「[ドメインIDの確認方法](/general/ja/admin/list_old/domainid.html)」を参照してください。
{{% /warning %}}
{{% /enabled %}}

オフィス外からWebブラウザーで{{%service%}}のサービスにアクセスするために必要な設定を説明します。  
セキュアアクセスを利用している場合と利用していない場合で、設定方法が異なります。

## セキュアアクセスを利用している場合{#remote_webbrowser_10}

### STEP1：「モバイルからのアクセス」画面を表示する{#remote_webbrowser_1010}

{{% enabled JP %}}

1. アカウント設定を表示します。  
  アカウント設定を表示する方法は、サービスによって異なります。  
   * サイボウズ Office、Garoon、またはメールワイズの場合：  
     画面右上のユーザー名をクリックし、ドロップダウンリストの[アカウント設定]を選択します。  
     Garoonの例：  
    {{< screen src="/general/img-ja/remote_img01.png"  alt="[アカウント設定]が赤枠で囲まれた画像">}}
   * {{%kintone%}}の場合：  
    画面右上のユーザー名の右の ![▼アイコン](/general/img/dropdown_jp_cn.png) をクリックし、ドロップダウンリストの[アカウント設定]をクリックします。
   　{{< screen src="/general/img-ja/remote_img02.png"  alt="[アカウント設定]が赤枠で囲まれた画像">}}

1. [モバイルからのアクセス]をクリックします。
    {{< screen src="/general/img-ja/webbrowser_01.png"  alt="プロフィール画面">}}
    「モバイルからのアクセス」や「クライアント証明書の情報」が表示されない場合、[「モバイルからのアクセス」画面や「クライアント証明書の情報」が表示されない場合](/general/ja/user/list_access/access_service.html)の対処方法を確認してください。

{{% /enabled %}}

{{% enabled US %}}

1. アカウント設定を表示します。  
    * {{%kintone%}}の場合：  
    画面右上のユーザー名の右の ![▼アイコン](/general/img/dropdown_jp_cn.png) をクリックし、ドロップダウンリストの[アカウント設定]をクリックします。
    {{< screen src="/general/img-ja/remote_img01_us.png"  alt="[アカウント設定]が赤枠で囲まれた画像">}}
1. [モバイルからのアクセス]をクリックします。
    {{< screen src="/general/img-ja/webbrowser_01.png"  alt="プロフィール画面">}}
    「モバイルからのアクセス」や「クライアント証明書の情報」が表示されない場合、[「モバイルからのアクセス」画面や「クライアント証明書の情報」が表示されない場合](/general/ja/user/list_access/access_service.html)の対処方法を確認してください。

{{% /enabled %}}

{{% enabled CN %}}

1. アカウント設定を表示します。  
  アカウント設定を表示する方法は、サービスによって異なります。  
    * Garoonの場合：  
    画面右上のユーザー名をクリックし、ドロップダウンリストの[アカウント設定]を選択します。  
    {{< screen src="/general/img-ja/remote_img01.png"  alt="[アカウント設定]が赤枠で囲まれた画像">}}
    * {{%kintone%}}の場合：  
    画面右上のユーザー名の右の ![▼アイコン](/general/img/dropdown_jp_cn.png) をクリックし、ドロップダウンリストの[アカウント設定]をクリックします。
    {{< screen src="/general/img-ja/remote_img02_cn.png"  alt="[アカウント設定]が赤枠で囲まれた画像">}}
1. [モバイルからのアクセス]をクリックします。
    {{< screen src="/general/img-ja/webbrowser_01.png"  alt="プロフィール画面">}}
    「モバイルからのアクセス」や「クライアント証明書の情報」が表示されない場合、[「モバイルからのアクセス」画面や「クライアント証明書の情報」が表示されない場合](/general/ja/user/list_access/access_service.html)の対処方法を確認してください。

{{% /enabled %}}

### STEP2：クライアント証明書のファイルを利用する端末に送信する{#remote_webbrowser_1020}

1. 「クライアント証明書の情報」欄に記載されているパスワードを控えます。このあとの手順で必要になります。  
    {{< screen src="/general/img-ja/webbrowser_02.png"  alt="クライアント証明書の情報が表示されている画像">}}
1. [Webブラウザーからアクセスする]をクリックします。
    {{< screen src="/general/img-ja/webbrowser_03.png"  alt="[Webブラウザーからアクセスする]が赤枠で囲まれた画像">}}
1. 利用する端末で受信可能なEmailアドレスを入力して「送信」をクリックします。  
  クライアント証明書（********.pfx）が添付されたメールが届きます。
    {{< screen src="/general/img-ja/webbrowser_05.png"  alt="Emailアドレスを入力する画像">}}
1. 受信したメールに添付されているクライアント証明書（********.pfx）を、任意のフォルダーに保存します。

### STEP3：クライアント証明書を登録する{#remote_webbrowser_1030}

メールまたは管理者から入手したクライアント証明書（********.pfx）を登録します。  
クライアント証明書の登録方法は、Webブラウザーの種類によって異なります。[サポートガイド「クライアント証明書を登録する」](/ja/settings/browser/certificate.html)を参照してください。 　

{{% note %}}
{{% subtitle %}}iOS用のGmailアプリまたはOutlookアプリを利用している場合{{% /subtitle %}}
クライアント証明書（********.pfx）を開けません。アプリではなく、SafariからGmailまたはOffice365にアクセスして、メールに添付されたクライアント証明書を開いてください。

{{% subtitle %}}Androidを利用している場合{{% /subtitle %}}
端末の設定やOSのバージョンによって、クライアント証明書の登録に画面ロックの設定を必要とする場合があります。画面ロックが未設定の場合、クライアント証明書を登録する際に、画面ロックの設定が要求されます。
{{% /note %}}

### STEP4：{{%service%}}にアクセスする{#remote_webbrowser_1040}

{{% enabled JP %}}

Webブラウザーを起動し、受信したメールに記載されているアクセスURL（https://（サブドメイン名）<b>.s</b>.{{%cybozu_com%}}）にアクセスします。  

{{< screen src="/general/img-ja/webbrowser_04.png"  alt="メールの画像">}}

{{% /enabled %}}

{{% enabled US %}}

Webブラウザーを起動し、受信したメールに記載されているアクセスURL（https://（サブドメイン名）<b>.s</b>.{{%cybozu_com%}}）にアクセスします。  

{{< screen src="/general/img-ja/webbrowser_04_us.png"  alt="メールの画像">}}

{{% /enabled %}}

{{% enabled CN %}}

Webブラウザーを起動し、受信したメールに記載されているアクセスURL（https://（サブドメイン名）<b>.s</b>.{{%cybozu_com%}}）にアクセスします。  

{{< screen src="/general/img-ja/webbrowser_04_cn.png"  alt="メールの画像">}}

{{% /enabled %}}

## セキュアアクセスを利用していない場合{#remote_webbrowser_20}

サービスのURLにアクセスした際に、ログイン画面が表示される場合と、認証ウィンドウが表示される場合で手順が異なります。

1. WebブラウザーでサービスのURL（https://（サブドメイン名）.{{%cybozu_com%}}/）にアクセスします。

  * <b>ログイン画面が表示される場合</b>  
    {{%cybozu_com%}}のログイン名とパスワードを入力してログインします。
  * <b>認証ウィンドウが表示される場合</b>  
    Basic認証を使用している場合は、ログイン画面の前に次のような認証ウィンドウが表示されます。  
    システム管理者にBasic認証のユーザー名とパスワードを確認して、手順2にすすみます。
    {{< screen src="/general/img-ja/webbrowser_img08.png"  alt="chromeの認証ウィンドウの画像">}}
   認証ウィンドウは、OSやWebブラウザーによって異なります。

1. 認証ウィンドウに、システム管理者に確認したBasic認証のユーザー名とパスワードを入力します。  
1. 認証に成功したら、{{%service%}}のログイン名とパスワードを入力してログインします。
