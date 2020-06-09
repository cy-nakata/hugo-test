---
title: "Internet Explorerで、{{%cybozu_com%}}の画面が正しく表示されない場合"
weight: 300
---
{{% enabled JP %}}
Internet Explorerでサイボウズ Office、Garoon、{{%kintone%}}、またはメールワイズの画面を正しく表示できない場合は、下記のチェックリストに沿ってWebブラウザーの設定を確認してください。  
{{% /enabled %}}
{{% enabled CN %}}
Internet ExplorerでGaroonまたは{{%kintone%}}の画面を正しく表示できない場合は、下記のチェックリストに沿ってWebブラウザーの設定を確認してください。
{{% /enabled %}}
{{% enabled US %}}
Internet Explorerで{{%kintone%}}の画面が正しく表示できない場合は、下記のチェックリストに沿ってWebブラウザーの設定を確認してください。
{{% /enabled %}}

## トラブル解決に向けたチェックリスト{#list_start_ie_compatible_10}

STEP1から順に、Webブラウザーで下記の設定を確認します。  

* <b>STEP1</b>  
  この操作のあと、トラブルが解決していれば、STEP2以降の操作は不要です。  
  <table>
    <tbody>
    <tr>
    <th width="300">参照する項目</th>
    <th width="300">作業すること</th>
    </tr>
    <tr>
    <td rowspan="5"><a href="#list_start_ie_compatible_20">STEP1：Webブラウザーの設定を確認する</a></td>
    <td>TLS 1.1以降を有効にする</td>
    </tr>
    <tr>
    <td>JavaScriptの設定を有効にする</td>
    </tr>
    <tr>
    <td>Cookieを有効にする</td>
    </tr>
    <tr>
    <td>キャッシュの設定を確認する</td>
    </tr>
    <tr>
    <td>互換表示を無効にする</td>
    </tr>
    </tbody>
  </table>

* <b>STEP2</b>  
  この操作のあと、トラブルが解決していれば、STEP3の操作は不要です。  
  <table>
    <tbody>
    <tr>
    <th width="300">参照する項目</th>
    <th width="300">作業すること</th>
    </tr>
    <tr>
    <td rowspan="3"><a href="#list_start_ie_compatible_30">STEP2：STEP1を実行しても解決しない場合の対処</a></td>
    <td>Cookieやキャッシュファイルを削除する</td>
    </tr>
    <tr>
    <td>アドオンを無効にする</td>
    </tr>
    <tr>
    <td>「信頼済みサイト」に{{%service%}}のURLを登録する</td>
    </tr>
    </tbody>
  </table> 

* <b>STEP3</b>  
  <table>
    <tbody>
    <tr>
    <th width="300">参照する項目</th>
    <th width="300">作業すること</th>
    </tr>
    <tr>
    <td rowspan="3"><a href="#list_start_ie_compatible_40">STEP3：上記STEPを実行しても解決しない場合の対処</a></td>
    <td>同じクライアントパソコンで、ほかのWebブラウザーから、問題が発生するページにアクセスする</td>
    </tr>
    <tr>
    <td>ほかのクライアントパソコンから、問題が発生するページにアクセスする</td>
    </tr>
    </tbody>
  </table>

## STEP1：Webブラウザーの設定を確認する{#list_start_ie_compatible_20}

動作環境のWebブラウザーを使用していても、設定が正しくないと、{{%service%}}の画面を正しく表示できない場合があります。 

