---
title: "「モバイルからのアクセス」画面や「クライアント証明書の情報」が表示されない場合"
weight: 300
---
{{% enabled US %}}
{{% warning %}}
この記事は、[AWSへの移行](https://www.kintone.com/aws-migration/)が完了していないお客様向けです。ドメインIDが「c」で始まるお客様が該当します。ドメインIDを確認するには「[ドメインIDの確認方法](/general/ja/admin/list_old/domainid.html)」を参照してください。
{{% /warning %}}
{{% /enabled %}}

[モバイルからのアクセス画面を表示する](/general/ja/user/list_access/remote/webbrowser.html#remote_webbrowser_1010)手順を行っても、「モバイルからのアクセス」画面が表示されない場合や、クライアント証明書の情報が表示されない場合の対処方法を説明します。

## 「モバイルからのアクセス」が表示されない場合{#access_service_10}

セキュアアクセスを契約していても「モバイルからのアクセス」が表示されない場合は、管理者にクライアント証明書の発行を依頼してください。  
管理者が行う作業は、[クライアント証明書を発行する](/general/ja/admin/list_security/list_secureaccess/secureaccess.html#list_secureaccess_secureaccess_30)方法を参照してください。

{{< screen src="/general/img-ja/access_service_img01.png" alt="モバイルからのアクセスが表示されていない画像">}}  

## 「クライアント証明書の情報」が表示されない場合{#access_service_20}

次のいずれかに該当する場合、クライアント証明書の情報が表示されません。

* <b>クライアント証明書のダウンロードが禁止されている</b>  
  管理者が、[ユーザーによるクライアント証明書のダウンロードを禁止](/general/ja/admin/list_security/list_secureaccess/secureaccess.html#list_secureaccess_secureaccess_402010)しています。  
  Webブラウザーからアクセスする場合は、管理者からクライアント証明書とパスワードを受け取り、[STEP3：クライアント証明書を登録する](/general/ja/user/list_access/remote/webbrowser.html#remote_webbrowser_1030)に進みます。  
  スマートフォンアプリからのアクセスは、管理者がクライアント証明書のダウンロードを許可しないかぎりできません。
{{< screen src="/general/img-ja/access_service_img02.png" alt="クライアント証明書の情報が表示されていない画像">}}

* <b>クライアント証明書の有効期限が過ぎている</b>  
  システム管理者に、クライアント証明書を再発行するよう依頼してください。  
  管理者が行う作業は、[クライアント証明書を発行する](/general/ja/admin/list_security/list_secureaccess/secureaccess.html#list_secureaccess_secureaccess_30)方法を参照してください。
  {{< screen src="/general/img-ja/access_service_img03.png" alt="クライアント証明書の有効期限が過ぎている画像">}}

* <b>セキュアアクセスを契約していない</b>  
  「クライアント証明書の情報」は表示されません。  
  Webブラウザーからアクセスする手順は、[セキュアアクセスを利用していない場合](/general/ja/user/list_access/remote/webbrowser.html#remote_webbrowser_20)を参照してください。  
  スマートフォンアプリからアクセスする手順は、[スマートフォンアプリからサービスにアクセスする](/general/ja/user/list_access/remote/mobileapp.html)方法を参照してください。
  {{< screen src="/general/img-ja/access_service_img04.png" alt="セキュアアクセスを契約していない画像">}}
