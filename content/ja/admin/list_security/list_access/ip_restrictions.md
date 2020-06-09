---
title: "IPアドレス制限とは"
weight: 400
disabled: [CN]
---

{{% enabled US %}}
{{% warning %}}
この記事は、[AWSに移行](https://www.kintone.com/aws-migration/)したお客様向けです。ドメインIDが「y」で始まるお客様が該当します。AWSへの移行が未完了のお客様は、[IPアドレス制限を設定する（AWSへの移行が未完了のお客様向け）](/general/ja/admin/list_old/ip_basic_old.html)をお読みください。  

ドメインIDを確認するには「[ドメインIDの確認方法](/general/ja/admin/list_old/domainid.html)」を参照してください。
{{% /warning %}}
{{% /enabled %}}

IPアドレス制限とは、接続元のIPアドレスを使ってアクセスを制限する機能です。  
たとえば、{{%service%}}へのアクセスを自社オフィスのIPアドレスだけに許可し、それ以外からのアクセスを遮断する、といった設定ができます。  
利用できる場所を限定し、社外からのアクセスを遮断できるため、第三者による不正アクセスを効果的に防げます。  

{{% enabled JP %}}
{{< screen src="/general/img-ja/list_access_overview_img01_jp.png"  alt="IPアドレス制限のイメージ">}}
{{% /enabled %}}
{{% enabled US %}}
{{< screen src="/general/img-ja/list_access_overview_img01_us.png"  alt="IPアドレス制限のイメージ">}}
{{% /enabled %}}

## IPアドレス制限を設定できるユーザー {#list_access_ip_restrictions_10}

{{% enabled JP %}}

* {{%store%}}の管理者
* アクセス制限を設定する権限が付与された、{{%slash%}}共通管理者

{{% /enabled %}}

{{% enabled US %}}

* {{%slash%}}共通管理者

{{% /enabled %}}

管理者の詳細は、[管理者の種類](/general/ja/admin/list_administrator/list_type_of_administrator/administrator.html)を参照してください。

## 設定方法 {#list_access_ip_restrictions_20}

IPアドレス制限の設定では、許可するネットワークを「グローバルIPアドレス」で指定します。  
お使いのネットワークのグローバルIPアドレスは、ネットワークの管理者やプロバイダーに確認してください。グローバルIPアドレスは、複数指定できます。  
IPアドレス制限の設定方法は下記のとおりです。  

{{% enabled JP %}}

### {{%store%}}の管理者が設定する場合 {#list_access_ip_restrictions_2010}

1. [{{%store%}}](https://store.{{%cybozu_com%}}/login)にアクセスします。  

1. {{%store%}}の管理者のメールアドレス、パスワードを入力してログインします。
  {{< screen src="/general/img-ja/list_access_ip_restrictions_img01.png"  alt="ログイン画面">}}
  ログイン情報を忘れてしまった場合は、[{{%store%}}にログインできません。](/general/ja/login/store_account.html)を参照してください。

1. [ドメイン管理]をクリックします。

1. 「セキュリティと認証」タブをクリックします。  
  複数のドメインを所有している場合は、設定するドメインをドロップダウンリストから選択します。
  {{< screen src="/general/img-ja/list_access_ip_restrictions_img02.png"  alt="ドメイン管理の画面">}}

1. 「IPアドレス制限」欄の[変更]をクリックします。  
  {{< screen src="/general/img-ja/list_access_ip_restrictions_img03.png"  alt="ドメイン管理の画面">}}

1. 設定する内容に応じて、「すべて拒否」または「一部許可」を選択します。  
  設定内容は、あとから追加や編集ができます。
  {{< screen src="/general/img-ja/list_access_ip_restrictions_img04.png"  alt="ドメイン管理の画面">}}
    * **「一部許可」を選択する場合：**  
      * 「IPアドレス」欄：  
        アクセスを許可するネットワークのグローバルIPアドレスを登録します。IPアドレスは、2,900個まで登録できます。  
        IPv4アドレスにのみ対応しています。IPv6アドレスには対応していません。  
      * 「CIDR」欄：  
        複数のIPアドレスを範囲指定する場合にだけ入力します。  
    * **大量のIPアドレスを登録する場合：**  
      CSVファイルを使用してIPアドレスを一括で登録できます。
      詳細は、[IPアドレスを読み込むCSVファイルのフォーマット](/general/ja/admin/list_security/list_access/ip_restrictions.html#list_access_ip_restrictions_2030)を参照してください。

1. 入力した内容を確認し、[保存]をクリックします。  
  設定が完了すると、{{%store%}}の管理者のメールアドレス宛にメールが送信されます。  

{{% /enabled %}}

### {{%slash%}}共通管理者が設定する場合 {#list_access_ip_restrictions_2020}

{{% enabled JP %}}

1. {{%slash%}}共通管理画面にアクセスします。

1. 「セキュリティ」の[アクセス制限]をクリックします。
  {{< screen src="/general/img-ja/list_access_ip_restrictions_img05.png"  alt="[アクセス制限]が赤枠で囲まれた画像">}}

1. [{{%store%}}へ]をクリックします。  
  {{< screen src="/general/img-ja/list_access_ip_restrictions_img06.png"  alt="アクセス制限の設定画面">}}

1. これ以降の手順は、[{{%store%}}の管理者が設定する場合](#list_access_ip_restrictions_2010)と同じです。

{{% /enabled %}}

{{% enabled US %}}

1. {{%slash%}}共通管理画面にアクセスします。

1. 「セキュリティ」の[アクセス制限]をクリックします。  
  デフォルトでは「すべて許可」が選択されています。  
  {{< screen src="/general/img-ja/list_access_ip_restrictions_img05.png"  alt="[アクセス制限]が赤枠で囲まれた画像">}}

1. 「一部許可」をクリックします。  
  {{< screen src="/general/img-ja/list_access_ip_restrictions_img05_us.png"  alt="アクセス制限の設定画面">}}
  **「一部許可」を選択する場合：**  
    * 「IPアドレス」欄：  
      アクセスを許可するネットワークのグローバルIPアドレスを登録します。IPアドレスは、2,900個まで登録できます。  
      IPv4アドレスにのみ対応しています。IPv6アドレスには対応していません。  
    * 「CIDR」欄：  
      複数のIPアドレスを範囲指定する場合にだけ入力します。  

1. [保存]をクリックします。  
  設定が反映されるまでしばらく時間がかかることがあります。  
  設定が完了すると、管理者のメールアドレス宛にメールが送信されます。

{{% /enabled %}}

{{% enabled JP %}}

### IPアドレスを読み込むCSVファイルのフォーマット {#list_access_ip_restrictions_2030}

IPアドレスの登録に使用するCSVファイルには、1行目に項目名を、2行目以降に項目の値を記載します。  

<table>
    <caption>記載例：</caption>
    <thead>
        <tr>
            <td>IPアドレス</td>
            <td>CIDR</td>
            <td>メモ</td>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>61.202.247.1</td>
            <td>&nbsp;</td>
            <td>東京オフィス</td>
        </tr>
        <tr>
            <td>61.202.247.2</td>
            <td>&nbsp;</td>
            <td>大阪オフィス</td>
        </tr>
        <tr>
            <td>61.202.247.5</td>
            <td>&nbsp;</td>
            <td>札幌オフィス</td>
        </tr>
        <tr>
            <td>24.4.25.121</td>
            <td>&nbsp;</td>
            <td>サンフランシスコオフィス</td>
        </tr>
    </tbody>
</table>

[example.csv](/general/files-ja/example.csv)から、CSVファイルのサンプルをダウンロードできます。

{{% /enabled %}}

{{% enabled US %}}

### 設定を失敗し、アクセスできなくなった場合 {#list_access_ip_restrictions_2040}

IPアドレス制限の設定を失敗し、{{%service%}}にアクセスできなくなった場合は、下記のどちらかをお試しください。

* 設定完了時に送られてたメールに記載されている「リセットURL」をクリックする。  
  リセットURLの有効期限は発行後1時間です。  
* [Contact Us](https://www.kintone.com/support/)から問い合わせる。

{{% /enabled %}}

## 出張やリモートワークに必要な設定 {#list_access_ip_restrictions_30}

{{% enabled US %}}

IPアドレス制限を設定すると、指定したIPアドレスだけに{{%service%}}へのアクセスを許可し、そのほかのIPアドレスを遮断できます。  
しかし、4G回線などのモバイルネットワークではグローバルIPアドレスを指定できません。  
このため、IPアドレス制限を設定した状態で、出張やリモートワークの際にモバイル端末から、4G回線などのモバイルネットワークを利用すると、{{%service%}}にアクセスできなくなります。  

出張やリモートワークで使う端末を考慮し、お客様の運用にあった設定をしてください。  
<br>

* **出張やリモートワークで、タブレットやスマートフォンを使う場合：**  
  2要素認証の利用をおすすめします。2要素認証を利用する場合、IPアドレス制限は「すべて許可」を選択する必要があります。  
  1人でも2要素認証を使うメンバーがいる場合は、下記の設定をします。
    1. IPアドレス制限を、「すべて許可」に設定します。  
    1. ユーザーに、各自で2要素認証を有効にする旨をアナウンスします。  
      詳細は、[2要素認証を設定する](/general/ja/user/list_personal/two_factor_authentication.html)を参照してください。

* **出張やリモートワークでモバイル端末を使わず、パソコンからアクセスする場合：**  
  IPアドレス制限をおすすめします。  
    1. IPアドレス制限を、「一部許可」に設定します。  
    1. 許可するネットワークに、メンバーが利用するネットワークを追加します。  
    1. 出張やリモートワークをするメンバーに、次の内容をアナウンスします。
        * モバイルネットワークではアクセスできない
        * パソコンからアクセスする必要がある

{{% /enabled %}}

{{% enabled JP %}}

出張やリモートワークなど、許可したIPアドレス以外の場所からのアクセスが考えられる場合は、IPアドレス制限に加えて、Basic認証、または、セキュアアクセスのどちらかを設定します。  
詳細は次のページを参照してください。  

* [Basic認証とは](/general/ja/admin/list_security/list_access/basic_auth.html)
* [セキュアアクセスとは](/general/ja/admin/list_security/list_access/secureaccess.html)

### 「IPアドレス制限」と「Basic認証」の組み合わせ {#list_access_ip_restrictions_3010}

IPアドレス制限とBasic認証の組み合わせによって、アクセス制限の対象が変わります。  
おすすめの組み合わせは、次のいずれかのパターンです。  

* パターン4
* パターン5
* パターン6

<table>
<caption>IPアドレス制限とBasic認証の組み合わせ</caption>
  <tbody>
  <tr>
  <th width=80></th>
  <th width=150>IPアドレス制限</th>
  <th width=100>Basic認証</th>
  <th>結果</th>
  </tr>
  <tr>
  <th>パターン1</th>
  <td>すべて許可</td>
  <td>設定なし</td>
  <td>すべてのIPアドレスからアクセス可能になります。<br>
      セキュリティが低下します。</td>
  </tr>
  <tr>
  <th>パターン2</th>
  <td>すべて許可</td>
  <td>設定あり</td>
  <td>この組み合わせは設定不可です。<br>
      Basic認証は、IPアドレス制限を設定している場合にのみ設定できます。</td>
  </tr>
  <tr>
  <th>パターン3</th>
  <td>すべて拒否</td>
  <td>設定なし</td>
  <td>すべてのアクセスが不可になります。</td>
  </tr>
  <tr>
  <th>パターン4</th>
  <td>すべて拒否</td>
  <td>設定あり</td>
  <td>認証ダイアログが表示されます。<br>
      認証情報を知っているユーザーのみアクセスできます。</td>
  </tr>
  <tr>
  <th>パターン5</th>
  <td> 一部許可</td>
  <td>設定なし</td>
  <td>たとえば「192.0.2.0」を許可した場合、そのIPアドレスを持つネットワークからのみアクセスできます。</td>
  </tr>
  <tr>
  <th>パターン6</th>
  <td> 一部許可</td>
  <td>設定あり</td>
  <td>
  <ul>
  <li><b>「192.0.2.0」を許可した場合：</b><br>
      そのIPアドレスを持つネットワークからのみアクセスできます。</li>
  <li><b>他のIPアドレスからアクセスする場合：</b><br>
      認証ダイアログが表示されます。<br>
      認証情報を知っているユーザーのみアクセスできます。</li>
  </ul>
  </td>
  </tr>
  </tbody>
</table>

### モバイルネットワーク（4G回線など）利用時に必要な設定 {#list_access_ip_restrictions_3020}

IPアドレス制限を設定すると、指定したIPアドレスだけに{{%service%}}へのアクセスを許可し、そのほかのIPアドレスを遮断できます。  
しかし、4G回線などのモバイルネットワークではグローバルIPアドレスを指定できません。  
このため、IPアドレス制限を設定した状態で、出張やリモートワークの際にモバイル端末から、4G回線などのモバイルネットワークを利用すると、{{%service%}}にアクセスできなくなります。  

モバイルネットワークからアクセスする場合は、IPアドレス制限に加えて、Basic認証、または、セキュアアクセスのどちらかを設定します。  
詳細は次のページを参照してください。  

* [Basic認証とは](/general/ja/admin/list_security/list_access/basic_auth.html)
* [セキュアアクセスとは](/general/ja/admin/list_security/list_access/secureaccess.html)

管理者側の設定が完了次第、社外でモバイル端末を利用するメンバーに、次のどちらかの情報をアナウンスしてください。  

* Basic認証の情報
* セキュアアクセスの利用方法

{{% /enabled %}}

## さらにセキュリティを高めるには {#list_access_ip_restrictions_40}

パスワードの制限を強化すると、お使いのサービスのセキュリティをより高められます。  
許可したネットワーク以外の場所からのアクセスがある場合は、必ず設定しましょう。  
詳細は、[パスワードの複雑さや有効期間を設定する](/general/ja/admin/list_security/list_login/pw_policy.html)を参照してください。  