1. 使用しているInternet Explorerのバージョンが「11」であることを確認します。  
  「10」以前のバージョンは動作保証をしていません。  
  詳細は、[Internet Explorer のバージョン確認方法](https://support.microsoft.com/ja-jp/help/17295/internet-explorer-which-version-am-i-using)を参照してください。  

1. [Internet Explorer 11の設定方法](/ja/settings/browser/webbrowser/windows/winie11.html)を参照し、必要な設定をします。  

1. トラブルが解決しているかどうかを確認します。  

  * トラブルが解決していない場合：  
    [STEP2：STEP1を実行しても解決しない場合の対処](#list_start_ie_compatible_30)に進みます。  
  * トラブルが解決した場合：  
    作業は終了です。STEP2以降の操作は不要です。  

## STEP2：STEP1を実行しても解決しない場合の対処{#list_start_ie_compatible_30}

STEP1を実行してもトラブルが解決しない場合は、次の操作を上から順に実行します。  

* Cookieやキャッシュファイルを削除する
* アドオンを無効にする
* 「信頼済みサイト」に{{%service%}}のURLを登録する

### Cookieやキャッシュファイルを削除する{#list_start_ie_compatible_3010}

次の手順で、Internet ExplorerのCookieやキャッシュファイルを削除します。  

{{% warning %}}
この操作により、{{%service%}}を含め、保存している各サイトのログイン情報などが削除されます。
{{% /warning %}}

1. Webブラウザーを終了します。

1. [コントロールパネル]を表示し、[ネットワークとインターネット]をクリックします。  

1. [インターネットオプション]をクリックします。  

1. 「全般」タブを選択し、「閲覧の履歴」セクションの[削除]をクリックします。  

1. 「閲覧の履歴の削除」画面で、「インターネット一時ファイルおよび Web サイトのファイル」と「クッキーと Web サイト データ」のチェックボックスを選択し、[削除]をクリックします。  
  弊社製品のアクセスURLをお気に入りに登録している場合は、「お気に入り Web サイト データを保持する」のチェックボックスの選択も外します。  

1. 「インターネットのプロパティ」画面で、[適用] &gt; [OK]の順にクリックします。

1. トラブルが解決しているかどうかを確認します。  

  * トラブルが解決していない場合：  
    [アドオンを無効にする](#list_start_ie_compatible_3020)に進みます。  
  * トラブルが解決した場合：  
    作業は終了です。STEP2の残りの設定は不要です。

### アドオンを無効にする{#list_start_ie_compatible_3020}

次の手順で、Internet Explorerのアドオンを無効にします。  
アドオンの詳細は、Microsoft社のヘルプ：[Internet Explorer 11 のアドオンを管理する](https://support.microsoft.com/ja-jp/help/17447/windows-internet-explorer-11-manage-add-ons#ie=ie-10)
を参照してください。

1. Internet Explorerを起動し、 [ツール] &gt; [アドオンの管理] の順にクリックします。  
  メニューバーが表示されていない場合は、Altキーを押すと表示されます。

1. 画面下部の「表示」欄で「現在読み込まれているアドオン」を選択します。  

1. 無効にするアドオンを選択し、 [無効にする] &gt; [閉じる]の順にクリックします。  

1. トラブルが解決しているかどうかを確認します。  

  * トラブルが解決していない場合：  
    別のアドオンを無効にして解決しないか、手順1～3を繰り返して確認します。  
    他のアドオンを無効にしても解決しない場合は、[「信頼済みサイト」に{{%service%}}のURLを登録する](#list_start_ie_compatible_3030)に進みます。  
  * トラブルが解決した場合：  
    作業は終了です。影響がないアドオンは必要に応じて再度有効にします。  
    また、STEP2の残りの設定は不要です。

### 「信頼済みサイト」に{{%service%}}のURLを登録する{#list_start_ie_compatible_3030}

次の手順で、Internet Explorerの信頼済みサイトに{{%service%}}のURLを登録します。  

1. Internet Explorerメニューの「ツール」> 「インターネットオプション」をクリックします。  
    メニューが表示されていない場合は、Altキーを押すと表示されます。  

1. 「セキュリティ」タブ > 「信頼済みサイト」&gt; [サイト]の順にクリックします。  

1. 「この Web サイトをゾーンに追加する」に、ご利用中のサービスの、アクセスURLのIPアドレスまたはドメインまでの部分を入力します。  
    入力形式：https://（サブドメイン）.{{%cybozu_com%}}/  

1. 「このゾーンのサイトにはすべてのサーバーの確認（https:）を必要とする」のチェックを外します。  

1. [追加]をクリックし、「Web サイト」に手順3で入力したURLが追加されたことを確認します。  

1. 「信頼済みサイト」画面で、[閉じる]をクリックします。  

1. 「インターネットオプション」画面で、[OK]をクリックします。

1. トラブルが解決しているかどうかを確認します。  

  * トラブルが解決していない場合：  
    [STEP3：上記STEPを実行しても解決しない場合の対処](#list_start_ie_compatible_40)に進みます。  
  * トラブルが解決した場合：  
    作業は終了です。STEP3は不要です。

## STEP3：上記STEPを実行しても解決しない場合の対処{#list_start_ie_compatible_40}

STEP1とSTEP2を実行をしてもトラブルが解決しない場合は、下記の項目を確認します。  
確認結果を管理者にご相談のうえ、必要に応じて、管理者から[サポートにお問い合わせ](/general/ja/admin/support.html)ください。  

### 同じクライアントパソコンで、ほかのWebブラウザーから、問題が発生するページにアクセスする{#list_start_ie_compatible_4010}

Internet Explorer以外の動作保証されたWebブラウザーで、問題が発生するページにアクセスし、正しく表示されるかどうかを確認します。  

1. [動作環境のWebブラウザー](/general/ja/user/list_start/webbrowser.html#list_start_webbrowser_10)を表示します。  

1. 必要に応じて、Internet Explorer以外のWebブラウザーをインストールします。

1. Internet Explorer以外のWebブラウザーから、問題が発生するページにアクセスします。

1. 画面が正しく表示されるかどうかを確認します。  

  * 画面が正しく表示される場合：  
    [ほかのクライアントパソコンから、問題が発生するページにアクセスする](#list_start_ie_compatible_4020)に進みます。  
  * 画面が正しく表示されない場合：  
    ほかのWebブラウザーで表示に問題がない場合は、使用中のInternet Explorerの状態を確認します。  
    Internet Explorerをリセットすると、トラブルが解決する場合があります。詳細はMicrosoft社のヘルプ：[Internet Explorer の設定を変更またはリセットする](https://support.microsoft.com/ja-jp/help/17441/windows-internet-explorer-change-reset-settings)を参照してください。  
 
### ほかのクライアントパソコンから、問題が発生するページにアクセスする{#list_start_ie_compatible_4020}

ほかのクライアントパソコンでも、同じ現象が発生するかどうかを確認します。  
ほかのクライアントパソコンで表示に問題がない場合は、ご利用中のクライアントパソコンに依存する原因である可能性があります。  
