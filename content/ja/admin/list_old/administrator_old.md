---
title: "管理者の種類（AWSへの移行が未完了のお客様向け）"
weight: 150
disabled: [JP,CN]
---
{{% warning %}}
この記事は、[AWSへの移行](https://www.kintone.com/aws-migration/)が完了していないお客様向けです。ドメインIDが「c」で始まるお客様が該当します。ドメインIDを確認するには「[ドメインIDの確認方法](/general/ja/admin/list_old/domainid.html)」を参照してください。
{{% /warning %}}

{{% enabled JP US %}}
{{%service%}}の管理者には、次の4種類があります。

* {{%store%}}の管理者  
  {{%service%}}の契約や、{{%service%}}へのアクセス制限の設定などをする管理者です。
* {{%slash%}}共通管理者  
  ユーザーの追加や、クライアント証明書の発行など、{{%service%}}で各種設定業務を行う管理者です。権限を付与されている場合、サービスの発注やアクセス制限の設定も可能です。
* Administrator  
  ドメインを作成した際に自動的に登録される、特別なユーザーです。初期状態では「停止中」のため、ユーザーとしては使用できません。詳細については、次のページを参照してください。  
  [Administratorとは](/general/ja/admin/list_administrator/list_type_of_administrator/whatisadmin.html)
* 組織の管理者  
  特定の組織で、ユーザーと組織に関する管理業務を行うユーザーです。初期状態では存在しておらず、{{%slash%}}共通管理者が、必要に応じて作成します。詳細については、次のページを参照してください。  
  [組織の管理者とは](/general/ja/admin/list_administrator/list_type_of_administrator/whatisumaadmin.html)

{{% /enabled %}}

{{% enabled CN %}}
{{%service%}}の管理者には、次の3種類があります。

* {{%slash%}}共通管理者  
  ユーザーの追加や、クライアント証明書の発行など、{{%service%}}で各種設定業務を行う管理者です。
* Administrator  
  ドメインを作成した際に自動的に登録される、特別なユーザーです。初期状態では「停止中」のため、ユーザーとしては使用できません。詳細については、次のページを参照してください。  
  [Administratorとは](/general/ja/admin/list_administrator/list_type_of_administrator/whatisadmin.html)
* 組織の管理者  
  特定の組織で、ユーザーと組織に関する管理業務を行うユーザーです。初期状態では存在しておらず、{{%slash%}}共通管理者が、必要に応じて作成します。詳細については、次のページを参照してください。  
  [組織の管理者とは](/general/ja/admin/list_administrator/list_type_of_administrator/whatisumaadmin.html)

{{% /enabled %}}

{{% enabled JP %}}
{{%service%}}環境を新規に作成したユーザーは、{{%store%}}の管理者と{{%slash%}}共通管理者の両方の権限を持ちます。
各管理者が管理できる主な項目は、次のとおりです。
<table cellpadding="1" cellspacing="1">
    <tbody>
        <tr>
            <th rowspan="2" style="text-align: center;">管理できる項目</th>
            <th rowspan="2">
            <div>{{%store%}}の管理者</div>
            &nbsp;</th>
            <th colspan="2" style="text-align: center;">{{%slash%}}共通管理者</th>
        </tr>
        <tr>
            <th style="text-align: left;">契約情報やアクセス制限の設定権限あり</th>
            <th style="text-align: left;">契約情報やアクセス制限の設定権限なし</th>
        </tr>
        <tr>
            <th style="text-align: left;"><span style="line-height: 20.8px;">会社情報の編集</span>&nbsp;</th>
            <td style="text-align: center; vertical-align: middle;">○</td>
            <td style="text-align: center; vertical-align: middle;">○</td>
            <td style="text-align: center; vertical-align: middle;">&times;</td>
        </tr>
        <tr>
            <th style="text-align: left;">各サービスの購入・見積・解約&nbsp;</th>
            <td style="text-align: center; vertical-align: middle;">○</td>
            <td style="text-align: center; vertical-align: middle;">○</td>
            <td style="text-align: center; vertical-align: middle;">&times;</td>
        </tr>
        <tr>
            <th style="text-align: left;">各サービスの試用申し込み</th>
            <td style="text-align: center; vertical-align: middle;">○</td>
            <td style="text-align: center; vertical-align: middle;">○</td>
            <td style="text-align: center; vertical-align: middle;">&times;</td>
        </tr>
        <tr>
            <th style="text-align: left;">ユーザー数追加・減数の発注・見積&nbsp;</th>
            <td style="text-align: center; vertical-align: middle;">○</td>
            <td style="text-align: center; vertical-align: middle;">○</td>
            <td style="text-align: center; vertical-align: middle;">&times;</td>
        </tr>
        <tr>
            <th style="text-align: left;">{{%store%}}の管理者の設定</th>
            <td style="text-align: center; vertical-align: middle;">○</td>
            <td style="text-align: center; vertical-align: middle;">&times;</td>
            <td style="text-align: center; vertical-align: middle;">&times;</td>
        </tr>
        <tr>
            <th style="text-align: left;">IPアドレス制限とBasic認証の設定</th>
            <td style="text-align: center; vertical-align: middle;">○</td>
            <td style="text-align: center; vertical-align: middle;">○</td>
            <td style="text-align: center; vertical-align: middle;">&times;</td>
        </tr>
        <tr>
            <th style="text-align: left;">ドメインの追加</th>
            <td style="text-align: center; vertical-align: middle;">○</td>
            <td style="text-align: center; vertical-align: middle;">&times;</td>
            <td style="text-align: center; vertical-align: middle;">&times;</td>
        </tr>
        <tr>
            <th style="text-align: left;">ドメイン名の変更</th>
            <td style="text-align: center; vertical-align: middle;">○</td>
            <td style="text-align: center; vertical-align: middle;">○</td>
            <td style="text-align: center; vertical-align: middle;">&times;</td>
        </tr>
        <tr>
            <th style="text-align: left;">サービスを利用するユーザーの追加・編集・削除</th>
            <td style="text-align: center; vertical-align: middle;">&times;</td>
            <td style="text-align: center; vertical-align: middle;">○</td>
            <td style="text-align: center; vertical-align: middle;">○</td>
        </tr>
        <tr>
            <th style="text-align: left;">パスワードポリシーの設定</th>
            <td style="text-align: center; vertical-align: middle;">&times;</td>
            <td style="text-align: center; vertical-align: middle;">○</td>
            <td style="text-align: center; vertical-align: middle;">○</td>
        </tr>
        <tr>
            <th style="text-align: left;">{{%kintone%}}のシステム設定</th>
            <td style="text-align: center; vertical-align: middle;">&times;</td>
            <td style="text-align: center; vertical-align: middle;">○</td>
            <td style="text-align: center; vertical-align: middle;">○</td>
        </tr>
        <tr>
            <th style="text-align: left;">監査ログの閲覧</th>
            <td style="text-align: center; vertical-align: middle; margin-left: 0px;">&times;</td>
            <td style="text-align: center; vertical-align: middle;">○</td>
            <td style="text-align: center; vertical-align: middle;">○</td>
        </tr>
    </tbody>
</table>

{{% note %}}
{{% subtitle %}}
2014年11月8日までに作成された環境の場合
{{% /subtitle %}}

初期状態では、{{%slash%}}共通管理者には契約情報やアクセス制限の設定変更権限はありません。権限を付与するには、{{%store%}}での設定を変更する必要があります。詳細は次の項目を参照してください。  
[契約情報やアクセス制限の設定変更の権限を{{%service%}}管理者に付与する](/general/ja/admin/list_administrator/store_auth.html)
{{% /note %}}
{{% /enabled %}}

{{% enabled US %}}
{{%service%}}環境を新規に作成したユーザーは、{{%store%}}の管理者と{{%slash%}}共通管理者の両方の権限を持ちます。
各管理者が管理できる主な項目は、次のとおりです。

<table cellpadding="1" cellspacing="1">
    <tbody>
        <tr>
            <th rowspan="2" style="text-align: center;">管理できる項目</th>
            <th rowspan="2">
            <div>{{%store%}}の管理者</div>
            &nbsp;</th>
            <th colspan="2" style="text-align: center;">{{%slash%}}共通管理者</th>
        </tr>
        <tr>
            <th style="text-align: left;">契約情報やアクセス制限の設定権限あり</th>
            <th style="text-align: left;">契約情報やアクセス制限の設定権限なし</th>
        </tr>
        <tr>
            <th style="text-align: left;"><span style="line-height: 20.8px;">会社情報の編集</span>&nbsp;</th>
            <td style="text-align: center; vertical-align: middle;">○</td>
            <td style="text-align: center; vertical-align: middle;">○</td>
            <td style="text-align: center; vertical-align: middle;">&times;</td>
        </tr>
        <tr>
            <th style="text-align: left;">各サービスの購入・見積・解約&nbsp;</th>
            <td style="text-align: center; vertical-align: middle;">○</td>
            <td style="text-align: center; vertical-align: middle;">○</td>
            <td style="text-align: center; vertical-align: middle;">&times;</td>
        </tr>
        <tr>
            <th style="text-align: left;">各サービスの試用申し込み</th>
            <td style="text-align: center; vertical-align: middle;">○</td>
            <td style="text-align: center; vertical-align: middle;">○</td>
            <td style="text-align: center; vertical-align: middle;">&times;</td>
        </tr>
        <tr>
            <th style="text-align: left;">ユーザー数追加・減数の発注・見積&nbsp;</th>
            <td style="text-align: center; vertical-align: middle;">○</td>
            <td style="text-align: center; vertical-align: middle;">○</td>
            <td style="text-align: center; vertical-align: middle;">&times;</td>
        </tr>
        <tr>
            <th style="text-align: left;">{{%store%}}の管理者の設定</th>
            <td style="text-align: center; vertical-align: middle;">○</td>
            <td style="text-align: center; vertical-align: middle;">&times;</td>
            <td style="text-align: center; vertical-align: middle;">&times;</td>
        </tr>
        <tr>
            <th style="text-align: left;">IPアドレス制限とBasic認証の設定</th>
            <td style="text-align: center; vertical-align: middle;">○</td>
            <td style="text-align: center; vertical-align: middle;">○</td>
            <td style="text-align: center; vertical-align: middle;">&times;</td>
        </tr>
        <tr>
            <th style="text-align: left;">ドメインの追加</th>
            <td style="text-align: center; vertical-align: middle;">○</td>
            <td style="text-align: center; vertical-align: middle;">&times;</td>
            <td style="text-align: center; vertical-align: middle;">&times;</td>
        </tr>
        <tr>
            <th style="text-align: left;">ドメイン名の変更</th>
            <td style="text-align: center; vertical-align: middle;">○</td>
            <td style="text-align: center; vertical-align: middle;">○</td>
            <td style="text-align: center; vertical-align: middle;">&times;</td>
        </tr>
        <tr>
            <th style="text-align: left;">サービスを利用するユーザーの追加・編集・削除</th>
            <td style="text-align: center; vertical-align: middle;">&times;</td>
            <td style="text-align: center; vertical-align: middle;">○</td>
            <td style="text-align: center; vertical-align: middle;">○</td>
        </tr>
        <tr>
            <th style="text-align: left;">パスワードポリシーの設定</th>
            <td style="text-align: center; vertical-align: middle;">&times;</td>
            <td style="text-align: center; vertical-align: middle;">○</td>
            <td style="text-align: center; vertical-align: middle;">○</td>
        </tr>
        <tr>
            <th style="text-align: left;">{{%kintone%}}のシステム設定</th>
            <td style="text-align: center; vertical-align: middle;">&times;</td>
            <td style="text-align: center; vertical-align: middle;">○</td>
            <td style="text-align: center; vertical-align: middle;">○</td>
        </tr>
        <tr>
            <th style="text-align: left;">監査ログの閲覧</th>
            <td style="text-align: center; vertical-align: middle; margin-left: 0px;">&times;</td>
            <td style="text-align: center; vertical-align: middle;">○</td>
            <td style="text-align: center; vertical-align: middle;">○</td>
        </tr>
    </tbody>
</table>
{{% /enabled %}}

{{% enabled CN %}}
{{%slash%}}共通管理者は、{{%slash%}}共通管理画面で、サービスを利用するユーザーの追加、編集、削除などのユーザー管理、および、パスワードポリシーやクライアント証明書の設定などのシステム管理などを行います。
管理者が管理できる主な項目は、次のとおりです。
<table cellpadding="1" cellspacing="1">
    <tbody>
        <tr>
            <th style="text-align:center;">管理できる項目</th>
            <th style="text-align:center;">{{%slash%}}共通管理者</th>
        </tr>
        <tr>
            <th><span style="line-height: 20.7999992370605px;">サービスを利用するユーザーの追加・編集・削除 </span></th>
            <td style="text-align:center;vertical-align:middle">○</td>
        </tr>
        <tr>
            <th>パスワードポリシーの設定</th>
            <td style="text-align:center;vertical-align:middle">○</td>
        </tr>
        <tr>
            <th>各サービスのシステム設定</th>
            <td style="text-align:center;vertical-align:middle">○</td>
        </tr>
        <tr>
            <th>監査ログの閲覧</th>
            <td style="text-align:center;vertical-align:middle">○</td>
        </tr>
    </tbody>
</table>
{{% /enabled %}}
