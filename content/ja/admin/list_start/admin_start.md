---
title: "使用開始までの流れ（管理者向け）"
weight: 100
---
{{% enabled JP %}}
{{%service%}}とは、サイボウズが提供するクラウドサービスのプラットフォームです。

サイボウズのクラウドサービス（クラウド版Garoonやkintoneなど）を使用するには、最初にユーザー、組織、セキュリティなど、全クラウドサービスに共通する項目を設定する必要があります。  
{{< screen src="/general/img-ja/admin_start_01_jp.png" alt="cybozu.comのイメージ図">}}  
サイボウズのクラウドサービスを開始するまでの流れは、次のとおりです。
{{% /enabled %}}

{{% enabled US %}}
{{%slash%}}共通管理では、ユーザー管理やセキュリティ設定などを設定します。

{{%kintone%}}を開始するまでの流れは、次のとおりです。
{{% /enabled %}}

{{% enabled CN %}}
{{%service%}}とは、サイボウズが提供するクラウドサービスのプラットフォームです。  
Garoonや{{%kintone%}}を使用するには、最初にユーザー、組織、セキュリティなど、全クラウドサービスに共通する項目を設定する必要があります。  

サイボウズのクラウドサービスを開始するまでの流れは、次のとおりです。
{{% /enabled %}}

## STEP1 {{%slash%}}共通管理にアクセスする{#list_start_admin_start_10}

次の手順で、{{%slash%}}共通管理にアクセスします。

{{% enabled JP %}}
{{% note %}}
ログイン名やパスワードがわからない場合は、[管理者がアカウントやパスワードを忘れた場合](/general/ja/login/admin_account.html)を参照してください。  
{{% /note %}}

1. 「https://（サブドメイン名）.{{%cybozu_com%}}/」にアクセスします。
1. ログイン名とパスワードを入力し、[ログイン]をクリックします。  
    <table>
    <tbody>
        <tr>
            <th>ログイン名</th>
            <td>試用を申し込む際に登録したメールアドレスです。</td>
        </tr>
        <tr>
            <th>パスワード</th>
            <td>試用を申し込む際に入力したパスワードです。</td>
        </tr>
    </tbody>
</table>
{{< screen src="/general/img-ja/admin_start_02.png" alt="ログイン画面">}}

1. [{{%slash%}}共通管理]をクリックします。  
 {{< screen src="/general/img-ja/admin_start_03.png" alt="共通管理画面へのリンクアイコン">}}

{{% /enabled %}}

{{% enabled US %}}
{{% note %}}
ログイン名やパスワードがわからない場合は、[管理者がアカウントやパスワードを忘れた場合](/general/ja/login/admin_account.html)を参照してください。  
{{% /note %}}

1. 「https://（サブドメイン名）.{{%cybozu_com%}}/」にアクセスします。
1. ログイン名とパスワードを入力し、[ログイン]をクリックします。  
    <table>
    <tbody>
        <tr>
            <th>ログイン名</th>
            <td>試用を申し込む際に登録したメールアドレスです。</td>
        </tr>
        <tr>
            <th>パスワード</th>
            <td>試用を申し込む際に入力したパスワードです。</td>
        </tr>
    </tbody>
</table>
    {{< screen src="/general/img-ja/admin_start_02_us.png" alt="ログイン画面">}}
1. [共通管理]をクリックします。
    {{< screen src="/general/img-ja/admin_start_03_us.png" alt="共通管理画面へのリンクアイコン">}}
{{% /enabled %}}

{{% enabled CN %}}

1. 「https://（サブドメイン名）.{{%cybozu_com%}}/」にアクセスします。
1. ログイン名とパスワードを入力し、[ログイン]をクリックします。  
    <table>
    <tbody>
        <tr>
            <th>ログイン名</th>
            <td>試用を申し込む際に登録したメールアドレスです。<br />
            メールアドレスがわからない場合は、サイボウズにお問い合わせください。</td>
        </tr>
        <tr>
            <th>パスワード</th>
            <td>試用を申し込む際に入力したパスワードです。<br />
            パスワードがわからない場合は、サイボウズにお問い合わせください。</td>
        </tr>
    </tbody>
</table>
    {{< screen src="/general/img-ja/admin_start_02_cn.png" alt="ログイン画面">}}
1. [{{%slash%}}共通管理]をクリックします。
    {{< screen src="/general/img-ja/admin_start_03_cn.png" alt="共通管理画面へのリンクアイコン">}}
{{% /enabled %}}

## STEP2 組織を追加する{#list_start_admin_start_20}

ご自身の会社の組織構造に合わせて、組織を追加します。

{{% note %}}
{{% subtitle %}}
組織の一括登録
{{% /subtitle %}}

CSVファイルを読み込み、組織を一括登録することもできます。[組織を一括で登録、編集する](/general/ja/admin/list_useradmin/list_csv/org.html)
を参照してください。  
{{% /note %}}

1. 「組織/ユーザー」を選択し、「組織の追加」をクリックします。  
 {{< screen src="/general/img-ja/admin_start_04.jpg" alt="「組織の追加」をクリックする画面">}}
1. 必要な項目を入力し、[保存]をクリックします。  
  各項目の詳細は、[組織の設定画面](/general/ja/admin/list_useradmin/list_division/dprmntdetails.html)を参照してください。
  {{< screen src="/general/img-ja/admin_start_05.png" alt="組織の追加画面">}}
 組織の表示順を変更する手順など、組織に関するその他の設定については [組織の設定](/general/ja/admin/list_useradmin/list_division.html)を参照してください。  

