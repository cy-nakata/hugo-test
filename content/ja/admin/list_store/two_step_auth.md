---
title: "2段階認証を設定する"
weight: 200
disabled: [CN]
---
{{% enabled US %}}
{{% warning %}}
この記事は、[AWSへの移行](https://www.kintone.com/aws-migration/)が完了していないお客様向けです。ドメインIDが「c」で始まるお客様が該当します。ドメインIDを確認するには「[ドメインIDの確認方法](/general/ja/admin/list_old/domainid.html)」を参照してください。
{{% /warning %}}
{{% /enabled %}}

2段階認証とは、メールアドレスとパスワードに加えて、毎回異なる確認コード（ワンタイムパスワード）を入力してログインする方法です。1度ログインに使用した確認コードは無効になるため、万が一、パスワードを盗まれた場合でも、不正ログインを防止できます。

2段階認証では、{{%store%}}のログイン画面でメールアドレスとパスワードを入力すると、指定したメールアドレス宛に確認コードが送信されます。メールに記載された確認コードをログイン画面に入力すると、{{%store%}}にログインできます。

{{% enabled JP %}}
{{< screen src="/general/img-ja/two_step_auth_jp_ja_01.png"  alt="2段階認証を説明する図">}}
{{% /enabled %}}

{{% enabled US %}}
{{< screen src="/general/img-ja/two_step_auth_us_ja_01.png"  alt="2段階認証を説明する図">}}
{{% /enabled %}}

## 2段階認証の設定手順 {#list_store_two_step_auth_10}

1. [{{%store%}}](https://store.{{%cybozu_com%}}/manage/)にログインします。
1. 左ナビで[アカウント管理]をクリックします。  
1. {{%store%}}管理者に登録されているアカウントを確認します。  
  {{< screen src="/general/img-ja/two_step_auth_jp_ja_03.png"  alt="ストアの画面">}}
  {{% note %}}
  {{% subtitle %}}2段階認証を設定する前に、必ず{{%store%}}管理者を複数人登録してください。{{% /subtitle %}}
  ワンタイムパスワードの送信先メールアドレスを忘れたり、失効したりすると、{{%store%}}にログインできません。また、2段階認証も解除できません。  
  複数の{{%store%}}管理者を登録していれば、次の手順でログインできない管理者を救済できます。  
  <br>
    1. 別の管理者が、ログインできないアカウントを削除する  
      [{{%store%}}の管理者を削除する](/general/ja/admin/list_administrator/list_type_of_administrator/store_admin_del.html)  
    2. 削除したアカウントを、管理者として追加し直す  
      [{{%store%}}の管理者を追加する](/general/ja/admin/list_administrator/list_type_of_administrator/store_admin.html)
  {{% /note %}}
1. 右上のメールアドレスをクリックし、ドロップダウンリストから[アカウント設定]を選択します。
1. 「2段階認証」の[設定]をクリックします。
  {{< screen src="/general/img-ja/two_step_auth_jp_ja_02.png"  alt="ストアの画面">}}
1. Email欄に確認コードの送信先メールアドレスを入力します。  
  確認コードは、{{%store%}}のログインに使用しているメールアドレス宛には送信できません。別のメールアドレスを用意してください。  
1. [送信]をクリックします。  
  確認コードを含むメールが送信されます。  
  {{%store%}}の画面はそのまま表示しておきます。
1. 手順6で指定したメールアドレスで「[{{%service%}} Store] セキュリティ確認コード」のメールを受信します。  
  確認コード（6桁の数字）を入手します。
1. {{%store%}}の「確認コード」欄に確認コードを入力し、[確認]をクリックします。
1. [設定]をクリックします。  
  これで2段階認証の設定は完了です。

## 2段階認証を設定している場合のログイン手順 {#list_store_two_step_auth_20}

1. [{{%store%}}](https://store.{{%cybozu_com%}}/manage/)で、メールアドレスとパスワードを入力し、[ログイン]をクリックします。  
  設定手順6で登録したメールアドレスに確認コードを送信した旨のメッセージが表示されます。
1. メールを受信します。
1. 記載されている確認コード（6桁の数字）を、{{%store%}}の「確認コード」欄に入力します。
1. [確認]をクリックします。  
  ログインに成功すると「契約管理」画面が表示されます。
