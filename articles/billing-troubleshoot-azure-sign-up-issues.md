---
title: "Azure のサインアップに関する問題のトラブルシューティング | Microsoft Docs"
description: "Azure のサインアップに関する一般的な問題をトラブルシューティングする方法について説明します。"
services: 
documentationcenter: 
author: JiangChen79
manager: felixwu
editor: 
tags: billing,top-support-issue
ms.assetid: a0907da1-cb2d-41d1-a97f-43841fabe355
ms.service: billing
ms.workload: na
ms.tgt_pltfrm: ibiza
ms.devlang: na
ms.topic: article
ms.date: 10/25/2016
ms.author: cjiang
translationtype: Human Translation
ms.sourcegitcommit: 219dcbfdca145bedb570eb9ef747ee00cc0342eb
ms.openlocfilehash: e2e22b767ce1d54e7b90158fb6adb877e3a165b8


---
# <a name="i-cant-sign-up-for-azure"></a>Azure にサインアップできません
Azure にサインアップできない場合は、問題をトラブルシューティングするために確認できるいくつかの事柄があります。

## <a name="no-text-messages-or-calls-during-sign-up-account-verification"></a>サインアップ アカウントの検証中に、テキスト メッセージの送信がなく、電話もかかってこない
* SMS を受信できる電話番号であることを確認します。
* ドロップダウン メニューで、国コードの内容を含む電話番号を再確認してください。
* [テキスト メッセージを受信] を使用する場合はご自分の電話でテキスト メッセージ (SMS) を受信できることを、[電話で確認コードを受け取る] を選択した場合は通話呼び出しを受信できることを確認します。
* 携帯電話を使用する場合は、携帯電話の接続状態が良好であることを確認します。
* [テキスト メッセージを受信] を選択した場合は、最大で 4 分待つと、メッセージング システムからお客様のテキスト コードが送信されてきます。
* テキスト メッセージを受信したら、テキスト ボックスにそのコードを入力し、検証ボタンをクリックして続行します。

### <a name="suggestions"></a>検索候補
* ご自分の電話でテキスト メッセージ (SMS) を受信しない場合は、代わりの確認方法である [電話で確認コードを受け取る] を使用してください。
* SMS と [電話で確認コードを受け取る] のどちらの方法を使用しても電話での確認手順に失敗する場合は、別の電話番号を使用してください。
* 電話確認処理に VoIP 電話番号を使用することはできません。

> [!NOTE]
> 後で希望の電話番号を変更するには、 [プロファイル情報を更新します](billing-how-to-change-azure-account-profile.md)。
> 
> 

## <a name="credit-card-declined-or-not-accepted"></a>クレジット カードが拒否されます
サインアップ時に使用する支払方法が Azure のアクティブ化または支払いでサポートされていることを確認します。

* バーチャルおよびプリペイドのクレジット/デビット カードは使用できません。
* 使用できるクレジット/デビット カード会社は、アカウントの国によって異なります。

### <a name="suggestion"></a>推奨事項
クレジット カードやデビット カードを使用したサインアップの問題の一般的な原因については、「[サインアップ時にクレジット カードまたはデビット カードが拒否される場合](billing-credit-card-fails-during-azure-sign-up.md)」を参照してください。

## <a name="cant-activate-azure-benefit-plan-like-msdn-bizspark-bizsparkplus-or-mpn"></a>MSDN、BizSpark、BizSparkPlus、MPN などの Azure 特典プランをアクティブ化できません
プランを選択する資格がある場合は、特典プログラム チャネルを調べます。

* MSDN
  * [MSDN アカウント ページ](https://msdn.microsoft.com/subscriptions/manage/default.aspx)で資格の状態を確認します。
  * 状態を確認できない場合は、 [MSDN サブスクリプション カスタマー サービス センター](https://msdn.microsoft.com/subscriptions/contactus.aspx)
* MPN
  * [MPN ポータル](https://mspartner.microsoft.com/en/us/Pages/Locale.aspx) にサインインし、資格の状態を確認します。 該当する [クラウド プラットフォーム コンピテンシー](https://mspartner.microsoft.com/en/us/pages/membership/cloud-platform-competency.aspx)をお持ちの場合、追加特典の資格を与えられることがあります。
  * 状態を確認できない場合は、 [MPN サポート](https://mspartner.microsoft.com/en/us/Pages/Support/Premium/contact-support.aspx)にお問い合わせください。
* Bizpark
  * [BizSpark ポータル](https://www.microsoft.com/bizspark/default.aspx#start-two) にサインインし、BizSpark と BizSpark Plus の資格の状態を確認します。
  * 自分の資格の状態を確認できない場合は、 [BizSpark サポート チーム](mailto:bizspark@microsoft.com?subject=BizSpark%20Support&body=Thank%20you%20for%20contacting%20BizSpark.%20Please%20provide%20as%20much%20of%20the%20following%20information%20as%20possible,%20as%20it%20will%20help%20expedite%20our%20response%20to%20you.%0aContact%20name:%0aStartup%20name:%0aMicrosoft%20Account/Live%20ID:%0aSpecific%20description%20of%20issue%20experienced%20or%20question:%0a%0aThank%20you,%0a%0aThe%20BizSpark%20Team)

### <a name="suggestion"></a>推奨事項
サインアップ操作中に新しい特典サブスクリプションをアクティブ化しようとするとエラーが発生する場合は、[Azure サブスクリプション ページ](http://account.windowsazure.com/Subscriptions)でサブスクリプションのセットアップが完了していることを確認してください。 サブスクリプションがアクティブ状態であると表示されるまで数分かかる場合があります。 サブスクリプションがアクティブになると、電子メールが届きます。 5 分以上経過してもサブスクリプションが保留中のままである場合は、[Azure サポートにお問い合わせ](http://go.microsoft.com/fwlink/?linkid=544831&clcid=0x409)ください。

## <a name="cant-activate-new-azure-in-open-subscription"></a>新しい Azure イン オープン プラン サブスクリプションをアクティブ化できません
新しい Azure イン オープン プラン サブスクリプションをアクティブ化するには、少なくとも 1 つの Azure イン オープン プラン トークンが関連付けられている有効な OSA キーを持っている必要があります。

### <a name="suggestion"></a>推奨事項
OSA キーを持っていない場合は、[Microsoft Pinpoint](http://pinpoint.microsoft.com/)に記載されている Microsoft パートナーにお問い合わせください。

## <a name="cant-activate-azure-free-trial"></a>Azure 無料試用版をアクティブ化できません
過去に Azure サブスクリプションを使用していませんか。 Azure 使用条件契約書では、Azure を初めて使用するユーザーのみが Azure 無料試用版をアクティブ化できるという制限を設けています。 他の種類の Azure サブスクリプションを持っている場合も、無料試用版をアクティブ化することはできません。

### <a name="suggestion"></a>推奨事項
* Azure サブスクリプションを過去にアクティブ化しているために無料試用版をアクティブ化できない場合は、従量課金サブスクリプションをご検討ください。 
* 特典プランを利用できる資格があるかどうかを確認します。 [Microsoft Azure プランの詳細に関するページ](https://azure.microsoft.com/support/legal/offer-details/)を参照してください。 特典プランのご利用には前提条件があります。

## <a name="need-help-contact-support"></a>お困りの際は、 サポートにお問い合せください。
お困りの際は、問題を迅速に解決するために、[サポートにお問い合わせ](https://portal.azure.com/?#blade/Microsoft_Azure_Support/HelpAndSupportBlade)ください。 




<!--HONumber=Nov16_HO3-->


