---
title: "ログイン画面をカスタマイズする"
weight: 200
---
{{% enabled JP %}}
ログイン画面に表示する会社名や背景画像を変更できます。初期状態では、{{%store%}}で登録した会社名が表示されます。
{{% /enabled %}}

{{% enabled CN %}}
ログイン画面に表示するタイトルや背景画像を変更できます。初期状態では、申し込み時に登録した会社名が表示されます。
{{% /enabled %}}

{{% enabled US %}}
ログイン画面に表示する会社名や背景画像を変更できます。初期状態で表示される内容は、ご利用環境のドメインにより異なります。

* **[AWSへの移行](https://www.kintone.com/aws-migration/)が完了していないお客様**（[ドメインID](/general/ja/admin/list_old/domainid.html)が「c」で始まるお客様）  
  {{%store%}}で登録した会社名が表示されます。
* **[AWSへの移行](https://www.kintone.com/aws-migration/)が完了したお客様**（[ドメインID](/general/ja/admin/list_old/domainid.html)が「y」で始まるお客様）  
  何も表示しません。
{{% /enabled %}}

1. 「{{%slash%}}共通管理」画面の「カスタマイズ」の[ログインページ]をクリックします。
  {{< screen src="/general/img-ja/loginSetting_img01.png"  alt="[ログインページ]が赤枠で囲まれた画像">}}
1. 会社名や背景画像を設定します。
   * <b>会社名を変更する場合</b>  
     [タイトル]に変更後の会社名を記載します。何も表示しない場合は空欄にします。
   * <b>背景画像を変更する場合</b>  
     [参照]をクリックして画像ファイルを設定します。  
     使用できる画像ファイルのサイズは、最大で5MBです。  
     登録した背景画像は、ユーザーのモニターのサイズに合わせて拡大または縮小されて表示されます。  
     鮮明な画像を表示するには、できるだけ縦横のサイズが大きい画像を登録します。ただし、画像ファイルの横幅が2,048pxを超える場合は、縦横比を維持した状態で、画像が縮小されます。  
     背景画像に使用できるファイルの形式は次のとおりです。
      * gif
      * jpeg
      * jpg
      * png
      * bmp
  
    {{< screen src="/general/img-ja/loginSetting_img02.png"  alt="ログインページの設定画面">}}

1. [保存]をクリックします。
    {{< screen src="/general/img-ja/loginSetting_img03.png"  alt="[保存]が赤枠で囲まれた画像">}}

{{% enabled JP %}}
{{% note %}}
{{%slash%}}共通管理の「ログインページの設定」画面でタイトルを変更しても、{{%store%}}に登録された会社名は変更されません。  
[{{%store%}}](https://store.cybozu.com/login)にログインし、「会社情報」を編集します。
{{% /note %}}
{{% /enabled %}}

{{% enabled US %}}
{{% note %}}
{{%slash%}}共通管理の「ログインページの設定」画面でタイトルを変更しても、購入時に登録された会社名は変更されません。  
購入時に登録された会社名を変更する手順は、下記を確認してください。  

* **[AWSへの移行](https://www.kintone.com/aws-migration/)が完了していないお客様**（[ドメインID](/general/ja/admin/list_old/domainid.html)が「c」で始まるお客様）  
  [{{%store%}}](https://store.kintone.com/login)にログインし、「Profile」を編集します。
* **[AWSへの移行](https://www.kintone.com/aws-migration/)が完了したお客様**（[ドメインID](/general/ja/admin/list_old/domainid.html)が「y」で始まるお客様）  
  {{%slash%}}共通管理画面から変更できます。次のページの手順にしたがって購入状況を確認し、契約内容が表示されたページの「Contact Information」でCompany Nameを変更してください。  
  [契約内容を確認する](/store/ja/contract/confirm.html)

{{% /note %}}
{{% /enabled %}}
