---
title: "端末をなくしたとき（パスワードの変更と、クライアント証明書の無効化）"
weight: 300
---
{{% enabled US %}}
{{% warning %}}
セキュアアクセスは、[AWSに移行](https://www.kintone.com/aws-migration/)したお客様（[ドメインID](/general/ja/admin/list_old/domainid.html)が「y」で始まるお客様）にはご利用いただけません。
{{% /warning %}}
{{% /enabled %}}

ユーザーがクライアント証明書をインストールした端末をなくしたときは、次の手順でユーザーのパスワードの変更と、クライアント証明書の無効化を行ってください。  
なくした端末からセキュアアクセスを使用できなくなります。また、スマートフォンアプリからの通知も表示されなくなります。  

## STEP1：ユーザーのパスワードを変更する

「ユーザー情報の編集」画面で、ユーザーのパスワードを変更します。  
詳細な手順は、[ユーザー情報を編集する](/general/ja/admin/list_useradmin/list_user/edit_user.html)方法を参照してください。
{{< screen src="/general/img-ja/client_revoke_img08.png"  alt="ユーザー情報の編集画面">}}

## STEP2：クライアント証明書を無効にして再発行する

1. 「{{%slash%}}共通管理」画面で、「クライアント証明書」の[発行とダウンロード]をクリックします。
  {{< screen src="/general/img-ja/client_revoke_img01.png"  alt="[発行とダウンロード]が赤枠で囲まれた画像">}}
1. 目的のユーザーが所属する組織を選択します。  
  目的のユーザーが組織に属していない場合、[未所属のユーザー]または[すべてのユーザー]を選択します。
  {{< screen src="/general/img-ja/client_revoke_img02.png"  alt="特定の組織を選択している画像">}}
1. 「有効な証明書」を選択します。
  {{< screen src="/general/img-ja/client_revoke_img03.png"  alt="有効な証明書を選択している画像">}}
1. 目的のユーザーのチェックボックスを選択します。ユーザーは複数選択できます。
  {{< screen src="/general/img-ja/client_revoke_img04.png"  alt="特定のユーザーを選択している画像">}}
1. クライアント証明書の有効期限を設定します。
  {{< screen src="/general/img-ja/client_revoke_img05.png"  alt="クライアント証明書の有効期限を設定している画像">}}
1. 「発行済みのクライアント証明書を無効にして再発行する」を選択します。
  {{< screen src="/general/img-ja/client_revoke_img06.png"  alt="チェックボックスを選択している画像">}}
1. [発行]をクリックします。
  {{< screen src="/general/img-ja/client_revoke_img07.png"  alt="[発行]が赤枠で囲まれた画像">}}
