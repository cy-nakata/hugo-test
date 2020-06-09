---
title: "管理者のアカウントとパスワードの初期設定"
weight: 300
disabled: [US,CN]
---
{{%service%}}のサービスである{{%kintone%}}、サイボウズ Office、Garoon、またはメールワイズを初めて試用した際に、次の2つの管理者が作成されます。  

* <b>{{%store%}}管理者</b>  
  {{%service%}}の契約や、{{%service%}}へのアクセス制限の設定などを行う管理者
* <b>{{%slash%}}共通管理者</b>  
  ユーザーの追加や、クライアント証明書の発行など、{{%service%}}で各種設定業務を行う管理者

それぞれの管理者のログインアカウントとパスワードの初期値は、初めて試用した場合と、試用または契約後に新たにサービスを追加した場合で、次のように異なります。

## {{%service%}}のサービスを初めて試用した場合 {#list_administrator_admin_account_initial_10}

{{%store%}}管理者と{{%slash%}}共通管理者のログインアカウントとパスワードの初期値は次のとおりです。

<table width="100%">
<tbody>
    <tr>
        <th width="20%">ログインアカウント</th>
        <td width="80%">30日間無料お試しを申し込んだ際に登録したメールアドレス（{{%store%}}からのメールに掲載されています。）<br>
        <img src="/general/img-ja/admin_account_initial_img01.png" alt="メールアドレスを入力する画像" />
        </td>
    </tr>
    <tr>
        <th width="20%">パスワード</th>
        <td width="80%">30日間無料お試しを申し込んだ際に登録したパスワード<br>
        <img src="/general/img-ja/admin_account_initial_img02.png" alt="パスワードを入力する画像" />
        </td>
    </tr>
</tbody>
</table>

{{% note %}}
{{% subtitle %}}販売店（パートナー）を通して購入した場合{{% /subtitle %}}
{{%store%}}管理者と{{%slash%}}共通管理者のログインアカウントとパスワードは、受注手続きが完了したあとに設定します。詳細は、よくあるご質問（FAQ）の[販売店（パートナー）を通して購入しました。サービスを利用するにはどうしたらいいですか？](https://faq.cybozu.info/alphascope/cybozu/web/cybozu.com/Detail.aspx?id=1831)を参照してください。
{{% /note %}}

## {{%service%}}のサービスを既に試用または契約をしていて、新たにサービスを追加した場合 {#list_administrator_admin_account_initial_20}

{{%store%}}管理者のログインアカウントとパスワードに変更はありません。  
次のいずれかによって、{{%slash%}}共通管理者のパスワードが異なります。

| 追加方法|詳細      |
| ------------------------------------------------------------ | ---- |
| [新しいドメインで試用環境を申し込んだ場合](#list_administrator_admin_account_initial_2010) | 既に利用しているサービスとは別のドメインで、新たにサービスを試用した。 |
| [新しいドメインでサービスを発注した場合](#list_administrator_admin_account_initial_2020) | 既に利用しているサービスとは別のドメインで、新たにサービスを試用せずに発注した。 |
| [使用中のドメインに新しいサービスの試用を申し込んだ、または発注した場合](#list_administrator_admin_account_initial_2030) | 既に利用しているサービスと同じドメインで、別のサービスを試用または発注した。 |

### 新しいドメインで試用環境を申し込んだ場合 {#list_administrator_admin_account_initial_2010}

{{%slash%}}共通管理者のログインアカウントとパスワードの初期値は次のとおりです。

<table width="100%">
<tbody>
    <tr>
        <th width="20%">ログインアカウント</th>
        <td width="80%">ドメインを作成した{{%store%}}管理者のメールアドレス（{{%store%}}からのメールに掲載されています。）<br>
        </td>
    </tr>
    <tr>
        <th width="20%">パスワード</th>
        <td width="80%">サイボウズが発行するランダムなパスワード（{{%store%}}からのメールに掲載されています。）<br>
        <ul>
                <li>メールの件名は「[{{%service%}}]_サービスの準備ができました」です。</li>
                <li>メールの文面は変更される場合があります。</li>
            </ul>
        <img src="/general/img-ja/admin_account_initial_img03.png" alt="仮パスワードが記載されているメールの例" />
        </td>
    </tr>
</tbody>
</table>

### 新しいドメインでサービスを発注した場合 {#list_administrator_admin_account_initial_2020}

試用せずに発注した場合の、{{%slash%}}共通管理者のログインアカウントとパスワードの初期値は次のとおりです。

<table width="100%">
<tbody>
    <tr>
        <th width="20%">ログインアカウント</th>
        <td width="80%">ドメインを作成した{{%store%}}管理者のメールアドレス（{{%store%}}からのメールに掲載されています。）<br>
        </td>
    </tr>
    <tr>
        <th width="20%">パスワード</th>
        <td width="80%">発注時に入力する「ご利用環境のパスワード」（{{%store%}}からのメールには記載されませんので、注意して決定してください。）<br>
        <img src="/general/img-ja/admin_account_initial_img04.png" alt="ご利用環境のパスワードを入力する画像" />
        </td>
    </tr>
</tbody>
</table>

### 使用中のドメインに新しいサービスの試用を申し込んだ、または発注した場合 {#list_administrator_admin_account_initial_2030}

既に利用中の{{%slash%}}共通管理者のアカウントとパスワードで、ログインできます。
