---
title: "監査ログをファイルに書き出す"
weight: 400
---
監査ログをファイルに書き出す方法を説明します。  
直近6週間未満の監査ログを書き出す場合と、6週間以上前の監査ログを書き出す場合で、手順が異なります。  

## 直近6週間未満の監査ログ {#list_audit_download_audit_10}

6週間未満の監査ログは、CSVファイル形式（UTF-8）で10万件まで書き出せます。  

1. {{%slash%}}共通管理画面で、「監査ログ」の[閲覧とダウンロード]をクリックします。
  {{< screen src="/general/img-ja/download_audit_img01.png"  alt="[閲覧とダウンロード]が赤枠で囲まれた画像">}}

1. 絞り込み条件を設定し、[ダウンロード]をクリックします。  
  {{< screen src="/general/img-ja/download_audit_img02.png"  alt="絞り込み条件を設定する画像">}}

1. [監査ログのファイルをExcelで開く](/general/ja/admin/list_systemadmin/list_audit/audit_excel.html)を参照して、ダウンロードしたCSVファイルを確認します。  
  上記の操作をせずに、CSVファイルを直接Microsoft Excelで開いてしまうと、文字化けする場合があります。  

## 6週間以上前の監査ログ {#list_audit_download_audit_20}

6週間以上前の監査ログはアーカイブされます。  
アーカイブ化された監査ログは、CSVファイル形式（UTF-8）でダウンロードできます。  

保存期間の初期値は3年間で、最大10年間まで設定できます。  
詳細は、[監査ログの保存期間を設定する](/general/ja/admin/list_systemadmin/list_audit/set_audit.html)を参照してください。

1. {{%slash%}}共通管理画面で、「監査ログ」の[閲覧とダウンロード]をクリックします。
  {{< screen src="/general/img-ja/download_audit_img01.png"  alt="[閲覧とダウンロード]が赤枠で囲まれた画像">}}

1. [6週間以上前のログのダウンロード]をクリックします。
  {{< screen src="/general/img-ja/download_audit_img03.png"  alt="[6週間以上前のログのダウンロード]が赤枠で囲まれた画像">}}

1. 「検索する年」を入力して[検索]をクリックします。
  {{< screen src="/general/img-ja/download_audit_img04.png"  alt="検索する年を入力している画像">}}

1. 「ダウンロード」に表示されたアーカイブを、クリックしてダウンロードします。
  {{< screen src="/general/img-ja/download_audit_img05.png"  alt="アーカイブが表示されたときの画面例">}}

1. [監査ログのファイルをExcelで開く](/general/ja/admin/list_systemadmin/list_audit/audit_excel.html)を参照して、ダウンロードしたCSVファイルを確認します。  
  上記の操作をせずに、CSVファイルを直接Microsoft Excelで開いてしまうと、文字化けする場合があります。  
