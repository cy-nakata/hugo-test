---
title: "セキュアアクセスを利用したログインの流れ"
weight: 170
disabled: [US]
---

1. 使用するWebブラウザーやモバイル端末に、クライアント証明書をインストールします。  
  詳細は、[クライアント証明書の登録方法](/ja/settings/browser/certificate.html)を参照してください。  
  OSやWebブラウザーのバージョンによって、手順は異なります。  
  クライアント証明書は、有効期間が切れるまで端末にインストールしたままにします。  

1. 手順1で準備したWebブラウザーまたはモバイル端末から、{{%service%}}のログイン画面にアクセスします。
    * ログインURL：https://（サブドメイン名）.{{%cybozu_com%}}

1. 「このボタンをチェックすると、以後自動的にリダイレクトします。」を選択します。  
  {{< screen src="/general/img-ja/list_secureaccess_login_flow_img01.png"  alt="Code403の画面">}}
  このチェックボックスを選択しておくと、次回から「Code: 403 Forbidden」エラーは表示されません。  

1. URLをクリックします。  
  {{< screen src="/general/img-ja/list_secureaccess_login_flow_img02.png"  alt="Code403の画面">}}
  {{%service%}}のログイン画面に移動します。  

1. {{%service%}}のログイン名とパスワードを入力し、[ログイン]をクリックします。  
  これで、ログインは完了です。  
  {{< screen src="/general/img-ja/list_secureaccess_login_flow_img03.png"  alt="ログイン画面">}}

## 「Code: 496 No Cert」と表示される場合  {#list_secureaccess_login_flow_10}

セキュアアクセス用のURL「https://（サブドメイン名）**.s**.{{%cybozu_com%}}/」にアクセスした際に、「アクセスにはクライアント証明書が必要です。Code: 496 No Cert」と表示されて、アクセスできないことがあります。  
  {{< screen src="/general/img-ja/list_secureaccess_login_flow_img04.png"  alt="Code496の画面">}}

### 対処方法  {#list_secureaccess_login_flow_1010}

セキュアアクセスを利用するには、使用するWebブラウザーやモバイル端末にクライアント証明書を登録する必要があります。  
クライアント証明書が登録されているかどうか確認し、再度アクセスしてください。  

1. Webブラウザーまたはモバイル端末に、クライアント証明書が登録されているか確認します。  
  OSやWebブラウザーのバージョンによって、手順は異なります。  
    * **Google Chromeの場合：**  
      画面右上の「![Googleメニューアイコン](/general/img/google_menu.png) 」&gt; [設定] &gt;「プライバシーとセキュリティ」セクションの[証明書の管理] &gt;「個人」タブ
    * **iOSの場合：**  
      ホーム画面の[設定] &gt; [一般] &gt; [プロファイル]

1. Webブラウザーを再起動します。  

1. お使いのWebブラウザーやモバイル端末にあわせて、下記の操作を実行します。  
    * **Google ChromeまたはAndroid Chromeの場合：**  
      シークレットモードでアクセスします。  
      詳細は、Google社：[プライベート ブラウジングページ](https://support.google.com/chrome/answer/95464?hl=ja)を参照してください。
    * **Internet Explorerの場合：**  
      [ツール] &gt; [インターネットオプション] &gt; 「コンテンツ」タブ &gt; [SSL状態のクリア]を実行します。  
