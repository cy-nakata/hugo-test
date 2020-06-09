---
title: "スマートフォンアプリからサービスにアクセスする"
weight: 200
---
{{% enabled US %}}
{{% warning %}}
この記事は、[AWSへの移行](https://www.kintone.com/aws-migration/)が完了していないお客様向けです。ドメインIDが「c」で始まるお客様が該当します。ドメインIDを確認するには「[ドメインIDの確認方法](/general/ja/admin/list_old/domainid.html)」を参照してください。
{{% /warning %}}
{{% /enabled %}}

{{% enabled JP CN %}}

設定方法は、利用するスマートフォンアプリによって異なります。お使いの端末の種類に合わせて、各スマートフォンアプリで提供しているマニュアルを参照してください。  

* [iPhoneからアクセスする場合](#remote_mobileapp_10)
* [Androidからアクセスする場合](#remote_mobileapp_20)

{{% warning %}}
{{% subtitle %}}セキュアアクセスを利用している場合{{% /subtitle %}}

* 「モバイルからのアクセス」画面や「クライアント証明書の情報」が表示されない場合、スマートフォンアプリは利用できません。  
  詳細は、[「モバイルからのアクセス」画面や「クライアント証明書の情報」が表示されない場合](/general/ja/user/list_access/access_service.html)を参照してください。

{{% subtitle %}}SAML認証を使用している場合{{% /subtitle %}}

* ログイン時にSAML認証だけを使うように制限されていると、利用できないモバイルアプリがあります。  
  詳細は、[制限を有効にした際に利用できなくなるサービスやモバイルアプリ](/general/ja/admin/list_externalservices/list_saml/saml_restriction.html#list_saml_saml_restriction_10)を参照してください。

{{% /warning %}}
{{% /enabled %}}

{{% enabled US %}}

スマートフォンアプリ「{{%kintone%}} モバイル」の設定方法は、お使いの端末の種類に合わせて、次の{{%kintone%}}のマニュアルを参照してください。

* [iPhoneからアクセスする場合](#remote_mobileapp_10)
* [Androidからアクセスする場合](#remote_mobileapp_20)

{{% warning %}}
{{% subtitle %}}セキュアアクセスを利用している場合{{% /subtitle %}}

* 「モバイルからのアクセス」画面や「クライアント証明書の情報」が表示されない場合、スマートフォンアプリは利用できません。  
  詳細は、[「モバイルからのアクセス」画面や「クライアント証明書の情報」が表示されない場合](/general/ja/user/list_access/access_service.html)を参照してください。

{{% subtitle %}}SAML認証を設定している場合{{% /subtitle %}}

* ログイン時にSAML認証だけを使うように制限すると、利用できなくなるモバイルアプリがあります。  
  詳細は、[制限を有効にした際に利用できなくなるサービスやモバイルアプリ](/general/ja/admin/list_externalservices/list_saml/saml_restriction.html#list_saml_saml_restriction_10)を参照してください。

{{% /warning %}}
{{% /enabled %}}

## iPhoneからアクセスする場合{#remote_mobileapp_10}

{{% enabled JP %}}

設定手順は、各スマートフォンアプリのマニュアルを参照してください。

| スマートフォンアプリ       | マニュアル                                                       |
| -------------------------- | ------------------------------------------------------------ |
| KUNAI                      | [設定ファイルを使用して接続設定を行う（KUNAI for iPhone）](https://manual.cybozu.co.jp/kunai/ip/setting/sa.html) |
| サイボウズ Office 新着通知 | [「サイボウズ Office 新着通知」を設定する（「モバイルかんたん設定機能」を使用する場合）](https://jp.cybozu.help/ja/o/user/secure/nsp/secure) |
| {{%kintone%}} モバイル      | セキュアアクセスを利用している場合：[セキュアアクセスでモバイルを利用する(iOS)](/k/ja/user/mobile_access/ios/secure_ios.html#ios_secure_ios_30)<br> セキュアアクセスを利用していない場合：[iOSのモバイルアプリを利用する](/k/ja/user/mobile_access/ios/mobileapp_ios.html) |
| メールワイズ       | [「メールワイズ for iOS」の接続設定をする](https://manual.cybozu.co.jp/mailwise_cloud/ios/setting.html#anchor02) |

{{% /enabled %}}

{{% enabled US %}}

* <b>セキュアアクセスを利用している場合：</b>  
  [セキュアアクセスでモバイルを利用する(iOS)](/k/ja/user/mobile_access/ios/secure_ios.html#ios_secure_ios_30)ページを参照してください。
* <b>セキュアアクセスを利用していない場合：</b>  
  [iOSのモバイルアプリを利用する](/k/ja/user/mobile_access/ios/mobileapp_ios.html)ページを参照してください。

{{% /enabled %}}

{{% enabled CN %}}

設定手順は、各スマートフォンアプリのマニュアルを参照してください。

| スマートフォンアプリ       | マニュアル                                                       |
| -------------------------- | ------------------------------------------------------------ |
| KUNAI                      | [設定ファイルを使用して接続設定を行う（KUNAI for iPhone）](https://manual.cybozu.co.jp/kunai/ip/setting/sa.html) |
| {{%kintone%}} モバイル      |セキュアアクセスを利用している場合：[セキュアアクセスでモバイルを利用する(iOS)](/k/ja/user/mobile_access/ios/secure_ios.html#ios_secure_ios_30)<br> セキュアアクセスを利用していない場合：[iOSのモバイルアプリを利用する](/k/ja/user/mobile_access/ios/mobileapp_ios.html) |

{{% /enabled %}}

{{% note %}}
iOS用のGmailアプリまたはOutlookアプリを利用している場合、クライアント証明書（********.pfx）を開けません。アプリではなく、SafariからGmailまたはOffice365にアクセスして、メールに添付されたクライアント証明書を開いてください。
{{% /note %}}

## Androidからアクセスする場合{#remote_mobileapp_20}

{{% enabled JP %}}

設定手順は、各スマートフォンアプリのマニュアルを参照してください。

| スマートフォンアプリ       | マニュアル                                                       |
| -------------------------- | ------------------------------------------------------------ |
| KUNAI                      | [設定ファイルを使用して接続設定を行う（KUNAI for Android）](https://manual.cybozu.co.jp/kunai/an/setting/sa.html) |
| サイボウズ Office 新着通知 | [「サイボウズ Office 新着通知」を設定する（「モバイルかんたん設定機能」を使用する場合）](https://jp.cybozu.help/ja/o/user/secure/ansp/secure)|
| {{%kintone%}} モバイル      |セキュアアクセスを利用している場合：[セキュアアクセスでモバイルを利用する（Android）](/k/ja/user/mobile_access/android/secure_android.html#android_secure_android_30)<br> セキュアアクセスを利用していない場合：[Androidのモバイルアプリを利用する](/k/ja/user/mobile_access/android/mobileapp_android.html)|
| メールワイズ       | [「メールワイズ for Android」の接続設定をする](https://manual.cybozu.co.jp/mailwise_cloud/android/setting.html#anchor01) |

{{% /enabled %}}

{{% enabled US %}}

* <b>セキュアアクセスを利用している場合：</b>  
  [セキュアアクセスでモバイルを利用する（Android）](/k/ja/user/mobile_access/android/secure_android.html#android_secure_android_30)ページを参照してください。
* <b>セキュアアクセスを利用していない場合：</b>  
  [Androidのモバイルアプリを利用する](/k/ja/user/mobile_access/android/mobileapp_android.html)ページを参照してください。

{{% /enabled %}}

{{% enabled CN %}}

設定手順は、各スマートフォンアプリのマニュアルを参照してください。

| スマートフォンアプリ       | マニュアル                                                       |
| -------------------------- | ------------------------------------------------------------ |
| KUNAI                      | [設定ファイルを使用して接続設定を行う（KUNAI for Android）](https://manual.cybozu.co.jp/kunai/an/setting/sa.html) |
| {{%kintone%}} モバイル      | セキュアアクセスを利用している場合：[セキュアアクセスでモバイルを利用する（Android）](/k/ja/user/mobile_access/android/secure_android.html#android_secure_android_30)<br> セキュアアクセスを利用していない場合：[Androidのモバイルアプリを利用する](/k/ja/user/mobile_access/android/mobileapp_android.html)|

{{% /enabled %}}

{{% note %}}
端末の設定やOSのバージョンによって、クライアント証明書の登録に画面ロックの設定を必要とする場合があります。画面ロックが未設定の場合、クライアント証明書を登録する際に、画面ロックの設定が要求されます。
{{% /note %}}
