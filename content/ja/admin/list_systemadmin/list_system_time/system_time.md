---
title: "ローカライズの設定を変更する"
weight: 200
---
ローカライズでは、{{%cybozu_com%}}のシステムが使用するタイムゾーンと言語を設定します。

## 設定が適用される項目、指定できる設定値、および初期値

<table>
    <caption>タイムゾーン</caption>
    <tbody>
        <tr>
            <th>適用される項目</th>
            <td>
            <ul>
                <li>監査ログで出力するデータの日時</li>
                <li>「ユーザーの追加」画面のタイムゾーンの初期値</li>
                <li>「タイムゾーン」項目が空欄のCSVファイルを読み込んでユーザー情報を編集した場合に、タイムゾーンに設定される値</li>
                <li>「契約状況」画面の「開始日」と「終了日」<sup>1</sup></li>  
            </ul>
            </td>
        </tr>
        <tr>
            <th>設定値</th>
            <td>次のページを参照してください。<br />
            <a href="/general/ja/admin/list_systemadmin/list_system_time/timezone.html">タイムゾーンの一覧</a></td>
        </tr>
        <tr>
            <th>初期値</th>
            <td>{{% disabled US CN %}}{{%store%}}で{{% /disabled %}}サービスを契約した地域のタイムゾーン</td>
        </tr>
    </tbody>
</table>
{{% enabled JP %}}
<sup>1</sup> {{%store%}}の管理者の設定によっては、「契約状況」画面に「開始日」や「終了日」が表示されない場合があります。
{{% /enabled %}}

{{% enabled US %}}
{{% note %}}
{{% subtitle %}}<sup>1</sup>ご利用環境のドメインによる違い{{% /subtitle %}}

* **[AWSへの移行](https://www.kintone.com/aws-migration/)が完了していないお客様**（[ドメインID](/general/ja/admin/list_old/domainid.html)が「c」で始まるお客様）  
   {{%store%}}の管理者の設定によっては、「契約状況」画面に「開始日」や「終了日」が表示されない場合があります。
* **[AWSへの移行](https://www.kintone.com/aws-migration/)が完了したお客様**（[ドメインID](/general/ja/admin/list_old/domainid.html)が「y」で始まるお客様）  
  「契約状況」画面に「開始日」や「終了日」は表示されません。
{{% /note %}}
{{% /enabled %}}

<table>
    <caption>言語</caption>
    <tbody>
        <tr>
            <th>適用される項目</th>
            <td>
            <ul>
                <li>次のメール通知
                <ul>
                    <li>監査ログが記録されたときに送信されるメール通知</li>
                    <li>管理者がユーザーを追加したときに、追加したユーザー宛てに送信されるメール通知 <sup>1</sup></li>
                    <li>管理者がパスワードを変更したときに、パスワードが変わったユーザー宛てに送信されるメール通知 <sup>1</sup></li>
                </ul>
                </li>
                <li>次の選択肢の初期値
                <ul>
                    <li>ユーザーの「別言語での表示名」で指定する言語</li>
                    <li>組織の「別言語での表示名」で指定する言語</li>
                </ul>
                </li>
                <li>APIのエラーメッセージ <sup>2</sup></li>
            </ul>
            </td>
        </tr>
        <tr>
            <th>設定値</th>
            <td>
            <ul>
                <li>日本語</li>
                <li>英語</li>
                <li>中国語（簡体字）</li>
            </ul>
            </td>
        </tr>
        <tr>
            <th>初期値</th>
            <td>{{% enabled JP %}}日本語{{% /enabled %}}{{% enabled US %}}英語{{% /enabled %}}{{% enabled CN %}}中国語（簡体字）{{% /enabled %}}</td>
        </tr>
    </tbody>
</table>
<sup>1</sup> 通知を受信するユーザーが、言語を「Webブラウザーの設定に従う」以外に設定している場合は、通知を受信するユーザーが設定した言語で通知が送信されます。  
<sup>2</sup> HTTPヘッダーの「accept-language」プロパティで言語を指定している場合、または、APIの実行ユーザーが言語を「Webブラウザーの設定に従う」以外に設定している場合は、指定した言語でエラーメッセージが返ります。

## ローカライズの設定を変更する

1. 「{{%slash%}}共通管理」画面の[ローカライズ]をクリックします。
1. 「タイムゾーン」と「言語」のドロップダウンリストで、システムが使用するタイムゾーンと言語を選択し、[保存]をクリックします。
