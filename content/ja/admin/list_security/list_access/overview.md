---
title: "アクセス制限に関するセキュリティの概要"
weight: 100
---

{{% enabled US %}}
{{% warning %}}
この記事は、[AWSに移行](https://www.kintone.com/aws-migration/)したお客様向けです。ドメインIDが「y」で始まるお客様が該当します。AWSへの移行が未完了のお客様は、[セキュリティ設定の概要（AWSへの移行が未完了のお客様向け）](/general/ja/admin/list_old/security_tutorial_old.html)をお読みください。  

ドメインIDを確認するには「[ドメインIDの確認方法](/general/ja/admin/list_old/domainid.html)」を参照してください。
{{% /warning %}}
{{% /enabled %}}

{{%service%}}に保存するデータを安全に管理するために、{{%cybozu_com%}}標準の認証に加えて、アクセス制限を設定することをおすすめします。  
{{% note %}}
{{%cybozu_com%}}標準の認証とは、{{%service%}}にログインする際に、{{%slash%}}共通管理に登録しているログイン名とパスワードを入力する認証方式を指します。
{{% /note %}}

アクセス制限のパターンは下記のとおりです。  

{{% disabled US CN %}}

## 手軽にセキュリティを強化したい {#list_access_overview_10}

ユーザーのログイン名とパスワードに加えて、Basic認証の情報を知っているユーザーだけがアクセスできるようにします。  

<table>
<caption>設定の組み合わせ</caption>
  <tbody>
  <tr>
  <th width=200>IPアドレス制限</th>
  <th width=200>Basic認証</th>
  </tr>
  <tr>
  <td>すべて拒否</td>
  <td>設定あり</td>
  </tr>
  </tbody>
</table>

{{< screen src="/general/img-ja/list_access_overview_img06.png"  alt="">}}
{{% /disabled %}}

{{% disabled US %}}

## 社内のみにアクセスを限定したい {#list_access_overview_20}

IPアドレス制限を使って、アクセスを社内ネットワークからのみに限定します。  

<table>
<caption>設定の組み合わせ</caption>
  <tbody>
  <tr>
  <th width=200>IPアドレス制限</th>
  <th width=200>Basic認証</th>
  </tr>
  <tr>
  <td>一部許可</td>
  <td>設定なし</td>
  </tr>
  </tbody>
</table>

{{< screen src="/general/img-ja/list_access_overview_img01_jp.png"  alt="">}}
{{% /disabled %}}

{{% enabled JP %}}

## 社外からのアクセスにのみBasic認証をかけたい {#list_access_overview_30}

IPアドレス制限で許可した場所からのアクセスはスムーズにしつつ、それ以外の場所からはBasic認証で不正なアクセスを防ぎます。

<table>
<caption>設定の組み合わせ</caption>
  <tbody>
  <tr>
  <th width=200>IPアドレス制限</th>
  <th width=200>Basic認証</th>
  </tr>
  <tr>
  <td>一部許可</td>
  <td>設定あり</td>
  </tr>
  </tbody>
</table>

{{< screen src="/general/img-ja/list_access_overview_img02.png"  alt="">}}
{{% /enabled %}}

{{% enabled US%}}

## 特定の場所からのアクセスのみ許可したい {#list_access_overview_60}

IPアドレス制限で許可した場所からのアクセスはスムーズにしつつ、それ以外の場所からのアクセスを防ぎます。  
この場合、2要素認証は利用しません。  

<table>
<caption>設定の組み合わせ</caption>
  <tbody>
  <tr>
  <th width=200>IPアドレス制限</th>
    <th width=200>2要素認証</th>
  </tr>
  <tr>
  <td>一部許可</td>
  <td>設定なし</td>
  </tr>
  </tbody>
</table>

{{< screen src="/general/img-ja/list_access_overview_img01_us.png"  alt="">}}
{{% /enabled %}}

{{% disabled US %}}

## 利用できる端末を限定したい {#list_access_overview_40}

IPアドレス制限で許可した場所からのアクセスはスムーズにしつつ、それ以外の場所からはセキュアアクセスの利用ユーザーのみアクセスを許可します。  
セキュアアクセスは有料オプションです。

<table>
<caption>設定の組み合わせ</caption>
  <tbody>
  <tr>
  <th width=200>IPアドレス制限</th>
  <th width=200>セキュアアクセス</th>
  </tr>
  <tr>
  <td>一部許可</td>
  <td>ユーザー単位で許可</td>
  </tr>
  </tbody>
</table>

{{< screen src="/general/img-ja/list_access_overview_img03.png"  alt="">}}

{{% /disabled %}}

{{% disabled JP CN %}}

## 2要素認証でセキュリティを高めたい {#list_access_overview_50}

{{%service%}}にアクセスできる場所（IPアドレス）は限定されません。  
しかし、ユーザーだけが知っている情報と、ユーザーのモバイル端末で確認できるコードの両方の入力を求めることでセキュリティを高めます。  
確認コードは、{{%service%}}へのログイン毎に新しいコードに更新されます。

<table>
<caption>設定の組み合わせ</caption>
  <tbody>
  <tr>
  <th width=200>IPアドレス制限</th>
  <th width=200>2要素認証</th>
  </tr>
  <tr>
  <td>すべて許可</td>
  <td>ユーザー単位で許可</td>
  </tr>
  </tbody>
</table>

{{< screen src="/general/img-ja/list_access_overview_img04.png"  alt="">}}

{{% /disabled %}}
