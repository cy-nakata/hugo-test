---
title: "2段階認証のメールアドレスを変更する"
weight: 300
disabled: [CN]
---
{{% enabled US %}}
{{% warning %}}
この記事は、[AWSへの移行](https://www.kintone.com/aws-migration/)が完了していないお客様向けです。ドメインIDが「c」で始まるお客様が該当します。ドメインIDを確認するには「[ドメインIDの確認方法](/general/ja/admin/list_old/domainid.html)」を参照してください。
{{% /warning %}}
{{% /enabled %}}

{{% enabled JP %}}
2段階認証の確認コードの送信先メールアドレスを変更します。
{{%store%}}のログインに使用しているメールアドレスには指定できません。

1. {{%store%}}にログインします。
1. 右上のメールアドレスをクリックし、ドロップダウンリストから[アカウント設定]を選択します。
1. 「アカウント設定」画面で、「2段階認証」の[変更]をクリックします。
1. 「Email」欄に、新しいメールアドレスを入力し、[送信]をクリックします。確認コードを含むメールが送信されます。{{%store%}}の画面はそのまま表示しておきます。
1. 手順4で指定したメールアドレスで「[{{%service%}} Store] セキュリティ確認コード」のメールを受信し、確認コード（6桁の数字）を入手します。
1. {{%store%}}の「確認コード」欄に確認コードを入力し、[確認]をクリックします。
1. [設定]をクリックします。

{{% /enabled %}}
{{% enabled US %}}
2段階認証の確認コードの送信先メールアドレスを変更します。
{{%store%}}のログインに使用しているメールアドレスには変更できません。

1. {{%store%}}にログインします。
1. 右上のメールアドレスをクリックし、ドロップダウンリストから[Account Settings]を選択します。
1. 「Account Settings」画面で、「Two-Step Verification」の[Enable Two-Step Verification]をクリックします。
1. 「Email」欄に、新しいメールアドレスを入力し、[Send]をクリックします。
  確認コードを含むメールが送信されます。
  {{%store%}}の画面はそのまま表示しておきます。
1. 手順4で指定したメールアドレスで「[{{%service%}} Store] Verification Code」のメールを受信し、確認コード（6桁の数字）を入手します。
1. {{%store%}}の「Verification Code」欄に確認コードを入力し、[Verify]をクリックします。
1. [Save]をクリックします。

{{% /enabled %}}
{{< seealso title="関連する記事" >}}  
[{{%store%}}](https://store.{{%cybozu_com%}}/manage/)
{{< /seealso >}}
