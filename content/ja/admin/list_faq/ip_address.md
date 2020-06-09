---
title: "{{%service%}}が使用するIPアドレスを教えてください。"
weight: 500
disabled: [JP]
---

メールサーバーなど、お客様が利用されているシステムにおいて、IPアドレスのセキュリティフィルターを設定している場合は、{{%service%}}が使用するIPアドレスをホワイトリストに追加してください。  
なお、サービス向上や災害対応などの理由により、本ページに記載されているIPアドレスは変更・追加される場合があります。  
{{%service%}}が使用するIPアドレスをホワイトリストに設定する場合は、定期的に本ページを参照し、IPアドレスの変更や追加がないか確認してください。  

{{% enabled US %}}
{{%service%}}で使用しているIPアドレスのCIDR記法は、次のとおりです。  

## [AWSへの移行](https://www.kintone.com/aws-migration/)が完了していないお客様

ドメインIDが「c」で始まるお客様が該当します。
ドメインIDを確認するには「[ドメインIDの確認方法](/general/ja/admin/list_old/domainid.html)」を参照してください。

* お客さまの端末から接続する{{%kintone%}}のIPアドレス（インバウンドIPアドレス）  
  動的に変更されます。
* {{%kintone%}}から外部へ接続するときに利用するIPアドレス（アウトバウンドIPアドレス）  
  103.79.14.0/24

## [AWSへの移行](https://www.kintone.com/aws-migration/)が完了したお客様

ドメインIDが「y」で始まるお客様が該当します。

* お客さまの端末から接続する{{%kintone%}}のIPアドレス（インバウンドIPアドレス）  
  動的に変更されます。
* {{%kintone%}}から外部へ接続するときに利用するIPアドレス（アウトバウンドIPアドレス）  
  52.32.46.167, 35.155.158.164

## IPアドレス一覧のダウンロード

{{%kintone%}}から外部へ接続するときに利用するIPアドレス（アウトバンドIPアドレス）の一覧をCIDR記法で記載したテキストファイルをダウンロードできます。  
ホワイトリストへのIPアドレスの追加などにご利用ください。  

* **[AWSへの移行](https://www.kintone.com/aws-migration/)が完了していないお客様**（[ドメインID](/general/ja/admin/list_old/domainid.html)が「c」で始まるお客様）  
 [slash_admin_ipaddlist.txt](/general/files-ja/slash_admin_ipaddlist.txt)
* **[AWSへの移行](https://www.kintone.com/aws-migration/)が完了したお客様**（[ドメインID](/general/ja/admin/list_old/domainid.html)が「y」で始まるお客様）  
 [slash_admin_ipaddlist_on_or_after0908.txt](/general/files-ja/slash_admin_ipaddlist_on_or_after0908.txt)

{{% /enabled %}}

{{% enabled CN %}}
{{%service%}}で使用しているIPアドレスのCIDR記法は、次のとおりです。  
211.144.213.64&#47;27

IPアドレス一覧をCIDR記法で記載したテキストファイルをダウンロードできます。  
ホワイトリストへのIPアドレスの追加などにご利用ください。  
[cybozucn_admin_ipaddlist.txt](/general/files-ja/cybozucn_admin_ipaddlist.txt)
{{% /enabled %}}
