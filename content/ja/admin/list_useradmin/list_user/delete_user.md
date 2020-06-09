---
title: "ユーザーを削除する"
weight: 900
---

{{%slash%}}共通管理からユーザーを削除します。  
ユーザーを削除すると、利用中のすべてのサービスから、指定したユーザーが削除されます。  
また、ユーザーの削除時に、そのユーザーに紐づくデータもあわせて削除されます。復旧はできません。  

## こんなときは {#list_user_delete_user_10}

### 休職や出向などで、{{%service%}}に長期間ログインしないユーザーがいる場合 {#list_user_delete_user_1010}

休職や出向などで、ユーザーが{{%service%}}に長期間ログインしない場合は、該当のユーザーを削除せず、一時的に使用停止にすることをおすすめします。  
使用停止にしたユーザーは{{%service%}}にログインできなくなります。また、サービスの利用ユーザー数にカウントされません。

* **例：契約ユーザー数が50名で、ステータスが「使用中」のユーザーが48名の場合**  
  この時点では、2名分の空席が{{%service%}}にあります。  
  翌週、ユーザーAとユーザーBの休職に伴い、2人のステータスを使用停止にすると、ステータスが「使用中」のユーザーは46名に減ります。  
  これにより、4名分の空席が{{%service%}}にできます。  

復職時には、ユーザーのステータスを使用停止から使用中に変更するだけで、{{%service%}}にアクセスできるようになります。  
詳細は、[ユーザーを使用停止にする／使用を再開する](/general/ja/admin/list_useradmin/list_user/stop_user.html)を参照してください。  

### 退職や部署移動などで、{{%service%}}へのアクセスを禁止したいユーザーがいる場合 {#list_user_delete_user_1020}

{{%service%}}へのアクセスを禁止したい場合にも、該当のユーザーを削除せず、一時的に使用停止にすることをおすすめします。  
使用停止にしたユーザーは{{%service%}}にログインできなくなります。また、サービスの利用ユーザー数にカウントされません。  

先にユーザーを使用停止にしたあと、[ユーザーを削除した場合に削除されるデータ](/general/ja/admin/list_useradmin/list_user/deleted_data.html)を確認してから、必要に応じてユーザーを削除してください。

{{% enabled JP CN %}}

### 特定のサービスからユーザーを削除したい {#list_user_delete_user_1030}

部署移動などで特定のサービスだけを使用しなくなった場合は、ユーザーが利用するサービスを変更します。  
たとえば、ユーザーCの利用サービスを、{{%kintone%}}とGaroonの2つから、{{%kintone%}}だけに変更するといった運用ができます。  
詳細は、[ユーザーが利用するサービスを設定する](/general/ja/admin/list_useradmin/list_user/service_user.html)を参照してください。  

{{% /enabled %}}

### 契約ユーザー数を減らしたい {#list_user_delete_user_1040}

契約ユーザー数を減らすには、次の両方の作業が必要です。  

* **{{%service%}}を利用しないユーザーのステータスを「使用中止」に変更する**  
  ステータスが「使用停止」のユーザーは、契約ユーザーにカウントされません。  
* **契約ユーザー数を変更する**  
  利用ユーザー数（ステータスが「使用中」のユーザー）を減らしたり、ユーザーを削除したりするだけでは、契約ユーザー数は変わりません。{{%cybozu_com%}}の課金は、契約ユーザー数を基準にします。  

{{% enabled JP %}}

