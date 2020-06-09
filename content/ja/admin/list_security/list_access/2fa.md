---
title: "2要素認証とは"
weight: 200
disabled: [JP,CN]
---

{{% enabled US %}}
{{% warning %}}
この記事は、[AWSに移行](https://www.kintone.com/aws-migration/)したお客様向けです。ドメインIDが「y」で始まるお客様が該当します。AWSへの移行が未完了のお客様は、[IPアドレス制限を設定する（AWSへの移行が未完了のお客様向け）](/general/ja/admin/list_old/ip_basic_old.html)をお読みください。  

ドメインIDを確認するには「[ドメインIDの確認方法](/general/ja/admin/list_old/domainid.html)」を参照してください。
{{% /warning %}}
{{% /enabled %}}

2要素認証とは、次の要素のうち、2つを組み合わせてユーザーの身元を確認する仕組みです。  

* ユーザーだけが知っていること
* ユーザーだけが所有しているもの
* ユーザー自身の特性（指紋や顔）

<br>
{{%service%}}の2要素認証では、「ユーザーだけが知っていること」と「ユーザーだけが所有しているもの」を使って認証します。  
IPアドレス制限は設定しないため、{{%service%}}にアクセスできる場所は限定されません。

<table>
<caption>認証の組み合わせ</caption>
  <tbody>
  <tr>
  <th width=200>ユーザーだけが知っていること</th>
  <th width=200>ユーザーだけが所有しているもの</th>
  </tr>
  <tr>
  <td>ユーザーのログイン名とパスワード</td>
  <td>モバイル端末にインストールした認証アプリの確認コード</td>
  </tr>
  </tbody>
</table>

{{< screen src="/general/img-ja/list_access_2fa_img01.png"  alt="">}}

## 2要素認証を利用する上で知っておくこと {#list_access_2fa_10}

2要素認証を有効にすると、社内から出張先からなどアクセスする場所にかかわらず、{{%service%}}へのログイン時は毎回、「ログイン名とパスワード」と「確認コード」の入力が求められます。  
**また、確認するコードは毎回新しいものに変わります。**  
このため、ログインするたびに、モバイル端末で確認コードを確認する必要があります。  

一見、わずらわしい操作のように見えますが、第三者がログインに必要な情報を特定しにくいようにするための仕組みです。安全にアクセスするための操作としてご理解ください。  

{{% warning %}}
2要素認証を有効にしたユーザーは、REST APIでパスワード認証を利用できません。  
別の認証方式（APIトークン、セッション認証、OAuth認証）を利用するか、2要素認証を無効にした別の連携用ユーザーを用意してください。
{{% /warning %}}

{{% reference %}}
<!-- * [2要素認証で制限したい](/general/ja/admin/list_security/2fa.html) -->

* [2要素認証を有効にする](/general/ja/user/list_personal/two_factor_authentication.html)
* [2要素認証の確認コードを入手するには](/general/ja/user/list_start/get_code.html)

{{% /reference %}}
