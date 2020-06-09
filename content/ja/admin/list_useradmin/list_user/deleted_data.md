---
title: "ユーザーを削除した場合に削除されるデータについて"
weight: 800
---
{{%slash%}}共通管理でユーザーを削除すると、各製品で下記のデータが削除されます。  
削除の取り消し、削除したユーザーおよびデータの復旧はできません。  

ユーザーの休職や出向などで、一時的に{{%service%}}の利用を停止する場合は、該当のユーザーを削除ではなく使用停止にすることをおすすめします。  
使用停止にしたユーザーは{{%service%}}にログインできなくなります。また、サービスの利用ユーザー数にカウントされません。  
各操作手順の詳細は、次のページを参照してください。  

* [ユーザーを使用停止にする](/general/ja/admin/list_useradmin/list_user/stop_user.html#list_user_stop_user_10)
* [ユーザーを削除する](/general/ja/admin/list_useradmin/list_user/delete_user.html)  

## {{%kintone%}}

ユーザーの削除時に、そのユーザーに紐づくデータもあわせて削除されます。  
削除したユーザーのピープルは閲覧できません。そのため、削除したユーザーとのメッセージや、ピープルに書き込まれたコメントや添付ファイルは閲覧できなくなります。  
[削除したユーザーのデータは消えますか？](/k/ja/admin/admin_faq/deleted_user.html)

{{% enabled JP %}}

## サイボウズ Office

ユーザーの削除時に、そのユーザーに紐づくデータもあわせて削除されます。  
削除されるサイボウズ Officeのデータについては、次のページを参照してください。  
[ユーザーを削除した場合に、削除されるデータと残るデータを教えてください。](https://faq.cybozu.info/alphascope/cybozu/web/office/Detail.aspx?id=1697)

削除されるデータであっても、ファイルの入出力に対応しているデータであれば、ユーザーを削除する前にバックアップを取得できます。  
詳細は、[ファイルの入出力一覧](/ja/o/admin/spec/input_output/)を参照してください。

{{% /enabled %}}

{{% enabled JP CN %}}

## Garoon

ユーザーの削除時に、そのユーザーに紐づくデータもあわせて削除されます。  
削除されるGaroonのデータについては、Garoonヘルプの次のページを参照してください。  
[削除されたユーザーに関するデータの処理](/g/ja/admin/system/users/user/user_delete.html#admin_system_users_user_user_delete_01)

削除されるデータであっても、ファイルの入出力に対応しているデータであれば、ユーザーを削除する前にバックアップを取得できます。  
詳細は、[ファイルの入出力一覧](/g/ja/admin/spec/io/)を参照してください。

{{% /enabled %}}

{{% enabled JP %}}

## メールワイズ

ユーザーの削除時に、そのユーザーに紐づくデータもあわせて削除されます。  
ただし、メールデータやメールに関連した履歴やコメント、およびメール情報などは残ります。  
[ユーザーを削除すると、担当していたメールは削除されますか？](https://faq.cybozu.info/alphascope/cybozu/web/mailwise/Detail.aspx?id=390)

{{% /enabled %}}
