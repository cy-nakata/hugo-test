---
title: "{{%store%}}の管理者を追加する"
weight: 200
disabled: [CN]
---
{{% enabled US %}}
{{% warning %}}
この記事は、[AWSへの移行](https://www.kintone.com/aws-migration/)が完了していないお客様向けです。ドメインIDが「c」で始まるお客様が該当します。ドメインIDを確認するには「[ドメインIDの確認方法](/general/ja/admin/list_old/domainid.html)」を参照してください。
{{% /warning %}}
{{% /enabled %}}

{{%store%}}の管理者を追加する手順を説明します。{{%store%}}の管理者は、サービスの発注や契約内容の変更、IP アドレス制限・Basic 認証の設定、ドメインの追加などを行います。{{%store%}}の管理者は複数設定できます。退職や異動などで管理者がいなくなる場合があるため、なるべく複数の管理者を設定してください。

{{% note %}}
{{% subtitle %}}
{{%store%}}管理者のサービス利用について
{{% /subtitle %}}

* {{%store%}}管理者は、{{%service%}} のサービスの利用は必須ではありません。サービスを利用していないユーザーが、{{%store%}}の管理者になることもできます。
* {{%store%}}の管理者と、{{%slash%}}共通管理者は別々に設定できるため、{{%store%}}の管理者でもサービスにログインできない場合があります。

{{% /note %}}

初めて{{%store%}}で試用を申し込んだアカウントは、自動的に{{%store%}}の管理者になります。{{%store%}}の管理者は複数人設定できます。{{%store%}}の管理者を追加する手順は、次のとおりです。

{{% enabled JP %}}

1. [{{%store%}}](https://store.cybozu.com/manage/)にログインします。
   {{< screen src="/general/img-ja/store_admin_ja_01.png"  alt="画像">}}
1. 「アカウント管理」画面の[管理者の追加]をクリックします。
   {{< screen src="/general/img-ja/store_admin_ja_JP_02.png"  alt="画像">}}
1. {{%store%}}の管理者に設定するアカウントのメールアドレスを記入し、[追加]をクリックします。  
   複数のメールアドレスを登録するには、メールアドレスを改行で区切ります。登録したメールアドレスに招待メールが送信されます。
   {{< screen src="/general/img-ja/store_admin_ja_03.png"  alt="画像">}}
1. 追加された管理者は招待メールを受信します。メールに記載されたURLにアクセスし、ログインします。  
   初めてログインする際にはパスワードを設定してください。ログインできたら設定は完了です。

{{% note %}}
{{% subtitle %}}
{{%CorpName%}}からの配信メール
{{% /subtitle %}}

{{%store%}}の管理者、ご連絡先、およびご請求先のメールアドレスには、{{%CorpName%}}からの配信メールが届きます。  
詳細は、[{{%CorpName%}}からのお知らせ／配信メール](/general/ja/admin/list_notice.html)を参照してください。
{{% /note %}}
{{% /enabled %}}

{{% enabled US %}}

1. [{{%store%}}](https://store.kintone.com/)にログインします。
   {{< screen src="/general/img-ja/store_admin_en_US_01.png"  alt="画像">}}
1. 「Accounts」画面の[New Account]をクリックします。
   {{< screen src="/general/img-ja/store_admin_en_US_02.png"  alt="画像">}}
1. {{%store%}}の管理者に設定するアカウントのメールアドレスを記入し、[Invite]をクリックします。  
   複数のメールアドレスを登録するには、メールアドレスを改行で区切ります。登録したメールアドレスに招待メールが送信されます。
   {{< screen src="/general/img-ja/store_admin_en_US_03.png"  alt="画像">}}
1. 追加された管理者は招待メールを受信します。メールに記載されたURLにアクセスし、ログインします。  
   初めてログインする際にはパスワードを設定してください。ログインできたら設定は完了です。

{{% /enabled %}}
