---
title: "{{%slash%}}共通管理者の設定"
weight: 400
---
{{%slash%}}共通管理者に設定されているユーザーの確認方法と、追加・削除・変更する手順を説明します。  

{{%slash%}}共通管理者は、ユーザーの追加や編集、パスワードポリシーの設定などを行います。  
初期状態では、{{%service%}}環境を作成したときに登録したメールアドレスとパスワードを使ってログインし、{{%slash%}}共通管理にアクセスできます。

{{% disabled CN %}}
{{% note %}}
{{% subtitle %}}
2014年11月以前に{{%service%}}環境を作成した場合
{{% /subtitle %}}
初期状態では、Administratorアカウントを使用して{{%slash%}}共通管理にアクセスできます。
{{% /note %}}
{{% /disabled %}}

## {{%slash%}}共通管理者に設定されているユーザーを確認する{#list_type_of_administrator_list_domain_auth10}

{{% enabled JP %}}

1. 「https://（サブドメイン名）.{{%cybozu_com%}}/」にアクセスします。  
  ログインできない場合は、[管理者がアカウントやパスワードを忘れた場合](/general/ja/login/admin_account.html)を参照してください。
1. 「{{%slash%}}共通管理」画面の「ユーザー管理」の、[管理者の設定]をクリックします。
  {{< screen src="/general/img-ja/list_domain_auth_img01.png"  alt="画像">}}
  「共通管理者」欄で、管理者に設定されているユーザーを確認できます。  
  {{< screen src="/general/img-ja/list_domain_auth_img02.png"  alt="画像">}}

{{% /enabled %}}

{{% enabled US %}}

1. 「https://（サブドメイン名）.{{%cybozu_com%}}/」にアクセスします。  
  ログインできない場合は、[管理者がアカウントやパスワードを忘れた場合](/general/ja/login/admin_account.html)を参照してください。
1. 「{{%slash%}}共通管理」画面の「ユーザー管理」の、[管理者の設定]をクリックします。
  {{< screen src="/general/img-ja/list_domain_auth_img01_us.png"  alt="画像">}}
  「共通管理者」欄で、管理者に設定されているユーザーを確認できます。  
  {{< screen src="/general/img-ja/list_domain_auth_img02_us.png"  alt="画像">}}

{{% /enabled %}}

{{% enabled CN %}}

1. 「https://（サブドメイン名）.{{%cybozu_com%}}/」にアクセスします。  
  ログインできない場合は、[管理者がアカウントやパスワードを忘れた場合](/general/ja/login/admin_account.html)を参照してください。  
1. 「{{%slash%}}共通管理」画面の「ユーザー管理」の、[管理者の設定]をクリックします。
  {{< screen src="/general/img-ja/list_domain_auth_img01.png"  alt="画像">}}
  「共通管理者」欄で、管理者に設定されているユーザーを確認できます。  
  {{< screen src="/general/img-ja/list_domain_auth_img02.png"  alt="画像">}}

{{% /enabled %}}

## {{%slash%}}共通管理者を追加・削除・変更する{#list_type_of_administrator_list_domain_auth20}

{{%slash%}}共通管理者を変更する場合は、次の手順で「共通管理者」欄のユーザーを追加または削除します。

{{% enabled JP %}}

