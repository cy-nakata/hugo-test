---
title: "監査ログの保存期間を設定する"
weight: 300
---

監査ログの保存期間は、6週間から10年間の間で指定できます。
お客様の運用に適した期間を設定してください。  

6週間以上前の監査ログはアーカイブされます。  
アーカイブ化された監査ログの確認方法は、[6週間以上前の監査ログ](/general/ja/admin/list_systemadmin/list_audit/download_audit.html#list_audit_download_audit_20)を参照してください。  

1. {{%slash%}}共通管理画面の、「監査ログ」の[設定]をクリックします。  
  {{< screen src="/general/img-ja/set_audit_img01.png"  alt="[設定]が赤枠で囲まれた画像">}}

1. 「保存期間」をプルダウンメニューから選択します。  
  初期値は3年間です。保存期間は、6週間から10年間の間で変更できます。
  {{< screen src="/general/img-ja/set_audit_img02.png"  alt="監査ログの保存期間を選択している画像">}}  
  下記の設定は、ログの重要度（レベル）に応じて、監査ログの情報をメールで通知する場合に利用します。  
  詳細は、[監査ログの情報をメールで送信する](/general/ja/admin/list_systemadmin/list_audit/send_audit.html)を参照してください。
  {{< screen src="/general/img-ja/set_audit_img03.png"  alt="監査ログの保存期間を選択している画像">}}

1. [保存]をクリックします。  
