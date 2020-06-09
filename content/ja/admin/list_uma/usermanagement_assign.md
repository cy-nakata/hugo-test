---
title: "組織の管理者を設定する"
weight: 100
---
{{%slash%}}共通管理者が組織の管理者を設定する手順を説明します。

組織の管理者については、[組織の管理者とは](/general/ja/admin/list_administrator/list_type_of_administrator/whatisumaadmin.html)を参照してください。  
1つの組織に設定できる組織の管理者は1000人までです。  

{{% disabled US %}}
{{% warning %}}
{{% subtitle %}}
組織の管理者を設定できる条件
{{% /subtitle %}}
組織の管理者は、{{%kintone%}}、もしくはGaroonを契約している場合のみ設定できます。
{{% /warning %}}
{{% /disabled %}}

## 組織の管理者を設定する前に確認すること {#list_uma_usermanagement_assign_10}

組織の管理者は、自身が管理権限をもつ組織のユーザー以外に、組織に未所属のユーザーについても、ユーザー情報の編集や、自分が管理する組織への追加ができます。  

{{%slash%}}共通管理者は、組織の管理者を設定する前に、未所属ユーザーを事前に確認し、必要に応じて適切な組織に所属させてください。なお、初期状態では、Administratorユーザーも未所属ユーザーに含まれます。

## 組織の管理者の設定方法 {#list_uma_usermanagement_assign_20}

{{% note %}}
組織の管理者と{{%slash%}}共通管理者の管理画面は異なります。  
組織の管理者は、ユーザー管理の一部の機能しか利用できないため、それ以外の管理項目は表示されません。
{{< screen src="/general/img-ja/usermanagement_assign_jaJP_05.png"  alt="画像">}}
{{% /note %}}

1. {{%slash%}}共通管理画面で「ユーザー管理」の[組織/ユーザー]をクリックします。
  {{< screen src="/general/img-ja/usermanagement_assign_jaJP_01.png"  alt="画像">}}

1. 「組織とユーザーの設定」で、管理者を設定する組織の歯車アイコンにカーソルをあわせます。  
  リストの中から[組織の管理者の設定]をクリックします。  
  {{%slash%}}共通管理者はすべての組織に対して、組織の管理者を設定できます。
  {{< screen src="/general/img-ja/usermanagement_assign_jaJP_02.png"  alt="画像">}}

1. 「組織の管理者の設定」で、組織の管理者に設定したいユーザーが所属する組織を選択し、リストの中から管理者にするユーザーを選択し、[追加]をクリックします。  
  右側の「組織の管理者」欄に選択したユーザーが表示されます。  
  管理する組織に所属していないユーザーでも、管理者として設定できます。
  {{< screen src="/general/img-ja/usermanagement_assign_jaJP_03.png"  alt="画像">}}

1. [保存]をクリックし、設定を完了します。  
  組織の管理者がログインすると、{{%slash%}}共通管理にアクセスできるメニューが表示されます。  
  {{% enabled JP %}}
  {{< screen src="/general/img-ja/usermanagement_assign_ja_04.png"  alt="画像">}}  
  {{% /enabled %}}
  {{% enabled US %}}
  {{< screen src="/general/img-ja/usermanagement_assign_img04_us.png"  alt="画像">}}  
  {{% /enabled %}}
  {{% enabled CN %}}
  {{< screen src="/general/img-ja/usermanagement_assign_img04_cn.png"  alt="画像">}}  
  {{% /enabled %}}