1. [{{%slash%}}共通管理者に設定されているユーザーを確認](#list_type_of_administrator_list_domain_auth10)します。
1. 「共通管理者」欄のユーザーを追加または削除して、{{%slash%}}共通管理者を変更します。  
  
   * <b>追加する場合</b>  
     1. {{%slash%}}共通管理者にユーザーを追加する場合は、「すべての組織」欄で該当のユーザーを含む組織を選択し、ユーザーを選択します。  
       ユーザーは複数選択できます。{{%slash%}}共通管理者に設定するユーザーは、あらかじめ{{%service%}}を利用するユーザーとして登録しておく必要があります。  
     1. [追加&gt;]をクリックして、「共通管理者」欄にユーザーを追加します。  
      {{< screen src="/general/img-ja/list_domain_auth_img03.png"  alt="画像">}}
   * <b>削除する場合</b>  
     {{%slash%}}共通管理者からユーザーを削除する場合は、「共通管理者」欄でユーザーを選択し、[&lt;解除]をクリックします。  
     Administratorユーザーは{{%slash%}}共通管理者から削除できません。
     {{< screen src="/general/img-ja/list_domain_auth_img04.png"  alt="画像">}}

1. {{%service%}}のメンテナンス情報などをメールで受け取る管理者のチェックボックスを選択します。  
  メールを受け取らない場合は、チェックボックスの選択を外します。  
  {{< screen src="/general/img-ja/list_domain_auth_img05.png"  alt="画像">}}
  配信メールに関する設定は、いつでも変更できます。    
  詳細は、[{{%CorpName%}}からのお知らせ／配信メール](/general/ja/admin/list_notice.html)を参照してください。
1. [保存]をクリックします。  

{{% /enabled %}}

{{% enabled US %}}

1. [{{%slash%}}共通管理者に設定されているユーザーを確認](#list_type_of_administrator_list_domain_auth10)します。
1. 「共通管理者」欄のユーザーを追加または削除して、{{%slash%}}共通管理者を変更します。  
  
  * <b>追加する場合</b>  
     1. {{%slash%}}共通管理者にユーザーを追加する場合は、「すべての組織」欄で該当のユーザーを含む組織を選択し、ユーザーを選択します。  
        ユーザーは複数選択できます。{{%slash%}}共通管理者に設定するユーザーは、あらかじめ{{%service%}}を利用するユーザーとして登録しておく必要があります。  
     1. [追加&gt;]をクリックして、「共通管理者」欄にユーザーを追加します。  
      {{< screen src="/general/img-ja/list_domain_auth_img03_us.png"  alt="画像">}}
  * <b>削除する場合</b>  
    {{%slash%}}共通管理者からユーザーを削除する場合は、「共通管理者」欄でユーザーを選択し、[&lt;解除]をクリックします。  
     Administratorユーザーは{{%slash%}}共通管理者から削除できません。
     {{< screen src="/general/img-ja/list_domain_auth_img04_us.png"  alt="画像">}}

1. [保存]をクリックします。 

{{% /enabled %}}

{{% enabled CN %}}

1. [{{%slash%}}共通管理者に設定されているユーザーを確認](#list_type_of_administrator_list_domain_auth10)します。
1. 「共通管理者」欄のユーザーを追加または削除して、{{%slash%}}共通管理者を変更します。  
  
  * <b>追加する場合</b>  
     1. {{%slash%}}共通管理者にユーザーを追加する場合は、「すべての組織」欄で該当のユーザーを含む組織を選択し、ユーザーを選択します。  
       ユーザーは複数選択できます。{{%slash%}}共通管理者に設定するユーザーは、あらかじめ{{%service%}}を利用するユーザーとして登録しておく必要があります。  
     1. [追加&gt;]をクリックして、「共通管理者」欄にユーザーを追加します。  
      {{< screen src="/general/img-ja/list_domain_auth_img03.png"  alt="画像">}}
  * <b>削除する場合</b>  
    {{%slash%}}共通管理者からユーザーを削除する場合は、「共通管理者」欄でユーザーを選択し、[&lt;解除]をクリックします。  
     Administratorユーザーは{{%slash%}}共通管理者から削除できません。
     {{< screen src="/general/img-ja/list_domain_auth_img04.png"  alt="画像">}}

1. {{%service%}}のメンテナンス情報などをメールで受け取る管理者のチェックボックスを選択します。  
  メールを受け取らない場合は、チェックボックスの選択を外します。  
   {{< screen src="/general/img-ja/list_domain_auth_img05.png"  alt="画像">}}
1. [保存]をクリックします。  

{{% /enabled %}}

{{< seealso title="関連する記事" >}}
[管理者の種類](/general/ja/admin/list_administrator/list_type_of_administrator/administrator.html)
{{< /seealso >}}
