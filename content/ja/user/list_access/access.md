---
title: "管理者にセキュリティの設定を確認する"
weight: 100
---
{{% enabled US %}}
{{% warning %}}
この記事は、[AWSへの移行](https://www.kintone.com/aws-migration/)が完了していないお客様向けです。ドメインIDが「c」で始まるお客様が該当します。ドメインIDを確認するには「[ドメインIDの確認方法](/general/ja/admin/list_old/domainid.html)」を参照してください。
{{% /warning %}}
{{% /enabled %}}

システム管理者の設定よっては、オフィス外から{{%service%}}のサービスへのアクセスに、セキュアアクセスの使用またはBasic認証が必要な場合があります。  
次の3つのセキュリティ設定のいずれに該当するかを、システム管理者に確認してください。

## セキュアアクセスを利用している場合{#list_access_access_10}

セキュアアクセスを利用している場合は、クライアント証明書の登録が必要です。

Webブラウザーからアクセスする際の設定手順は、[セキュアアクセスを利用している場合](/general/ja/user/list_access/remote/webbrowser.html#remote_webbrowser_10)を参照してください。  
スマートフォンアプリからアクセスする際の設定手順は、[スマートフォンアプリからサービスにアクセスする](/general/ja/user/list_access/remote/mobileapp.html#remote_webbrowser_20)方法を参照してください。  

## Basic認証を利用している場合{#list_access_access_20}

{{%slash%}}共通管理者にBasic認証のユーザー名とパスワードを確認する必要があります。  

Webブラウザーからアクセスする手順は、[セキュアアクセスを利用していない場合](/general/ja/user/list_access/remote/webbrowser.html#remote_webbrowser_20)を参照してください。  
スマートフォンアプリからアクセスする手順は、[スマートフォンアプリからサービスにアクセスする](/general/ja/user/list_access/remote/mobileapp.html)方法を参照してください。  

## セキュアアクセスとBasic認証のいずれも利用していない場合{#list_access_access_30}

オフィス外からでも、オフィス内と同様に{{%service%}}のサービスにアクセスできます。  

Webブラウザーからアクセスする場合は、「https://（サブドメイン名）.{{%cybozu_com%}}/」にアクセスしてログインします。  
スマートフォンアプリからアクセスする手順は、[スマートフォンアプリからサービスにアクセスする](/general/ja/user/list_access/remote/mobileapp.html)方法を参照してください。  
