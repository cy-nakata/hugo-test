---
title: "IPアドレス制限を設定する（AWSへの移行が未完了のお客様向け）"
weight: 300
disabled: [JP,CN]
---
{{% warning %}}
この記事は、[AWSへの移行](https://www.kintone.com/aws-migration/)が完了していないお客様向けです。ドメインIDが「c」で始まるお客様が該当します。ドメインIDを確認するには「[ドメインIDの確認方法](/general/ja/admin/list_old/domainid.html)」を参照してください。
{{% /warning %}}

IPアドレス制限を設定すると、{{%service%}}へのアクセスを自社のネットワークだけに許可し、社外からのアクセスを遮断できます。社外の第三者による{{%service%}}への不正なアクセスを防ぐため、IPアドレス制限を設定しておくことを推奨します。
{{% enabled JP %}}
{{< screen src="/general/img-ja/ip_basic_01.png"  alt="IPアドレス制限のイメージ">}}
{{% /enabled %}}
{{% enabled US %}}
{{< screen src="/general/img-ja/ip_basic_us_01.png"  alt="IPアドレス制限のイメージ">}}
{{% /enabled %}}

IPアドレス制限の設定では、{{%service%}}へのアクセスを許可するネットワークを、「グローバルIPアドレス」で指定します。お使いのネットワークのグローバルIPアドレスは、ネットワークの管理者やプロバイダーに確認してください。グローバルIPアドレスは、複数指定できます。

IPアドレス制限は、次の管理者が無料で設定できます。

* {{%store%}}の管理者
* アクセス制限を設定する権限が付与された{{%slash%}}共通管理者

管理者の詳細は[管理者の種類](/general/ja/admin/list_administrator/list_type_of_administrator/administrator.html)を参照してください。  

{{% note %}}
IPアドレス制限を設定した場合、社外から{{%service%}}にアクセスするには、Basic認証、またはセキュアアクセスのいずれかを設定します。  
[Basic認証とは](/general/ja/admin/list_security/list_access/basic_auth.html)  
[セキュアアクセスとは](/general/ja/admin/list_security/list_access/secureaccess.html)
{{% /note %}}

## 設定手順 {#list_old_ip_basic_old_10}

IPアドレス制限は、{{%store%}}、または{{%slash%}}共通管理で設定できます。

### {{%store%}}で設定する場合 {#list_old_ip_basic_old_1010}

{{% enabled JP %}}

1. [{{%store%}}](https://store.{{%cybozu_com%}}/manage/)にアクセスし、{{%store%}}の管理者のメールアドレス、パスワードを入力してログインします。
  {{< screen src="/general/img-ja/ip_basic_img02.png"  alt="ログイン画面">}}
1. [ドメイン管理]をクリックし、「セキュリティと認証」タブをクリックします。  
  複数のドメインを所有している場合は、設定するドメインをドロップダウンリストから選択します。
  {{< screen src="/general/img-ja/ip_basic_img03.png"  alt="ドメイン管理画面">}}
1. 「IPアドレス制限」の[変更]をクリックし、設定する内容に応じて「すべて拒否」または「一部許可」を選択します。  
  「一部許可」を選択した場合は、アクセスを許可するネットワークのグローバルIPアドレスを、すべて登録します。IPアドレスは、2,900個まで登録できます。「CIDR」は、複数のIPアドレスを範囲指定する場合だけ入力します。IPアドレスは、あとから追加や編集ができます。  
  大量のIPアドレスを登録する場合は、CSVファイルを使用してIPアドレスを一括で登録できます。  
  CSVファイルの記載方法は、[IPアドレスを読み込むCSVファイルのフォーマット](/general/ja/admin/list_old/ip_basic_old.html#list_old_ip_basic_old_1030)を参照してください。  
  {{< screen src="/general/img-ja/ip_basic_img04.png"  alt="IPアドレス制限を設定する画面">}}
1. [保存]をクリックします。  
   設定が完了すると、{{%store%}}の管理者のメールアドレス宛にメールが送信されます。

{{% /enabled %}}

{{% enabled US %}}

1. [{{%store%}}](https://store.{{%cybozu_com%}}/)にアクセスし、{{%store%}}の管理者のメールアドレス、パスワードを入力してログインします。
  {{< screen src="/general/img-ja/storelogin330_us_01.png"  alt="画像">}}
1. [Domains]をクリックし、「Security & Authentication」タブをクリックします。  
  複数のドメインを所有している場合は、設定するドメインをドロップダウンリストから選択します。
  {{< screen src="/general/img-ja/storedomainsecu_us_ja_01.png"  alt="画像">}}
1. IPアドレス制限欄の[Change]をクリックし、設定する内容に応じて「Deny all」または「Allow specific IP addresses」を選択します。
  「Allow specific IP addresses」を選択した場合は、アクセスを許可するネットワークのグローバルIPアドレスを、すべて登録します。「CIDR」は、複数のIPアドレスを範囲指定する場合だけ入力します。IPアドレスは、あとから追加や編集ができます。  
  大量のIPアドレスを登録する場合は、CSVファイルを使用してIPアドレスを一括で登録できます。CSVファイルの記載方法は、[IPアドレスを読み込むCSVファイルのフォーマット](/general/ja/admin/list_old/ip_basic_old.html#list_old_ip_basic_old_1030)を参照してください。  
  {{< screen src="/general/img-ja/storedomainsecu_us_ja_02.png"  alt="画像">}}
1. [Save]をクリックします。  
  設定が完了すると、{{%store%}}の管理者のメールアドレス宛にメールが送信されます。

{{% /enabled %}}

### {{%slash%}}共通管理画面から設定する場合 {#list_old_ip_basic_old_1020}

{{% enabled JP %}}

アクセス制限の設定が許可されている場合、次の手順でIPアドレス制限を設定できます。

1. {{%slash%}}共通管理画面で、「セキュリティ」の[アクセス制限]をクリックします。
1. 「今すぐ設定する」をクリックします。
  {{< screen src="/general/img-ja/ip_basic_jp_ja_01.png"  alt="今すぐ設定するが赤枠で囲まれた画像">}}
1. IPアドレス制限欄の[変更]をクリックし、設定する内容に応じて「すべて拒否」または「一部許可」を選択します。  
  「一部許可」を選択した場合は、アクセスを許可するネットワークのグローバルIPアドレスを、すべて登録します。IPアドレスは、2,900個まで登録できます。「CIDR」は、複数のIPアドレスを範囲指定する場合だけ入力します。IPアドレスは、あとから追加や編集ができます。  
  大量のIPアドレスを登録する場合は、CSVファイルを使用してIPアドレスを一括で登録できます。CSVファイルの記載方法は、次の項目を参照してください。  
  [IPアドレスを読み込むCSVファイルのフォーマット](/general/ja/admin/list_old/ip_basic_old.html#list_old_ip_basic_old_1030)
  {{< screen src="/general/img-ja/ip_basic_jp_ja_02.png"  alt="アクセス制限の設定画面">}}
1. [保存]をクリックします。  
  設定が完了すると、{{%store%}}の管理者のメールアドレス宛にメールが送信されます。

{{% /enabled %}}

{{% enabled US %}}

アクセス制限の設定が許可されている場合、次の手順でIPアドレス制限を設定できます。

1. {{%slash%}}共通管理画面で、「システム管理」の[アクセス制限]をクリックします。
1. 「今すぐ設定する」をクリックします。
1. IP Address Restrictionsの[Change]をクリックし、設定する内容に応じて「Deny All」または「Allow specific IP addressess」を選択します。  
   「Allow specific IP addressess」を選択した場合は、アクセスを許可するネットワークのグローバルIPアドレスを、すべて登録します。「CIDR」は、複数のIPアドレスを範囲指定する場合だけ入力します。IPアドレスは、あとから追加や編集ができます。
1. [Save]をクリックします。  
   設定が完了すると、{{%store%}}の管理者のメールアドレス宛にメールが送信されます。

{{% /enabled %}}

### IPアドレスを読み込むCSVファイルのフォーマット {#list_old_ip_basic_old_1030}

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

次のリンクから、CSVファイルのサンプルをダウンロードできます。：  
[example.csv](/general/files-ja/example.csv)

### 参考：パスワードの制限を強化する {#list_old_ip_basic_old_1040}

IPアドレス制限とBasic認証に加え、パスワードの制限を強化すると、お使いのサービスのセキュリティをより高められます。パスワードの制限を強化する方法は、[パスワードの複雑さや有効期間を設定する](/general/ja/admin/list_security/list_login/pw_policy.html)を参照してください。  
