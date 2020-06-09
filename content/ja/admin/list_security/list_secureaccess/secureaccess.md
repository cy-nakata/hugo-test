---
title: "セキュアアクセスを設定する"
weight: 150
---
{{% enabled US %}}
{{% warning %}}
セキュアアクセスは、[AWSに移行](https://www.kintone.com/aws-migration/)したお客様（[ドメインID](/general/ja/admin/list_old/domainid.html)が「y」で始まるお客様）にはご利用いただけません。
{{% /warning %}}
{{% /enabled %}}

{{% enabled JP US %}}
IPアドレス制限を設定する場合、社外など未登録のIPアドレスから{{%service%}}にアクセスするには、Basic認証、またはセキュアアクセスの設定が必要です。  
{{% /enabled %}}
{{% enabled CN %}}
IPアドレス制限を設定する場合、社外など未登録のIPアドレスから{{%service%}}にアクセスするには、セキュアアクセスの設定が必要です。  
{{% /enabled %}}

セキュアアクセスは有料オプションです。詳細は、[セキュアアクセスとは](/general/ja/admin/list_security/list_access/secureaccess.html)を参照してください。  
 
ここではセキュアアクセスの設定方法を説明します。

{{% warning %}}
必ずSTEP5の「[IPアドレス制限を設定する](#list_secureaccess_secureaccess_50)」まで行ってください。  
IPアドレス制限を設定するまでは、社外からの{{%service%}}へのアクセスを制限できません。
{{% /warning %}}

## STEP1：セキュアアクセスの利用を開始する{#list_secureaccess_secureaccess_10}

{{% enabled JP US %}}
[{{%store%}}](https://store.{{%cybozu_com%}}/manage/)で、セキュアアクセスの利用を開始します。1か月間は無料でお試しできます。
{{% /enabled %}}

{{% enabled CN %}}
セキュアアクセスの利用については、{{%CorpName%}}もしくは販売店にお問い合わせください。
{{% /enabled %}}

## STEP2：ユーザーにセキュアアクセスの利用を許可する{#list_secureaccess_secureaccess_20}

対象のユーザーに、セキュアアクセスの利用を許可します。  
次のどちらかの方法で設定できます。

### 方法1 ユーザーごとにセキュアアクセスの利用を許可する{#list_secureaccess_secureaccess_2010}

1. 「{{%slash%}}共通管理」画面の「ユーザー管理」の、[組織/ユーザー]をクリックします。  
  {{< screen src="/general/img-ja/allow_secure_img01.png" alt="[組織/ユーザー]が赤枠で囲まれた画像">}}
1. 組織を選択し、セキュアアクセスを利用するユーザーの![アイコン](/general/img/slash_edit_icon.png)をクリックします。  
  目的のユーザーが組織に属していない場合、[未所属のユーザー]を選択します。  
  {{< screen src="/general/img-ja/allow_secure_img02.png" alt="組織とユーザーを選択している画像">}}
1. 「ユーザー情報の編集」画面で、利用するサービスの「セキュアアクセス」のチェックボックスを選択します。
  {{< screen src="/general/img-ja/allow_secure_img03.png" alt="「セキュアアクセス」を選択している画像">}}
1. [保存]をクリックします。
  {{< screen src="/general/img-ja/allow_secure_img04.png" alt="[保存]が赤枠で囲まれた画像">}}

### 方法2 複数のユーザーに一括でセキュアアクセスの利用を許可する{#list_secureaccess_secureaccess_2020}

1. 「{{%slash%}}共通管理」画面の「ユーザー管理」の、[サービスの利用ユーザー]をクリックします。  
  {{< screen src="/general/img-ja/allow_secure_img05.png" alt="[サービスの利用ユーザー]が赤枠で囲まれた画像">}}
1. ドロップダウンリストから「セキュアアクセス」を選択します。  
  {{< screen src="/general/img-ja/allow_secure_img06.png" alt="「セキュアアクセス」を選択している画像">}}
1. 組織を選択し、ユーザーを選択します。ユーザーは複数選択できます。  
  目的のユーザーが組織に属していない場合、[未所属のユーザー]を選択します。  
  {{< screen src="/general/img-ja/allow_secure_img07.png" alt="組織とユーザーを選択する画像">}}
1. [追加>]をクリックして、「「セキュアアクセス」の利用ユーザー」にユーザーを追加します。
  {{< screen src="/general/img-ja/allow_secure_img08.png" alt="セキュアアクセスを利用するユーザーに追加する画像">}}
1. [保存]をクリックします。  
  {{< screen src="/general/img-ja/allow_secure_img09.png" alt="[保存]が赤枠で囲まれた画像">}}

## STEP3：クライアント証明書を発行する{#list_secureaccess_secureaccess_30}

セキュアアクセスを使用するユーザーごとに、クライアント証明書を発行します。

1. 「{{%slash%}}共通管理」画面で、「クライアント証明書」の[発行とダウンロード]をクリックします。  
  {{< screen src="/general/img-ja/issue_client_img01.png" alt="[発行とダウンロード]が赤枠で囲まれた画像">}}
1. 目的のユーザーが所属する組織と、ユーザーのクライアント証明書の状態を選択します。

    * 目的のユーザーが組織に属していない場合、[未所属のユーザー]または[すべてのユーザー]を選択します。
    * クライアント証明書の状態は、次の中から選択します。
        * 未発行：ユーザーに初めてクライアント証明書を発行する場合
        * 有効な証明書：ユーザーのクライアント証明書が有効期限内の場合
        * 期限切れの証明書：ユーザーのクライアント証明書が有効期限を過ぎている場合
  {{< screen src="/general/img-ja/issue_client_img02.png" alt="組織とクライアント証明書の状態を選択する画像">}}
1. 目的のユーザーのチェックボックスを選択します。  
  ユーザーは複数選択できます。  
  {{< screen src="/general/img-ja/issue_client_img03.png" alt="特定のユーザーを選択している画像">}}
1. 必要に応じて有効期限を変更します。  
  初期値は1年後に設定されています。  
  日付は1900-01-01から9999-12-30の範囲で指定してください。  
  {{< screen src="/general/img-ja/issue_client_img04.png" alt="有効期限を変更している画像">}}
  {{< note >}}

  * 有効期限には、クライアント証明書を発行する管理者のタイムゾーンが反映されます。  
    たとえば、管理者のタイムゾーンが「（UTC+09:00）大阪、札幌、東京」で、ユーザーのタイムゾーンが「（UTC-10:00）ハワイ」だとします。  
    この場合、有効期限が「2014年8月1日」のクライアント証明書を発行すると、クライアント証明書は、日本時間の2014年8月2日の0時00分（ハワイ時間の2014年8月1日の5時00分）に無効になります。  
  {{< screen src="/general/img-ja/issue_client_01.png" alt="タイムゾーンの例">}}
  {{< /note >}}

1. 発行済みのクライアント証明書がある場合、無効にするかどうかを選択します。  
  ユーザーに対して過去に発行したクライアント証明書を破棄し、新しい証明書を発行するには、「発行済みのクライアント証明書を無効にして再発行する」を選択します。  
  発行済みのクライアント証明書を有効にしたまま、新しい証明書を発行するには、選択を外します。
  {{< screen src="/general/img-ja/issue_client_img05.png" alt="無効にするかどうかを選択している画像">}}
1. [発行]をクリックします。

{{% note %}}
  
* クライアント証明書の有効期限が切れたユーザーは、セキュアアクセスを利用してサービスにアクセスできなくなります。  
  ユーザーが継続してサービスを利用するには、新しいクライアント証明書を発行し、使用する端末に再登録する必要があります。  
* 発行済みのクライアント証明書の有効期限は変更できません。  
  有効期限は、「有効な証明書」を選択すると確認できます。
* Internet ExplorerおよびiPhoneのSafariの場合、クライアント証明書の有効期限が切れても、セッションキャッシュの有効期限が切れるまでの最長10分間はアクセスできる場合があります。

{{% /note %}}

## STEP4：端末にクライアント証明書をインストールする{#list_secureaccess_secureaccess_40}

クライアント証明書のインストールには、次の2通りの方法があります。

### 方法1 ユーザー本人にインストールしてもらう{#list_secureaccess_secureaccess_4010}

初期状態では、ユーザーによるクライアント証明書のダウンロードは許可されています。  
クライアント証明書をインストールする方法は、次のページを参照してください。  
[オフィス外からサービスにアクセスする](/general/ja/user/list_access/remote.html)  
クライアント証明書をインストールしたら、セキュアアクセスの設定は完了です。

### 方法2 管理者がインストールする{#list_secureaccess_secureaccess_4020}

管理者が端末にクライアント証明書をインストールする場合、次の3つの設定を行います。

* [ユーザーによるクライアント証明書のダウンロードを禁止する](#list_secureaccess_secureaccess_402010)
* [各ユーザーのクライアント証明書をまとめてダウンロードする](#list_secureaccess_secureaccess_402020)
* [クライアント証明書をインストールする](#list_secureaccess_secureaccess_402030)

#### ユーザーによるクライアント証明書のダウンロードを禁止する{#list_secureaccess_secureaccess_402010}

1. 「{{%slash%}}共通管理」画面の「クライアント証明書」の、[ダウンロードの許可]をクリックします。  
  {{< screen src="/general/img-ja/prohibit_dl_ja_01.png" alt="[ダウンロードの許可]が赤枠で囲まれた画像">}}
1. チェックボックスの選択を外します。  
  {{< screen src="/general/img-ja/secureaccess_10.png" alt="チェックボックスの選択を外している画像">}}

#### 各ユーザーのクライアント証明書をまとめてダウンロードする{#list_secureaccess_secureaccess_402020}

1. 「{{%slash%}}共通管理」画面で、「クライアント証明書」の[発行とダウンロード]をクリックします。  
  {{< screen src="/general/img-ja/dl_certificate_img01.png" alt="[発行とダウンロード]が赤枠で囲まれた画像">}}
1. 目的のユーザーが所属する組織を選択します。  
  目的のユーザーが組織に属していない場合、[未所属のユーザー]または[すべてのユーザー]を選択します。  
  {{< screen src="/general/img-ja/dl_certificate_img02.png" alt="特定の組織を選択している画像">}}
1. 「有効な証明書」を選択します。  
  {{< screen src="/general/img-ja/dl_certificate_img03.png" alt="有効な証明書を選択している画像">}}
1. 目的のユーザーのチェックボックスを選択します。  
  {{< screen src="/general/img-ja/dl_certificate_img04.png" alt="特定のユーザーを選択している画像">}}
1. [ダウンロード]をクリックします。  
  ダウンロードファイルには、ユーザーごとにクライアント証明書とパスワードをまとめたzipファイルが含まれます。  
  {{< screen src="/general/img-ja/dl_certificate_img05.png" alt="[ダウンロード]が赤枠で囲まれた画像">}}

#### クライアント証明書をインストールする{#list_secureaccess_secureaccess_402030}

クライアント証明書をインストールする方法は、次のページを参照してください。  
[クライアント証明書の登録方法](/ja/settings/browser/certificate.html)  
クライアント証明書をインストールしたら、セキュアアクセスの設定は完了です。

## STEP5：IPアドレス制限を設定する{#list_secureaccess_secureaccess_50}

{{% enabled JP US %}}
{{%store%}}、または{{%slash%}}共通管理でIPアドレス制限の設定をします。  
詳細は、[IPアドレス制限とは](/general/ja/admin/list_security/list_access/ip_restrictions.html)を参照してください。  

{{% /enabled %}}

{{% enabled CN %}}
IPアドレス制限の利用については、{{%CorpName%}}もしくは販売店にお問い合わせください。
{{% /enabled %}}
