---
title: "「グループ（ロール）の追加」画面の項目"
weight: 600
---
グループ（ロール）情報で設定できる項目を説明します。  
グループ（ロール）を追加する手順は、[グループ（ロール）を追加する](/general/ja/admin/list_useradmin/list_group/set_group.html#list_group_set_group_20)方法を参照してください。

{{% enabled JP %}}
{{% warning %}}

グループ（ロール）の設定は、サイボウズ Officeとメールワイズには反映されません。

{{% /warning %}}
{{% /enabled %}}

画面で「&ast;」のついている項目は、必須項目です。
{{< screen src="/general/img-ja/group_details_img01.png" alt="グループ（ロール）の追加画面">}}

<table>
    <thead>
        <tr>
            <th scope="col">項目名</th>
            <th scope="col">説明</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>グループ名</td>
            <td>各サービスで表示されるグループ（ロール）の名前を入力します。<br />
            ほかのグループ名と重複しない任意の文字列を入力します。<br>
            「LoginUser」と「CommandLine」は、グループ名には使用できません。</td>
        </tr>
        <tr>
            <td>グループコード</td>
            <td>ほかのグループコードと重複しない任意の文字列を入力します。何も入力しない場合は自動で文字列が設定されます。</td>
        </tr>
        <tr>
            <td>タイプ</td>
            <td>
            <ul>
            <li><b>静的</b></li>
            ユーザーを指定してグループを構成する場合に選択します。<br />
            静的グループの所属ユーザーは、ユーザーごとにグループに所属させたり、所属から外したりできます。<br />
            <li><b>動的</b></li>
            指定した条件に該当するユーザーでグループを構成する場合に選択します。<br />
            役職を指定してグループを構成したり、複数の組織でひとつのグループを構成したりできます。<br />
            グループに所属するユーザーは、ユーザーに設定されている組織や役職などに応じて変わります。<br />
            <a href="/general/ja/admin/list_useradmin/list_group/query.html">動的グループの抽出条件について</a>
            </ul>
            </td>
        </tr>
        <tr>
            <td>説明</td>
            <td>グループ（ロール）の説明を入力します。<br />
            この説明は、「{{%slash%}}共通管理」画面以外では閲覧できません。</td>
        </tr>
    </tbody>
</table>

{{% enabled JP CN %}}
{{% note %}}
Garoonには、「静的グループ」のみが反映されます。  
またGaroonでは、静的グループは「ロール」として扱われます。  
[ロールとは（クラウド版 Garoon ヘルプ）](/g/ja/admin/system/users/role/whats_role.html)
{{% /note %}}
{{% /enabled %}}
