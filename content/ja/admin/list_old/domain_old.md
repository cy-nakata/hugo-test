---
title: "サブドメインを変更する（AWSへの移行が未完了のお客様向け）"
weight: 400
disabled: [JP,CN]
---
{{% warning %}}
この記事は、[AWSへの移行](https://www.kintone.com/aws-migration/)が完了していないお客様向けです。ドメインIDが「c」で始まるお客様が該当します。ドメインIDを確認するには「[ドメインIDの確認方法](/general/ja/admin/list_old/domainid.html)」を参照してください。
{{% /warning %}}

「サブドメイン」は、{{%service%}}を利用するときに、WebブラウザーでアクセスするURLに含まれる文字列です。

{{% enabled JP %}}
{{< screen src="/general/img-ja/subdomain330_ja_01.png" alt="サブドメインを説明する画像">}}  
{{%store%}}の「契約管理」画面に、設定済のドメイン名が表示されています。  
サブドメイン部分は{{%store%}}または{{%slash%}}共通管理で変更できます。
{{% /enabled %}}

{{% enabled US %}}
{{< screen src="/general/img-ja/subdomain330_us_ja_01.png" alt="サブドメインを説明する画像">}}  
{{%store%}}の「Services License」画面に、設定済のドメイン名が表示されています。  
サブドメイン部分は{{%store%}}または{{%slash%}}共通管理で変更できます。
{{% /enabled %}}

{{% warning %}}
サブドメインを変更すると、これまで利用していたURLでは{{%service%}}の各サービスにアクセスできなくなります。  
利用ユーザーへのURLの変更の連絡が必要です。  
ブックマークや、各サービスで参照しているURLも変更する必要があります。
{{% /warning %}}

## {{%store%}}で変更する場合 {#list_old_domain_old_10}

{{% enabled JP %}}

1. {{%store%}}の管理者で、{{%store%}}にログインします。  
 {{< screen src="/general/img-ja/domain_img02.png" alt="ドットコムストアのログイン画面">}}  
「契約管理」画面には、利用中のサービスや、設定されているドメインなどが表示されています。  
 {{%store%}}の管理者については[管理者の種類](/general/ja/admin/list_administrator/list_type_of_administrator/administrator.html)を参照してください。  
1. 左側のメニューで、[ドメイン管理]をクリックします。  
 {{< screen src="/general/img-ja/domain_img03.png" alt="[ドメイン管理]が赤枠で囲まれた画像">}}
1. 「ドメイン名の変更」欄の[変更]をクリックします。複数のドメインを利用している場合は、設定するドメインをプルダウンメニューから選択し、[変更]をクリックします。  
 {{< screen src="/general/img-ja/domain_img04.png" alt="ドメイン管理画面">}}
1. 新しいドメイン名の枠内に、新しいサブドメイン名を記入し、[変更]をクリックします。  
 サブドメインには、半角英数と「-（ハイフン）」のみ使用できます。  
 3文字以上32文字以下で設定してください。  
 入力したドメイン名が、すでに他のお客様により使用されている場合や、使用できない文字が含まれる場合などは、「使用できません」や「入力内容を確認してください」などのメッセージが表示されます。  
 使用可能な場合は、「使用できます」と表示されます。  
 {{< screen src="/general/img-ja/domain_img05.png" alt="新しいドメイン名を入力する画像">}}  
1. 設定が完了すると、「ドメイン名の変更を受け付けました。」と表示されます。  
 設定が反映されるまでしばらく時間がかかることがあります。
 {{< screen src="/general/img-ja/domain_img06.png" alt="ドメイン管理画面">}}  
1. 設定が反映されると、契約管理画面に新しいドメイン名が表示されます。  
 {{< screen src="/general/img-ja/subdomain330_ja_08.png" alt="新しいドメイン名が表示された画像">}}

{{% /enabled %}}

{{% enabled US %}}

1. {{%store%}}の管理者で、{{%store%}}にログインします。  
 {{< screen src="/general/img-ja/storelogin330_us_01.png" alt="Kintone Storeのログイン画面">}}  
「Services License」画面には、利用中のサービスや、設定されているドメインなどが表示されています。  
 {{%store%}}の管理者については[管理者の種類](/general/ja/admin/list_administrator/list_type_of_administrator/administrator.html)を参照してください。  
1. 左側のメニューで、[Domains]をクリックします。  
 {{< screen src="/general/img-ja/storeacount_us_ja_03.png" alt="[Domains]が赤枠で囲まれた画像">}}
1. 「Current Domain Name」欄の[Change Domain Name]をクリックします。複数のドメインを利用している場合は、設定するドメインをプルダウンメニューから選択し、[Change Domain Name]をクリックします。  
 {{< screen src="/general/img-ja/storedomain_us_ja_01.png" alt="Domains画面">}}
1. 新しいドメイン名の枠内に、新しいサブドメイン名を記入し、[Save]をクリックします。  
 サブドメインには、半角英数と「-（ハイフン）」のみ使用できます。  
 3文字以上32文字以下で設定してください。  
 入力したドメイン名が、すでに他のお客様により使用されている場合や、使用できない文字が含まれる場合などは、「Not available」や「The entered name is not valid.」などのメッセージが表示されます。  
 使用可能な場合は、「Available」と表示されます。  
 {{< screen src="/general/img-ja/storedomain_us_ja_02.png" alt="新しドメイン名を入力する画像">}}  
1. 設定が完了すると、「Your request was accepted.」と表示されます。  
 設定が反映されるまでしばらく時間がかかることがあります。
1. 設定が反映されると、「Services License」画面に新しいドメイン名が表示されます。

{{% /enabled %}}

## {{%slash%}}共通管理で変更する場合  {#list_old_domain_old_20}

「契約状況」画面に、見積、購入、解約ボタンなどが表示されている場合のみ、次の手順でドメイン名を変更できます。

{{% enabled JP %}}

1. {{%slash%}}共通管理画面で、[契約状況]をクリックします。
1. 「契約状況」画面で、[詳細な契約状況]をクリックします。  
 [詳細な契約状況]が表示されない場合は、{{%slash%}}共通管理ではドメイン名を変更できません。  
 {{< screen src="/general/img-ja/domain_jp_ja_01.png" alt="[詳細な契約状況]が赤枠で囲まれた画像">}}  
1. 「詳細な契約状況」画面で、「ドメイン名」の右の[変更]をクリックします。
1. 新しいドメイン名を入力し、[保存]をクリックします。

{{% /enabled %}}

{{% enabled US %}}

1. {{%slash%}}共通管理画面で、[契約状況]をクリックします。
1. 「契約状況」画面で、[詳細な契約状況]をクリックします。  
 [詳細な契約状況]が表示されない場合は、{{%slash%}}共通管理ではドメイン名を変更できません。  
 {{< screen src="/general/img-ja/domain_us_ja_01.png" alt="[詳細な契約状況]が赤枠で囲まれた画像">}}  
1. 「Payment Details」画面で、「Domain Name」の右の[Change Domain Name]をクリックします。
1. 新しいドメイン名を入力し、[Save]をクリックします。

{{% /enabled %}}
