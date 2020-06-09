---
title: "配信メールの宛先"
weight: 300
disabled: [US,CN]
---

## 配信先 {#list_notice_mail_address_10}

下記の宛先に、配信メールが送信されます。  

### {{%store%}}に登録している宛先 {#list_notice_mail_address_1010}

* **管理者のメールアドレス**  
  {{< screen src="/general/img-ja/list_notice_mail_img01.png"  alt="">}}
* **「ご連絡先」に登録されているメールアドレス**  
  {{< screen src="/general/img-ja/list_notice_mail_img02.png"  alt="">}}
* **「ご請求先」に登録されているメールアドレス**  
  {{< screen src="/general/img-ja/list_notice_mail_img08.png"  alt="キャプチャ待ち">}}
  「ご請求先」の情報が「ご連絡先」と同じ場合は下記のように表示されます。  
  {{< screen src="/general/img-ja/list_notice_mail_img03.png"  alt="">}}

### {{%service%}}に登録している宛先 {#list_notice_mail_address_1020}

* **{{%slash%}}共通管理者のメールアドレス**
  {{< screen src="/general/img-ja/list_notice_mail_img04.png"  alt="">}}
  {{< screen src="/general/img-ja/list_notice_mail_img05.png"  alt="">}}

## 配信先の変更方法 {#list_notice_mail_address_20}

### {{%store%}}に登録しているメールアドレスを変更する {#list_notice_mail_address_2010}

1. {{%store%}}の管理者で、[{{%store%}}](https://store.{{%cybozu_com%}}/login)にログインします。  
  ログインできない場合は、[{{%store%}}にログインできません。](/general/ja/login/store_account.html)を参照してください。  
1. 変更したい宛先に応じて、次の操作をします。  
    1. **「ご連絡先」や「ご請求先」のメールアドレスを変更する場合**  
      「ご連絡先」と「ご請求先」には、それぞれ1つのみメールアドレスを設定できます。
        1. 左ナビの[会社情報]をクリックします。
        1. [変更]をクリックします。
        1. メールアドレスを変更し、[保存]をクリックします。
    1. **新しい管理者を追加する場合**  
        1. 左ナビの[アカウント設定]をクリックします。
        1. [管理者の追加]をクリックします。
        1. 新しい管理者のメールアドレスを入力し、[追加]をクリックします。
        1. 新しい管理者に、メール通知を確認する旨を連絡します。
    1. **既存の管理者のメールアドレスを変更する場合**  
      新しいメールアドレスを追加し、古いメールアドレスを削除します。  
      自分のメールアドレスを変更する場合は、他の管理者に操作を依頼してください。  
        1. 左ナビの[アカウント設定]をクリックします。
        1. [管理者の追加]をクリックします。
        1. 新しい管理者のメールアドレスを入力し、[追加]をクリックします。
        1. メールアドレスの変更を依頼した管理者に、メール通知を確認する旨を連絡します。
        1. 古いメールアドレスの右横にある[削除]をクリックします。
        1. 削除対象を確認し、[削除する]をクリックします。

#### エラーが表示され、メールアドレスの登録や変更ができない場合 {#list_notice_mail_address_201010}

次のエラーメッセージは、過去にサービスの試用や契約経験があるなどで、該当のメールアドレスを、別の{{%store%}}で利用中であることを示します。  
{{< screen src="/general/img-ja/list_notice_mail_img07.png"  alt="エラーメッセージの画像">}}

1つのメールアドレスを、複数の{{%store%}}で使いまわすことはできません。  
上記のエラーメッセージが表示された場合は、次のどちらかの対処をしてください。  

* 別のメールアドレスを{{%store%}}に登録する
* 過去に利用していた{{%store%}}アカウントから自分のアカウントを削除し、運用中の{{%store%}}に再度メールアドレスを登録する  
  詳細は、[自分のアカウントを削除する場合](/general/ja/admin/list_administrator/list_type_of_administrator/store_admin_del.html#list_type_of_administrator_store_admin_del_10)を参照してください。

### {{%slash%}}共通管理者のメールアドレスを変更する {#list_notice_mail_address_2020}

{{%slash%}}共通管理者のユーザー情報に登録されているメールアドレスを変更します。  

1. 必要に応じて、各サービスのメール通知の設定を確認します。  
  ユーザー情報に登録されているメールアドレスは、各サービスのメール通知にも利用されます。このため、メールアドレスを変更すると、メール通知の宛先も変わります。
    * {{%kintone%}}：[メール通知を有効にする](/k/ja/admin/system_customization/enable_mail_notification.html)
    * Garoon：[メール通知を利用できるまでの流れ](/g/ja/admin/system/external/notify_flow)
    * サイボウズ Office：[通知対象と通知先を設定する](/ja/o/user/per/p03/n_mail.html#user_per_p03_n_mail_04)
    * メールワイズ：[メール通知を受信する](https://manual.cybozu.co.jp/mailwise_cloud/user/personal.html#anchor08)
1. {{%slash%}}共通管理者のアカウントで、「https://（サブドメイン名）.{{%cybozu_com%}}/」にログインします。
1. [{{%slash%}}共通管理]をクリックします。
1. 「ユーザー管理」の[組織/ユーザー]をクリックします。
1. 検索ボックスに、メールアドレスを変更したい管理者の表示名またはログイン名を入力して検索します。
1. 目的のユーザーの![編集アイコン](/general/img/slash_edit_icon.png)をクリックします。
1. メールアドレスを変更し、[保存]をクリックします。
