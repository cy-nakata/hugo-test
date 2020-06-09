---
title: "監査ログの見かた"
weight: 100
---
監査ログは、{{%slash%}}共通管理で確認します。  
必要に応じて、監査ログのファイル書き出しや、ログのレベルに応じたメール通知も設定できます。  

ログには下記のどちらかのレベルが表示されます。  
このレベルは、ログの絞り込み条件やメール通知の設定に利用します。  

* 重要
* 情報  

{{% note %}}
監査ログの出力時刻やメール通知文には、システムのタイムゾーンと言語が適用されます。  
システムのタイムゾーンや言語の設定は、[ローカライズの設定を変更する](/general/ja/admin/list_systemadmin/list_system_time/system_time.html)を参照してください。  
{{% /note %}}

1. {{%slash%}}共通管理画面の「監査ログ」の、[閲覧とダウンロード]をクリックします。  
  {{< screen src="/general/img-ja/audit_img01.png"  alt="[閲覧とダウンロード]をクリックする画像">}}  
  
1. 閲覧するログを絞り込み、[閲覧]をクリックします。  
  絞り込み条件に指定する「モジュール」や「アクション」の値は、[監査ログの一覧](/general/ja/admin/list_systemadmin/list_audit/log.html)を参照してください。  
  {{< screen src="/general/img-ja/audit_img02.png"  alt="表示するログの条件を設定する画像">}}  

1. ログを確認します。  
  画面下部に、絞り込んだログが表示されます。  
  表示されるログの詳細は、[監査ログの一覧](/general/ja/admin/list_systemadmin/list_audit/log.html)を参照してください。  
  {{< screen src="/general/img-ja/audit_img03.png"  alt="出力されたログを確認する画像">}}  
  {{%service%}}共通のログか、サービス特有のログかは、表示されるログの「サービス」欄で確認します。  
  {{< screen src="/general/img-ja/audit_img04.png"  alt="サービス欄を説明する画像">}}  

1. ログの詳細を確認する場合は、[i]アイコンをクリックします。  
  {{< screen src="/general/img-ja/audit_img05.png"  alt="[i]アイコンを示す画像">}}  

1. 「補足」欄で、監査ログの詳細を確認します。  
  {{< screen src="/general/img-ja/audit_img06.png"  alt="ログの詳細を示す画像">}}  

1. 必要に応じて、監査ログの出力に関する設定をします。  

    * [監査ログの保存期間を設定する](/general/ja/admin/list_systemadmin/list_audit/set_audit.html)
    * [監査ログの情報をメールで送信する](/general/ja/admin/list_systemadmin/list_audit/send_audit.html)
