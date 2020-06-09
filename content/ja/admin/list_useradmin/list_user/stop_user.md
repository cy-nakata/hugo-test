---
title: "ユーザーを使用停止にする／使用を再開する"
weight: 700
---
## ユーザーを使用停止にする{#list_user_stop_user_10}

ユーザーの退職や休職などによりサービスへのアクセスを禁止する場合に、ユーザー情報を削除せず、使用停止にできます。

使用停止中のユーザーは、次の状態になります。  

* サービスの利用ユーザーにカウントされません。
* サービスにログインできません。
* 使用停止にした段階で、発行済みのクライアント証明書は破棄されます。

{{% enabled JP %}}
{{% warning %}}
{{% subtitle %}}
ユーザーの使用停止と、契約ユーザー数の関係
{{% /subtitle %}}
ユーザーを使用停止にしただけでは、契約ユーザー数は変わりません。{{%cybozu_com%}}の課金は、{{%store%}}での契約ユーザー数を基準にします。契約ユーザー数を減らすには、{{%store%}}で契約内容を変更します。  
契約内容の変更方法は、「購入方法」の[ユーザー数の追加など、契約内容を変更する」](https://www.cybozu.com/jp/buy/add/)を参照してください。
{{% /warning %}}
{{% /enabled %}}

{{% enabled US %}}
{{% warning %}}
{{% subtitle %}}
ユーザーの使用停止と、契約ユーザー数の関係
{{% /subtitle %}}
ユーザーを使用停止にしただけでは、契約ユーザー数は変わりません。{{%cybozu_com%}}の課金は、契約ユーザー数を基準にします。  
契約内容の変更方法は、[契約内容の確認と変更](/store/en/contract.html)を参照してください。
{{% /warning %}}
{{% /enabled %}}

{{% enabled CN %}}
{{% warning %}}
{{% subtitle %}}
ユーザーの使用停止と、契約ユーザー数の関係
{{% /subtitle %}}
ユーザーを使用停止にしても、契約ユーザー数は変わりません。使用停止中のユーザーも、引き続き課金の対象になります。
{{% /warning %}}
{{% /enabled %}}

1. 「{{%slash%}}共通管理」画面の「ユーザー管理」の、[組織/ユーザー]をクリックします。  
  {{< screen src="/general/img-ja/stop_user_img01.png" alt="[組織/ユーザー]が赤枠で囲まれた画像">}}
1. 左側の一覧で組織を選択し、使用停止するユーザーの![アイコン](/general/img/slash_edit_icon.png)をクリックします。  
  {{< screen src="/general/img-ja/stop_user_img02.png" alt="組織とユーザーを選択する画像">}}
1. 使用状態の[使用中]をクリックし、[停止中]に変わったら、[保存]をクリックします。  
  {{< screen src="/general/img-ja/stop_user_img03.png" alt="使用状態を[停止中]に変更する画像">}}

{{% note %}}
{{% subtitle %}}
使用停止中のユーザーのプロフィール閲覧について
{{% /subtitle %}}
使用停止中のユーザーのプロフィールは、ほかのユーザーが閲覧できます。プロフィールを表示させないようにするには、次のどちらかの操作をします。

* ユーザー情報を編集して、不要な情報を削除する  
  [ユーザー情報を編集する](/general/ja/admin/list_useradmin/list_user/edit_user.html)
* ユーザーを完全に削除する  
  [ユーザーを削除する](/general/ja/admin/list_useradmin/list_user/delete_user.html)
{{% /note %}}

## ユーザーの使用を再開する{#list_user_stop_user_20}

使用停止中のユーザーの、使用を再開する手順は次のとおりです。

1. 「{{%slash%}}共通管理」画面の「ユーザー管理」の、[組織/ユーザー]をクリックします。  
  {{< screen src="/general/img-ja/stop_user_img01.png" alt="[組織/ユーザー]が赤枠で囲まれた画像">}}
1. 左側の一覧で組織を選択し、使用を再開するユーザーの![アイコン](/general/img/slash_edit_icon.png)をクリックします。  
  {{< screen src="/general/img-ja/stop_user_img02.png" alt="組織とユーザーを選択する画像">}}
1. 使用状態の[停止中]をクリックし、[使用中]に変わったら、[保存]をクリックします。  
  {{< screen src="/general/img-ja/stop_user_img04.png" alt="使用状態を[使用中]に変更する画像">}}

{{% disabled US %}}
{{% note %}}
{{% subtitle %}}使用停止にする前に、セキュアアクセスを使用していたユーザーの場合{{% /subtitle %}}
クライアント証明書が無効になっています。クライアント証明書を再発行する手順については、[クライアント証明書を発行する](/general/ja/admin/list_security/list_secureaccess/secureaccess.html#list_secureaccess_secureaccess_30)方法を参照してください。  
利用するスマートフォンやパソコンに、ユーザーがクライアント証明書を登録する方法については、[オフィス外からサービスにアクセスする](/general/ja/user/list_access/remote.html)方法を参照してください。  
{{% /note %}}
{{% /disabled %}}

{{% enabled US %}}
{{% note %}}
{{% subtitle %}}使用停止にする前に、セキュアアクセスを使用していたユーザーの場合{{% /subtitle %}}

* クライアント証明書が無効になっています。クライアント証明書を再発行する手順については、[クライアント証明書を発行する](/general/ja/admin/list_security/list_secureaccess/secureaccess.html#list_secureaccess_secureaccess_30)方法を参照してください。  
* 利用するスマートフォンやパソコンに、ユーザーがクライアント証明書を登録する方法については、[オフィス外からサービスにアクセスする](/general/ja/user/list_access/remote.html)方法を参照してください。  

なお、セキュアアクセスは、[AWSに移行](https://www.kintone.com/aws-migration/)したお客様（[ドメインID](/general/ja/admin/list_old/domainid.html)が「y」で始まるお客様）にはご利用いただけません。

{{% /note %}}
{{% /enabled %}}
