---
title: "監査ログの情報をメールで送信する"
weight: 200
---
監査ログは、重要度（レベル）に応じて、指定したメールアドレスに通知メールを送信できます。  
通知メールを送信できるのは、{{%cybozu_com%}}の管理や基本操作に関する監査ログのみです。

{{% enabled JP %}}
{{%kintone%}}、Garoon、サイボウズ Officeなど各サービスのログは通知されません。  
{{% /enabled %}}

{{% enabled CN %}}
{{%kintone%}}、Garoonなど各サービスのログは通知されません。
{{% /enabled %}}  

{{%cybozu_com%}}の管理や基本操作に関する監査ログには、下記が該当します。  

* [{{%service%}}全般のログ](/general/ja/admin/list_systemadmin/list_audit/log/general.html)
* [ログインとログアウトに関するログ](/general/ja/admin/list_systemadmin/list_audit/log/login.html)
* [ユーザーに関するログ](/general/ja/admin/list_systemadmin/list_audit/log/user.html)
* [組織に関するログ](/general/ja/admin/list_systemadmin/list_audit/log/organization.html)
* [グループに関するログ](/general/ja/admin/list_systemadmin/list_audit/log/group.html)
* [役職に関するログ](/general/ja/admin/list_systemadmin/list_audit/log/title.html)
* [利用サービスに関するログ](/general/ja/admin/list_systemadmin/list_audit/log/service.html)
* [クライアント証明書に関するログ](/general/ja/admin/list_systemadmin/list_audit/log/remote.html)
* [データ移行に関するのログ](/general/ja/admin/list_systemadmin/list_audit/log/migration.html)
* [連携サービスの設定に関するログ](/general/ja/admin/list_systemadmin/list_audit/log/integration.html)

{{% disabled US %}}

* [組織の事前設定に関するログ](/general/ja/admin/list_systemadmin/list_audit/log/tentative_reorganization.html)

{{% /disabled %}}

1. {{%slash%}}共通管理画面の、「監査ログ」の[設定]をクリックします。
  {{< screen src="/general/img-ja/send_audit_img01.png"  alt="[設定]が赤枠で囲まれた画像">}}

1. 通知メールを送信したい重要度（レベル）のドロップダウンリストで、「メールを送信する」を選択します。  
  どのログがどの重要度（レベル）であるかは、[監査ログの一覧](/general/ja/admin/list_systemadmin/list_audit/log.html)を参照してください。  
  {{< screen src="/general/img-ja/send_audit_img02.png"  alt="メールを送信するかどうか選択する画像">}}

1. 宛先のメールアドレスを入力します。  
   複数のメールアドレスを設定する場合は、1行ずつ改行で区切って入力します。メールアドレスは15件まで指定できます。  
   「テストメールを送信する」のチェックボックスを選択すると、宛先のアドレスにテストメールを送信できます。
  {{< screen src="/general/img-ja/send_audit_img03.png"  alt="宛先のメールアドレスを入力する画像">}}

1. [保存]をクリックします。
