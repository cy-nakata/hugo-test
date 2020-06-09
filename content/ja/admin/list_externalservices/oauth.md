---
title: "外部サービスとの連携を許可する（Microsoft Power AutomateやSlackなど）"
weight: 100
---
Microsoft Power AutomateやSlackなどの外部サービスと{{%kintone%}}との連携を、ユーザーに許可できます。  
認証にはOAuthを使用します。そのため、外部サービスや連携先のサービスに{{%kintone%}}のログイン名やパスワードを入力することなく、セキュアに連携できます。

{{%note%}}
Google Hangouts Chatとの連携は、現在使用できません。
{{%/note%}}

## Microsoft Power Automateとの連携でできること {#list_externalservices_oauth_10}

[Microsoft Power Automate](https://flow.microsoft.com/ja-jp/)は、{{%kintone%}}、SharePoint、Dropbox、Slack、メール、Excelなど多数のサービスをユーザーが好きな形で連携させることができるWebサービスです。  
Microsoft Power Automateを使うと、Microsoft Power Automateが対応する上記のサービスと{{%kintone%}}を連携できます。
{{%kintone%}}に登録されたデータを連携するサービスに反映することも、連携するサービスに登録されたデータを{{%kintone%}}に反映することも、どちらも可能です。

例：

* Outlookなどのメールクライアントでメールを受信したら、{{%kintone%}}に通知する
* {{%kintone%}}のアプリにレコードが登録されたら、Google Calendarに予定として登録する

### Microsoft Power Automateと連携する場合の注意点 {#list_externalservices_oauth_1010}

お使いのドメインでIPアドレス制限が有効な場合、そのままでは連携サービスを利用できません。  
作業する前に、Microsoft Power Automate、Office 365とMicrosoft Azureが使うIPアドレスからのアクセスを許可しておく必要があります。許可するIPアドレスは、Microsoft社の次のページを参照してください。  

* Microsoft社の資料：  
  * [Microsoft Power Automateでの制限事項と構成](https://docs.microsoft.com/ja-jp/flow/limits-and-config#ip-address-configuration)  
  * [Office 365 URL および IP アドレス範囲](https://support.office.com/ja-jp/article/office-365-url-%E3%81%8A%E3%82%88%E3%81%B3-ip-%E3%82%A2%E3%83%89%E3%83%AC%E3%82%B9%E7%AF%84%E5%9B%B2-8548a211-3fe7-47cb-abb1-355ea5aa88a2?ui=ja-JP&amp;rs=ja-JP&amp;ad=JP)  
  * [Microsoft Azure Datacenter IP Ranges](https://www.microsoft.com/en-us/download/details.aspx?id=41653)  

* {{%slash%}}共通管理画面での設定方法：  
  [IPアドレス制限とは](/general/ja/admin/list_security/list_access/ip_restrictions.html)

<br>
連携するサービスと{{%kintone%}}は、Microsoft Power Automateで同じデータグループに設定する必要があります。  

* Microsoft社の資料：  
  [データグループのすべて](https://docs.microsoft.com/ja-jp/flow/introduction-to-data-groups)

## Slackとの連携でできること {#list_externalservices_oauth_20}

[Slack](https://slack.com/intl/ja-jp/)はチャットサービスです。  
Slackと{{%kintone%}}を連携すると、プロセス管理でレコードの作業者になったユーザーにSlackのダイレクトメッセージで通知できるようになります。  
アプリとSlackを使ってタスクを管理する場合に便利な機能です。

## STEP1：{{%slash%}}共通管理画面で外部連携を許可する {#list_externalservices_oauth_30}

ここでは、Microsoft Power Automateとの連携を許可する場合を例に説明します。  

{{% enabled JP %}}

1. {{%kintone%}}のトップページで歯車アイコンをクリックし、「{{%slash%}}共通管理」をクリックします。  
  {{< screen src="/general/img-ja/oauth_img01.png"  alt="cybozu.com共通管理が赤枠で囲まれた画像">}}
1. 「{{%slash%}}共通管理」画面の「システム管理」の、[外部連携]をクリックします。
  {{< screen src="/general/img-ja/oauth_ja_03.png"  alt="[外部連携]が赤枠で囲まれた画像">}}
1. Microsoft Power Automateを[有効]にし、[連携利用ユーザーの設定]をクリックします。
  {{< screen src="/general/img-ja/oauth_ja_04.png"  alt="外部サービスとの連携を設定している画像">}}
1. [連携利用ユーザーの設定]画面で、外部連携サービスの利用を許可するユーザーにチェックを入れます。  
  組織を選択してユーザーを絞り込んだり、ユーザー検索パーツで検索したりできます。
  {{< screen src="/general/img-ja/oauth_ja_05.png"  alt="特定のユーザーを選択している画像">}}
1. [保存]をクリックします。
  {{< screen src="/general/img-ja/oauth_ja_06.png"  alt="[保存]が赤枠で囲まれた画像">}}
  {{%slash%}}共通管理画面での設定は、これで完了です。

{{% /enabled %}}

{{% enabled US %}}

1. {{%kintone%}}のトップページで歯車アイコンをクリックし、「{{%slash%}}共通管理」をクリックします。
  {{< screen src="/general/img-ja/oauth_img01_us.png"  alt="Kintone共通管理が赤枠で囲まれた画像">}}
1. 「{{%slash%}}共通管理」画面の「システム管理」の、[外部連携]をクリックします。
  {{< screen src="/general/img-ja/oauth_ja_03.png"  alt="[外部連携]が赤枠で囲まれた画像">}}
1. Microsoft Power Automateを[有効]にし、[連携利用ユーザーの設定]をクリックします。
  {{< screen src="/general/img-ja/oauth_ja_04.png"  alt="外部サービスとの連携を設定している画像">}}
1. [連携利用ユーザーの設定]画面で、外部連携サービスの利用を許可するユーザーにチェックを入れます。  
  組織を選択してユーザーを絞り込んだり、ユーザー検索パーツで検索したりできます。
  {{< screen src="/general/img-ja/oauth_ja_05.png"  alt="特定のユーザーを選択している画像">}}
1. [保存]をクリックします。
  {{< screen src="/general/img-ja/oauth_ja_06.png"  alt="[保存]が赤枠で囲まれた画像">}}
  {{%slash%}}共通管理画面での設定は、これで完了です。

{{% /enabled %}}

{{% enabled CN %}}

1. {{%kintone%}}のトップページで歯車アイコンをクリックし、「{{%slash%}}共通管理」をクリックします。
  {{< screen src="/general/img-ja/oauth_img01_cn.png"  alt="cybozu.cn共通管理が赤枠で囲まれた画像">}}
1. 「{{%slash%}}共通管理」画面の「システム管理」の、[外部連携]をクリックします。
  {{< screen src="/general/img-ja/oauth_ja_03.png"  alt="[外部連携]が赤枠で囲まれた画像">}}
1. Microsoft Power Automateを[有効]にし、[連携利用ユーザーの設定]をクリックします。
  {{< screen src="/general/img-ja/oauth_ja_04.png"  alt="特定のユーザーを選択している画像">}}
1. [連携利用ユーザーの設定]画面で、外部連携サービスの利用を許可するユーザーにチェックを入れます。  
  組織を選択してユーザーを絞り込んだり、ユーザー検索パーツで検索したりできます。
  {{< screen src="/general/img-ja/oauth_ja_05.png"  alt="特定のユーザーを選択している画像">}}
1. [保存]をクリックします。
  {{< screen src="/general/img-ja/oauth_ja_06.png"  alt="[保存]が赤枠で囲まれた画像">}}
  {{%slash%}}共通管理画面での設定は、これで完了です。

{{% /enabled %}}

## STEP2：{{%kintone%}}アプリ側で必要な設定をする {#list_externalservices_oauth_40}

{{%slash%}}共通管理画面での設定が完了したら、利用するサービスにあわせて、{{%kintone%}}アプリ側で必要な設定をします。  

### Microsoft Power Automateの場合 {#list_externalservices_oauth_4010}

次のページを参照し、{{%kintone%}}とWebサービスとの連携を設定します。  
{{% enabled JP %}}

* [Microsoft Power Automateと{{%kintone%}}を連携する](/k/ja/user/oauth/msflow.html)  
* [Microsoft Power Automateの{{%kintone%}}コネクタで特定のツイートを{{%kintone%}}に登録する](https://developer.cybozu.io/hc/ja/articles/115005486166)（cybozu developer network）

{{% /enabled %}}

{{% enabled US CN %}}

* [Microsoft Power Automateと{{%kintone%}}を連携する](/k/ja/user/oauth/msflow.html)  

{{% /enabled %}}

### Slackの場合 {#list_externalservices_oauth_4020}

次のページを参照し、{{%kintone%}}とWebサービスとの連携を設定します。  

* [Slackと{{%kintone%}}を連携する](/k/ja/user/oauth/slack_integration.html)  

## ユーザーが利用している外部連携サービスを確認する方法 {#list_externalservices_oauth_50}

* <b>{{%slash%}}共通管理者が確認する場合：</b>  
  ユーザー情報の編集画面で、ユーザーが利用中の外部連携サービスを確認できます。
  {{< screen src="/general/img-ja/oauth_ja_07.png"  alt="利用中の外部連携サービスが赤枠で囲まれた画像">}}
* <b>ユーザー自身が確認する場合：</b>  
  自分のアカウント設定から利用中の外部連携サービスを確認したり連携を解除したりできます。  
  [ユーザーが連携サービスを確認・解除する](/general/ja/user/list_personal/cooperation.html)

{{< seealso title="関連する記事" >}}
{{% enabled JP %}}
[{{%kintone%}}コネクタ（Microsoft Power Automate）を使う前に知っておきたいこと11選](https://developer.cybozu.io/hc/ja/articles/360000361506-help)
{{% /enabled %}}

{{% enabled US %}}
[11 Things to Know Before Using {{%kintone%}} with Microsoft Power Automate](https://www.kintone.com/ms-power-automate-things-to-know/)
{{% /enabled %}}
