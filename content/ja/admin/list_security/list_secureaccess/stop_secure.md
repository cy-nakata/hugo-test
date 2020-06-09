---
title: "セキュアアクセスが不要になったとき（セキュアアクセスの利用を無効にする）"
weight: 200
---
{{% enabled US %}}
{{% warning %}}
セキュアアクセスは、[AWSに移行](https://www.kintone.com/aws-migration/)したお客様（[ドメインID](/general/ja/admin/list_old/domainid.html)が「y」で始まるお客様）にはご利用いただけません。
{{% /warning %}}
{{% /enabled %}}

セキュアアクセスの利用が不要になったユーザーは、セキュアアクセスの利用を無効にしてください。セキュアアクセスの利用を一度無効にすると、使用していたクライアント証明書は無効になります。利用を再開するには、クライアント証明書を再発行し、インストールする必要があります。

{{% enabled JP US %}}

1. ユーザーが利用するサービスから「セキュアアクセス」を外します。  
  [ユーザーが利用するサービスを設定する](/general/ja/admin/list_uma/list_userdptmnt/uma_list_user/service_user.html)  
  ユーザーの画面に「モバイルからのアクセス」が表示されなくなります。
{{< screen src="/general/img-ja/stop_secure_img01.png" alt="ユーザー情報の編集画面">}}
{{% /enabled %}}

{{% enabled CN %}}

1. ユーザーが利用するサービスから「セキュアアクセス」を外します。  
  [ユーザーが利用するサービスを設定する](/general/ja/admin/list_uma/list_userdptmnt/uma_list_user/service_user.html)  
  ユーザーには、「外部からのアクセス」画面が表示されなくなります。  
{{< screen src="/general/img-ja/stop_secure_img01.png" alt="ユーザー情報の編集画面">}}
{{% /enabled %}}

{{% note %}}
ユーザーの退職や休職により、サービスへのアクセス自体を禁止する場合は、必要に応じて次の設定も確認してください。  
[ユーザーを使用停止にする](/general/ja/admin/list_useradmin/list_user/stop_user.html)  
[ユーザーを削除する](/general/ja/admin/list_useradmin/list_user/delete_user.html)  
{{% /note %}}
