---
title: "クライアント証明書の有効期限を迎えるユーザーに、クライアント証明書を発行する"
weight: 400
---
{{% enabled US %}}
{{% warning %}}
セキュアアクセスは、[AWSに移行](https://www.kintone.com/aws-migration/)したお客様（[ドメインID](/general/ja/admin/list_old/domainid.html)が「y」で始まるお客様）にはご利用いただけません。
{{% /warning %}}
{{% /enabled %}}

発行済みのクライアント証明書の有効期限は延長できません。クライアント証明書の有効期限後もセキュアアクセスを利用してサービスにアクセスする場合は、クライアント証明書を再発行する必要があります。

ここでは、ユーザーが使用中のクライアント証明書を有効にしたまま、新しいクライアント証明書を発行する方法を説明します。

1. 「{{%slash%}}共通管理」画面で、「クライアント証明書」の[発行とダウンロード]をクリックします。
  {{< screen src="/general/img-ja/client_update_img01.png"  alt="[発行とダウンロード]が赤枠で囲まれた画像">}}
1. 目的のユーザーが所属する組織を選択します。  
  目的のユーザーが組織に属していない場合、[未所属のユーザー]または[すべてのユーザー]を選択します。
  {{< screen src="/general/img-ja/client_update_img02.png"  alt="特定の組織を選択している画像">}}
1. 「有効な証明書」を選択します。
  {{< screen src="/general/img-ja/client_update_img03.png"  alt="有効な証明書を選択している画像">}}
1. 目的のユーザーのチェックボックスを選択します。ユーザーは複数選択できます。
  {{< screen src="/general/img-ja/client_update_img04.png"  alt="特定のユーザーを選択している画像">}}
1. クライアント証明書の有効期限を設定します。
  {{< screen src="/general/img-ja/client_update_img05.png"  alt="有効期限を設定している画像">}}
1. 「発行済みのクライアント証明書を無効にして再発行する」の選択を外します。
  {{< screen src="/general/img-ja/client_update_img06.png"  alt="チェックボックスの選択を外している画像">}}
1. [発行]をクリックします。
  {{< screen src="/general/img-ja/client_update_img07.png"  alt="[発行]が赤枠で囲まれた画像">}}
1. ユーザーの端末にクライアント証明書をインストールします。  
  クライアント証明書をインストールする手順は、[端末にクライアント証明書をインストールする](/general/ja/admin/list_security/list_secureaccess/secureaccess.html#list_secureaccess_secureaccess_40)方法を参照してください。  