1. {{%service%}}を利用しないユーザーのステータスを「使用中止」に変更します。  
  詳細は、[ユーザーを使用停止にする](/general/ja/admin/list_useradmin/list_user/stop_user.html#list_user_stop_user_10)を参照してください。  
    * **例：契約ユーザー数を50名から40名に変更したい場合：**  
      この時点では、利用ユーザー数が50名とします。  
      契約ユーザー数を40名に減らすには、最低でも10名分のステータスを「使用停止」にし、利用ユーザー数を40名以下にする必要があります。  

1. 契約内容を変更します。  
  詳細は、[「購入方法」の「ユーザー数の追加など、契約内容を変更する」](https://www.cybozu.com/jp/buy/add/)を参照してください。

1. 必要に応じて、使用停止にしているユーザーを削除します。  
  ステータスが「使用停止」のユーザーは、契約ユーザーにカウントされません。ユーザーを削除しなくても、運用に支障ありません。  

    * [ユーザーを個別に削除する](#list_user_delete_user_20)
    * [複数のユーザーを一括削除する](#list_user_delete_user_30)

{{% /enabled %}}

{{% enabled US %}}

1. {{%service%}}を利用しないユーザーのステータスを「使用中止」に変更します。  
  詳細は、[ユーザーを使用停止にする](/general/ja/admin/list_useradmin/list_user/stop_user.html#list_user_stop_user_10)を参照してください。  
    * **例：契約ユーザー数を50名から40名に変更したい場合：**  
      この時点では、利用ユーザー数が50名とします。  
      契約ユーザー数を40名に減らすには、最低でも10名分のステータスを「使用停止」にし、利用ユーザー数を40名以下にする必要があります。  

1. 契約内容を変更します。  

    * **[AWSへの移行](https://www.kintone.com/aws-migration/)が完了していないお客様**（[ドメインID](/general/ja/admin/list_old/domainid.html)が「c」で始まるお客様）  
      [{{%store%}}](https://store.kintone.com/login)で契約内容を変更してください。
    * **[AWSへの移行](https://www.kintone.com/aws-migration/)が完了したお客様**（[ドメインID](/general/ja/admin/list_old/domainid.html)が「y」で始まるお客様）  
      {{%slash%}}共通管理画面から変更できます。詳細は、[契約ユーザー数を変更する](/store/ja/contract/users.html)を参照してください。  

1. 必要に応じて、使用停止にしているユーザーを削除します。  
  ステータスが「使用停止」のユーザーは、契約ユーザーにカウントされません。ユーザーを削除しなくても、運用に支障ありません。  

    * [ユーザーを個別に削除する](#list_user_delete_user_20)
    * [複数のユーザーを一括削除する](#list_user_delete_user_30)

{{% /enabled %}}

{{% enabled CN %}}

1. {{%service%}}を利用しないユーザーのステータスを「使用中止」に変更します。  
  詳細は、[ユーザーを使用停止にする](/general/ja/admin/list_useradmin/list_user/stop_user.html#list_user_stop_user_10)を参照してください。  
    * **例：契約ユーザー数を50名から40名に変更したい場合：**  
      この時点では、利用ユーザー数が50名とします。  
      契約ユーザー数を40名に減らすには、最低でも10名分のステータスを「使用停止」にし、利用ユーザー数を40名以下にする必要があります。  

1. 契約内容を変更する旨を{{%CorpName%}}に連絡します。  
  詳細は、[お問い合わせ方法](/general/ja/admin/support.html)を参照してください。

1. 必要に応じて、使用停止にしているユーザーを削除します。  
  ステータスが「使用停止」のユーザーは、契約ユーザーにカウントされません。ユーザーを削除しなくても、運用に支障ありません。  

    * [ユーザーを個別に削除する](#list_user_delete_user_20)
    * [複数のユーザーを一括削除する](#list_user_delete_user_30)

{{% /enabled %}}

## ユーザーを個別に削除する {#list_user_delete_user_20}

{{% warning %}}

* 削除の取り消し、削除したユーザーおよびデータの復旧はできません。  
* Administratorは削除できません。

{{% /warning %}}

{{% enabled JP %}}

1. [ユーザーを削除した場合に削除されるデータ](/general/ja/admin/list_useradmin/list_user/deleted_data.html)を確認します。  
  ユーザーを削除しても問題ない場合は、手順2に進みます。  
  ユーザーを削除せずに、{{%service%}}へのアクセスを禁止する場合は、[ユーザーを使用停止にする](/general/ja/admin/list_useradmin/list_user/stop_user.html#list_user_stop_user_10)に進みます。  

1. {{%slash%}}共通管理画面の「ユーザー管理」の、[組織/ユーザー]をクリックします。  
   {{< screen src="/general/img-ja/delete_user_img01.png"  alt="[組織/ユーザー]が赤枠で囲まれた画像">}}

1. 組織を選択し、削除するユーザーの ![画像](/general/img/slash_edit_icon.png) をクリックします。  
   {{< screen src="/general/img-ja/delete_user_img02.png"  alt="組織とユーザーを選択する画像">}}

1. [このユーザーの削除]をクリックします。  
   {{< screen src="/general/img-ja/delete_user_img03.png"  alt="[このユーザーの削除]が赤枠で囲まれた画像">}}

1. 確認画面で[ユーザーを削除]をクリックします。  
   {{< screen src="/general/img-ja/delete_user_img04.png"  alt="ダイアログの画像">}}

{{% /enabled %}}

{{% enabled US %}}

1. [削除したユーザーのデータは消えますか？](/k/ja/admin/admin_faq/deleted_user.html)を確認します。  
  ユーザーを削除しても問題ない場合は、手順2に進みます。  
  ユーザーを削除せずに、{{%service%}}へのアクセスを禁止する場合は、[ユーザーを使用停止にする](/general/ja/admin/list_useradmin/list_user/stop_user.html#list_user_stop_user_10)に進みます。  

1. {{%slash%}}共通管理画面の「ユーザー管理」の、[組織/ユーザー]をクリックします。  
   {{< screen src="/general/img-ja/delete_user_img01.png"  alt="[組織/ユーザー]が赤枠で囲まれた画像">}}

1. 組織を選択し、削除するユーザーの ![画像](/general/img/slash_edit_icon.png) をクリックします。  
   {{< screen src="/general/img-ja/delete_user_img02.png"  alt="組織とユーザーを選択する画像">}}

1. [このユーザーの削除]をクリックします。  
   {{< screen src="/general/img-ja/delete_user_img03.png"  alt="[このユーザーの削除]が赤枠で囲まれた画像">}}

1. 確認画面で[ユーザーを削除]をクリックします。  
   {{< screen src="/general/img-ja/delete_user_img04.png"  alt="「このユーザーの削除」ダイアログの画像">}}

{{% /enabled %}}

{{% enabled CN %}}

1. [ユーザーを削除した場合に削除されるデータ](/general/ja/admin/list_useradmin/list_user/deleted_data.html)を確認します。  
  ユーザーを削除しても問題ない場合は、手順2に進みます。  
  ユーザーを削除せずに、{{%service%}}へのアクセスを禁止する場合は、[ユーザーを使用停止にする](/general/ja/admin/list_useradmin/list_user/stop_user.html#list_user_stop_user_10)に進みます。  

1. {{%slash%}}共通管理画面の「ユーザー管理」の、[組織/ユーザー]をクリックします。  
   {{< screen src="/general/img-ja/delete_user_img01.png"  alt="[組織/ユーザー]が赤枠で囲まれた画像">}}

1. 組織を選択し、削除するユーザーの ![画像](/general/img/slash_edit_icon.png) をクリックします。  
   {{< screen src="/general/img-ja/delete_user_img02.png"  alt="組織とユーザーを選択する画像">}}

1. [このユーザーの削除]をクリックします。  
   {{< screen src="/general/img-ja/delete_user_img03.png"  alt="[このユーザーの削除]が赤枠で囲まれた画像">}}

1. 確認画面で[ユーザーを削除]をクリックします。  
   {{< screen src="/general/img-ja/delete_user_img04.png"  alt="「このユーザーの削除」ダイアログの画像">}}

{{% /enabled %}}

## 複数のユーザーを一括削除する {#list_user_delete_user_30}

{{% warning %}}

* 削除の取り消し、削除したユーザーおよびデータの復旧はできません。  
* Administratorは削除できません。

{{% /warning %}}

{{% enabled JP %}}

1. [ユーザーを削除した場合に削除されるデータ](/general/ja/admin/list_useradmin/list_user/deleted_data.html)を確認します。  
  ユーザーを削除しても問題ない場合は、手順2に進みます。  
  ユーザーを削除せずに、{{%service%}}へのアクセスを禁止する場合は、[ユーザーを使用停止にする](/general/ja/admin/list_useradmin/list_user/stop_user.html#list_user_stop_user_10)に進みます。  

1. {{%slash%}}共通管理画面の「ユーザー管理」の、[ユーザーの一括削除]をクリックします。  
   {{< screen src="/general/img-ja/delete_user_img05.png"  alt="[ユーザーの一括削除]が赤枠で囲まれた画像">}}

1. 組織を選択し、削除するユーザーを選択します。
  ユーザーは複数選択できます。  

1. [追加&gt;]をクリックして、「削除するユーザー」にユーザーを追加します。  
   {{< screen src="/general/img-ja/delete_user_img06.png"  alt="ユーザーを複数選択して「削除するユーザー」にユーザーを追加する画像">}}

1. [削除]をクリックします。
   {{< screen src="/general/img-ja/delete_user_img07.png"  alt="[削除]が赤枠で囲まれた画像">}}

1. 確認画面で[ユーザーを削除]をクリックします。  
   {{< screen src="/general/img-ja/delete_user_img08.png"  alt="「ユーザーの削除」ダイアログの画像">}}

{{% /enabled %}}

{{% enabled US %}}

1. [削除したユーザーのデータは消えますか？](/k/ja/admin/admin_faq/deleted_user.html)を確認します。  
  ユーザーを削除しても問題ない場合は、手順2に進みます。  
  ユーザーを削除せずに、{{%service%}}へのアクセスを禁止する場合は、[ユーザーを使用停止にする](/general/ja/admin/list_useradmin/list_user/stop_user.html#list_user_stop_user_10)に進みます。  

1. {{%slash%}}共通管理画面の「ユーザー管理」の、[ユーザーの一括削除]をクリックします。  
   {{< screen src="/general/img-ja/delete_user_img05.png"  alt="[ユーザーの一括削除]が赤枠で囲まれた画像">}}

1. 組織を選択し、削除するユーザーを選択します。
  ユーザーは複数選択できます。  

1. [追加&gt;]をクリックして、「削除するユーザー」にユーザーを追加します。  
   {{< screen src="/general/img-ja/delete_user_img06.png"  alt="ユーザーを複数選択して「削除するユーザー」にユーザーを追加する画像">}}

1. [削除]をクリックします。
   {{< screen src="/general/img-ja/delete_user_img07.png"  alt="[削除]が赤枠で囲まれた画像">}}

1. 確認画面で[ユーザーを削除]をクリックします。  
   {{< screen src="/general/img-ja/delete_user_img08.png"  alt="「ユーザーの削除」ダイアログの画像">}}

{{% /enabled %}}

{{% enabled CN %}}

1. [ユーザーを削除した場合に削除されるデータ](/general/ja/admin/list_useradmin/list_user/deleted_data.html)を確認します。  
  ユーザーを削除しても問題ない場合は、手順2に進みます。  
  ユーザーを削除せずに、{{%service%}}へのアクセスを禁止する場合は、[ユーザーを使用停止にする](/general/ja/admin/list_useradmin/list_user/stop_user.html#list_user_stop_user_10)に進みます。  

1. {{%slash%}}共通管理画面の「ユーザー管理」の、[ユーザーの一括削除]をクリックします。  
   {{< screen src="/general/img-ja/delete_user_img05.png"  alt="[ユーザーの一括削除]が赤枠で囲まれた画像">}}

1. 組織を選択し、削除するユーザーを選択します。
  ユーザーは複数選択できます。  

1. [追加&gt;]をクリックして、「削除するユーザー」にユーザーを追加します。  
   {{< screen src="/general/img-ja/delete_user_img06.png"  alt="ユーザーを複数選択して「削除するユーザー」にユーザーを追加する画像">}}

1. [削除]をクリックします。
   {{< screen src="/general/img-ja/delete_user_img07.png"  alt="[削除]が赤枠で囲まれた画像">}}

1. 確認画面で[ユーザーを削除]をクリックします。  
   {{< screen src="/general/img-ja/delete_user_img08.png"  alt="「ユーザーの削除」ダイアログの画像">}}

{{% /enabled %}}