## STEP3 ユーザーを追加する{#list_start_admin_start_30}

サービスを利用するユーザーを追加します。

{{% note %}}
{{% subtitle %}}
ユーザーの一括登録
{{% /subtitle %}}

CSVファイルを読み込み、ユーザーを一括登録することもできます。[ユーザーを一括で登録、編集する](/general/ja/admin/list_useradmin/list_csv/user.html)を参照してください。  
{{% /note %}}

1. 「組織/ユーザー」を選択し、[ユーザーの追加]をクリックします。  
 {{< screen src="/general/img-ja/admin_start_06.png" alt="「ユーザーの追加」を選択する画面">}}
1. 必要な項目を入力し、[保存]をクリックします。  
 「利用するサービス」では、このユーザーに利用を許可するサービスを選択します。  
 「所属組織」では、STEP2で追加した組織を選択します。  
 その他の項目については、[ユーザー情報の設定画面](/general/ja/admin/list_useradmin/list_user/user_details.html)を参照してください。  
 {{< screen src="/general/img-ja/admin_start_07.png" alt="ユーザーの追加画面">}}
1. 「パスワードの設定」ダイアログで、追加したユーザーのパスワードを設定します。
    {{< screen src="/general/img-ja/add_user_img05.png" alt="「パスワードの設定」ダイアログの画像">}}
    ユーザーに関するその他の設定については、[ユーザーの設定](/general/ja/admin/list_useradmin/list_user.html)を参照してください。

## STEP4 必要に応じて、セキュリティの設定をする{#list_start_admin_start_40}

必要に応じて、ログインのセキュリティ設定や、オフィス外からのアクセスに関するセキュリティ設定をします。なお、これらはあとからでも設定・変更できます。  
詳細は、下記のページを参照してください。  

* [最初に行うセキュリティ設定](/general/ja/admin/list_security/list_login.html)
* [よりセキュリティを高める設定](/general/ja/admin/list_security/list_access.html)

{{% enabled US %}}
{{% warning %}}
Basic認証とセキュアアクセスは、[AWSに移行](https://www.kintone.com/aws-migration/)したお客様（[ドメインID](/general/ja/admin/list_old/domainid.html)が「y」で始まるお客様）にはご利用いただけません。  
{{% /warning %}}
{{% /enabled %}}

## STEP5 必要に応じて、その他の項目を設定する{#list_start_admin_start_50}

{{% enabled JP %}}
Garoonや{{%kintone%}}の場合は、必要に応じて、追加で次の項目を設定します。なお、これらはあとからでも設定・変更できます。  

* [グループ（ロール）を追加する](/general/ja/admin/list_useradmin/list_group/set_group.html)
* [役職名を登録し、ユーザーに設定する](/general/ja/admin/list_useradmin/list_title/title.html)

{{% /enabled %}}

{{% enabled US CN %}}
必要に応じて、追加で次の項目を設定します。なお、これらはあとからでも設定・変更できます。  

* [グループ（ロール）を追加する](/general/ja/admin/list_useradmin/list_group/set_group.html)
* [役職名を登録し、ユーザーに設定する](/general/ja/admin/list_useradmin/list_title/title.html)

{{% /enabled %}}

{{% enabled JP %}}
{{% note %}}
{{% subtitle %}}
グループ（ロール）と役職に対応している製品
{{% /subtitle %}}

グループ（ロール）や役職は、Garoonと{{%kintone%}}で使用します。サイボウズOfficeとメールワイズでは使用しません。
{{% /note %}}
{{% /enabled %}}

## STEP6 各サービスを設定する{#list_start_admin_start_60}

{{% enabled JP %}}
右上の歯車アイコンをクリックし、各サービスの管理画面に移動し、サービスごとの設定を行います。  
{{< screen src="/general/img-ja/admin_start_09.png" alt="移動先の管理画面を選択している画像">}}
{{% /enabled %}}

{{% enabled US %}}
右上の歯車アイコンをクリックし、管理画面に移動して設定を行います。
{{< screen src="/general/img-ja/admin_start_09_us.png" alt="[Kintoneシステム管理]が赤枠で囲まれた画像">}}
{{% /enabled %}}

{{% enabled CN %}}
右上の歯車アイコンをクリックし、各サービスの管理画面に移動し、サービスごとの設定を行います。  
{{< screen src="/general/img-ja/admin_start_09_cn.png" alt="移動先の管理画面を選択している画像">}}
{{% /enabled %}}

## STEP7 ユーザーに利用情報を連絡する{#list_start_admin_start_70}

サービスを利用するユーザーに次の情報を伝えます。

* 利用するサービスのアクセスURL（https://(サブドメイン名).{{%cybozu_com%}}/）  
* 各ユーザーのログイン名
* 各ユーザーのパスワード
* ユーザーが使用を開始するまでの流れ  
  [{{%service%}}の使用開始までの流れ（ユーザー向け)](/general/ja/user/list_start/start.html)

{{% enabled JP %}}
{{< seealso title="関連する記事" >}}
[{{%store%}}](https://store.cybozu.com/login)
{{< /seealso >}}
{{% /enabled %}}
