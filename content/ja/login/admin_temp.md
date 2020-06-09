---
title: "一時的な管理者を作成する"
weight: 700
disabled: [CN]
---

{{% enabled US %}}
{{% warning %}}
この記事は、[AWSへの移行](https://www.kintone.com/aws-migration/)が完了していないお客様向けです。ドメインIDが「c」で始まるお客様が該当します。ドメインIDを確認するには「[ドメインIDの確認方法](/general/ja/admin/list_old/domainid.html)」を参照してください。

**[AWSへの移行](https://www.kintone.com/aws-migration/)が完了したお客様（ドメインIDが「y」で始まるお客様）**  
{{%slash%}}共通管理者がログイン名を忘れるなどしてログインできない場合は、[サイボウズにお問い合わせ](https://www.kintone.com/support/)ください。

{{% /warning %}}
{{% /enabled %}}

一時的な管理者は、{{%store%}}の管理者だけが作成できる仮のユーザーです。作成から約1時間で利用停止になります。  
管理者の退職やアカウント情報の紛失などで、{{%service%}}の管理画面にアクセスできなくなった際に、一時的な管理者を作成します。  

{{% enabled JP %}}

1. {{%store%}}の管理者で、[{{%store%}}](https://store.{{%cybozu_com%}}/login)にログインします。  
  ログインできない場合は、[{{%store%}}にログインできません。](/general/ja/login/store_account.html)を参照してください。  

1. 「ドメイン管理」の「{{%slash%}}共通管理者」タブをクリックします。  
  {{< screen src="/general/img-ja/admin_temp_img01.png"  alt="ドメイン管理画面">}}  

1. 一時的な管理者のパスワードを入力し、[追加]をクリックします。  
  一時的な管理者のログイン情報がメールで送信されます。
  {{< screen src="/general/img-ja/admin_temp_img02.png"  alt="パスワードを入力する画像">}}  

1. {{%store%}}の管理者のメールアドレスに送信された、次のメールを確認します。  

  * メールの件名：  
    「[{{%service%}}_Store]_セキュリティ設定が行われました」  

1. メールに記載されたログイン名と、手順3で設定したパスワードで、{{%service%}}にログインします。  

1. [{{%slash%}}共通管理]をクリックします。  
  {{< screen src="/general/img-ja/admin_temp_img05.png"  alt="共通管理画面へのリンクアイコン">}}  

1. 「ユーザー管理」の[組織/ユーザー]をクリックし、ログインできない管理者の![編集アイコン](/general/img/slash_edit_icon.png)をクリックします。  
  {{< screen src="/general/img-ja/admin_temp_ja_03.png"  alt="組織とユーザーの設定画面">}}  

1. ログイン名の確認と[パスワードの変更](/general/ja/admin/list_useradmin/list_user/edit_userpw.html)を行います。  
  {{< screen src="/general/img-ja/admin_temp_ja_04.png"  alt="「ログイン名」と[パスワードの変更]が赤枠で囲まれた画像">}}  

1. {{%service%}}からログアウトします。  

1. 確認したログイン名とパスワードで、{{%service%}}にログインします。  

1. ログインが成功したら、一時的な管理者を削除します。  
  詳細は、[ユーザーを削除する](/general/ja/admin/list_useradmin/list_user/delete_user.html)を参照してください。  

1. 管理者がログインできない事態を回避できるよう、次の対応を検討します。  

      * <b>管理者を複数人設定する</b>：  
        {{%slash%}}共通管理で設定を変更できます。  
        詳細は[{{%slash%}}共通管理者の設定](/general/ja/admin/list_administrator/list_type_of_administrator/list_domain_auth.html)を参照してください。  
        {{< screen src="/general/img-ja/admin_temp_img06.png"  alt="「管理者の設定」メニューを示す画像">}}  

      * <b>パスワードリセットを許可する</b>：  
        {{%slash%}}共通管理で設定を変更できます。  
        パスワードポリシーに関する設定は、全ユーザーに適用されます。  
        {{< screen src="/general/img-ja/admin_temp_img07.png"  alt="パスワードポリシーに関する設定画面">}}  

{{% /enabled %}}

{{% enabled US %}}

1. {{%store%}}の管理者で、[{{%store%}}](https://store.kintone.com/)にログインします。  
  ログインできない場合は、[{{%store%}}にログインできません。](/general/ja/login/store_account.html)を参照してください。  

1. 「Domains」の「Administrator」タブを選択します。  
  {{< screen src="/general/img-ja/admin_temp_us_01.jpg"  alt="「Domains」画面">}}  

1. 一時的な管理者のパスワードを入力し、[Add]をクリックします。  
  一時的な管理者のログイン情報がメールで送信されます。
  {{< screen src="/general/img-ja/admin_temp_us_02.jpg"  alt="パスワードを入力する画像">}}  

1. {{%store%}}の管理者のメールアドレスに送信されたメールを確認します。  

1. メールに記載されたログイン名と、手順3で設定したパスワードで、{{%service%}}にログインします。  

1. [共通管理]をクリックします。  
  {{< screen src="/general/img-ja/admin_temp_img05_us.png"  alt="共通管理画面へのリンクアイコン">}}  

1. 「ユーザー管理」の[組織/ユーザー]をクリックし、ログインできない管理者の![編集アイコン](/general/img/slash_edit_icon.png)をクリックします。  
  {{< screen src="/general/img-ja/admin_temp_ja_03.png"  alt="組織とユーザーの設定画面">}}  

1. ログイン名の確認と[パスワードの変更](/general/ja/admin/list_useradmin/list_user/edit_userpw.html)を行います。  
  {{< screen src="/general/img-ja/admin_temp_ja_04.png"  alt="「ログイン名」と[パスワードの変更]が赤枠で囲まれた画像">}}  

1. {{%service%}}からログアウトします。  

1. 確認したログイン名とパスワードで、{{%service%}}にログインします。  

1. ログインが成功したら、一時的な管理者を削除します。  
  詳細は、[ユーザーを削除する](/general/ja/admin/list_useradmin/list_user/delete_user.html)を参照してください。  

1. 管理者がログインできない事態を回避できるよう、次の対応を検討します。  

      * <b>管理者を複数人設定する</b>：  
        {{%slash%}}共通管理で設定を変更できます。  
        詳細は[{{%slash%}}共通管理者の設定](/general/ja/admin/list_administrator/list_type_of_administrator/list_domain_auth.html)を参照してください。  
        {{< screen src="/general/img-ja/admin_temp_img06.png"  alt="「管理者の設定」メニューを示す画像">}}  

      * <b>パスワードリセットを許可する</b>：  
        {{%slash%}}共通管理で設定を変更できます。  
        パスワードポリシーに関する設定は、全ユーザーに適用されます。  
        {{< screen src="/general/img-ja/admin_temp_img07.png"  alt="パスワードポリシーに関する設定画面">}}  

{{% /enabled %}}

{{< seealso title="関連する記事" >}}

* [ログインできない：最初に確認すること](/general/ja/login/troubleshoot_first.html)
* [ログインできない：次に確認すること](/general/ja/login/troubleshoot_second.html)

{{< /seealso >}}
