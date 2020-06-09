---
title: "組織の管理者とは"
weight: 600
---
組織の管理者とは、特定の組織配下において、ユーザーと組織を管理する権限を付与された管理者のことをいいます。
複数の拠点を持つ組織や、ユーザー数が多い組織では、{{%slash%}}共通管理者が行うユーザー管理・組織管理業務の負荷も大きくなります。{{%slash%}}共通管理者は、必要に応じて、組織の管理者を割り当て、ユーザーと組織の管理を委任できます。

{{% enabled JP CN %}}
{{% warning %}}
{{% subtitle %}}
組織の管理者を設定できる条件
{{% /subtitle %}}組織の管理者は、{{%kintone%}}、もしくはGaroonを契約している場合のみ設定できます。
{{% /warning %}}
{{% /enabled %}}

{{% enabled US %}}
{{% warning %}}
{{% subtitle %}}
組織の管理者を設定できる条件
{{% /subtitle %}}組織の管理者は、{{%kintone%}}を契約している場合のみ設定できます。
{{% /warning %}}
{{% /enabled %}}

## {{%slash%}}共通管理者と、組織の管理者の関係性

![画像](/general/img-ja/whatisumaadmin_01_ja.png)

## 組織の管理者が管理できる項目

組織の管理者は、管理権限を持つ組織の配下で、ユーザーと組織に関する管理業務ができますが、役職の設定など、一部の設定はできません。
{{%slash%}}共通管理と組織の管理者の、管理できる項目の違いは次のとおりです。

* &#10004;：管理者が操作できることを示します。
* 空欄：管理者が操作できないことを示します。

{{% enabled JP CN %}}
<table cellpadding="1" cellspacing="1">
    <tbody>
        <tr>
            <th style="text-align: center;" colspan="2" width="142"><b>管理できる項目</b></th>
            <th style="text-align: center;" width="115"><b>&nbsp;{{%service%}}<br />
            共通管理者</b></th>
            <th style="text-align: center;" width="120"><b>&nbsp;組織の管理者</b></th>
        </tr>
        <tr>
            <th width="142" rowspan="8">ユーザー管理</th>
            <th width="200">組織とユーザー</th>
            <td style="text-align: center;" width="115">&nbsp;&#10004;</td>
            <td style="text-align: center;" width="120">&nbsp;&#10004;</td>
        </tr>
        <tr>
            <th width="200">サービスの利用ユーザー</th>
            <td style="text-align: center;" width="115">&nbsp;&#10004;</td>
            <td style="text-align: center;" width="120">&nbsp;&#10004;</td>
        </tr>
        <tr>
            <th width="200">組織の管理権限の付与</th>
            <td style="text-align: center;" width="115">&nbsp;&#10004;</td>
            <td style="text-align: center;" width="120">&nbsp;&#10004;</td>
        </tr>
        <tr>
            <th width="200">役職</th>
            <td style="height: 17px; text-align: center;" width="115">&nbsp;&#10004;</td>
            <td style="text-align: center;" width="120">&nbsp;</td>
        </tr>
        <tr>
            <th width="200">グループ（ロール）</th>
            <td style="text-align: center;" width="115">&nbsp;&#10004;</td>
            <td style="text-align: center;" width="120">&nbsp;</td>
        </tr>
        <tr>
            <th width="200">一括操作</th>
            <td style="text-align: center;" width="115">&nbsp;&#10004;</td>
            <td style="text-align: center;" width="120">&nbsp;</td>
        </tr>
        <tr>
            <th width="200">組織の事前設定</th>
            <td style="text-align: center;" width="115">&nbsp;&#10004;</td>
            <td style="text-align: center;" width="120">&nbsp;</td>
        </tr>
        <tr>
            <th width="200">組織間のアクセス権</th>
            <td style="text-align: center;" width="115">&nbsp;&#10004;</td>
            <td style="text-align: center;" width="120">&nbsp;</td>
        </tr>
        <tr>
            <th width="142">&nbsp;システム管理</th>
            <th width="200">すべての設定項目</th>
            <td style="text-align: center;" width="115">&nbsp;&#10004;</td>
            <td style="text-align: center;" width="120">&nbsp;</td>
        </tr>
    </tbody>
</table>
{{% /enabled %}}

{{% enabled US %}}
<table cellpadding="1" cellspacing="1">
    <tbody>
        <tr>
            <th style="text-align: center;" colspan="2" width="142"><b>管理できる項目</b></th>
            <th style="text-align: center;" width="115"><b>&nbsp;{{%service%}}<br />
            共通管理者</b></th>
            <th style="text-align: center;" width="120"><b>&nbsp;組織の管理者</b></th>
        </tr>
        <tr>
            <th width="142" rowspan="7">ユーザー管理</th>
            <th width="200">組織とユーザー</th>
            <td style="text-align: center;" width="115">&nbsp;&#10004;</td>
            <td style="text-align: center;" width="120">&nbsp;&#10004;</td>
        </tr>
        <tr>
            <th width="200">サービスの利用ユーザー</th>
            <td style="text-align: center;" width="115">&nbsp;&#10004;</td>
            <td style="text-align: center;" width="120">&nbsp;&#10004;</td>
        </tr>
        <tr>
            <th width="200">組織の管理権限の付与</th>
            <td style="text-align: center;" width="115">&nbsp;&#10004;</td>
            <td style="text-align: center;" width="120">&nbsp;&#10004;</td>
        </tr>
        <tr>
            <th width="200">役職</th>
            <td style="height: 17px; text-align: center;" width="115">&nbsp;&#10004;</td>
            <td style="text-align: center;" width="120">&nbsp;</td>
        </tr>
        <tr>
            <th width="200">グループ（ロール）</th>
            <td style="text-align: center;" width="115">&nbsp;&#10004;</td>
            <td style="text-align: center;" width="120">&nbsp;</td>
        </tr>
        <tr>
            <th width="200">一括操作</th>
            <td style="text-align: center;" width="115">&nbsp;&#10004;</td>
            <td style="text-align: center;" width="120">&nbsp;</td>
        </tr>
        <tr>
            <th width="200">組織間のアクセス権</th>
            <td style="text-align: center;" width="115">&nbsp;&#10004;</td>
            <td style="text-align: center;" width="120">&nbsp;</td>
        </tr>
        <tr>
            <th width="142">&nbsp;システム管理</th>
            <th width="200">すべての設定項目</th>
            <td style="text-align: center;" width="115">&nbsp;&#10004;</td>
            <td style="text-align: center;" width="120">&nbsp;</td>
        </tr>
    </tbody>
</table>
{{% /enabled %}}

組織の管理者を設定する手順は、次のページを参照してください。  
[組織の管理者を設定する](/general/ja/admin/list_uma/usermanagement_assign.html)  

組織の管理者による作業については、次のページを参照してください。  
[組織の管理者による作業](/general/ja/admin/list_uma/list_userdptmnt.html)  
