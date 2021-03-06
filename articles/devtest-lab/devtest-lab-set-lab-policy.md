---
title: "Azure DevTest Labs でのラボのポリシーの定義 | Microsoft Docs"
description: "VM サイズ、ユーザーごとの VM の最大数、シャットダウンの自動化など、ラボのポリシーを定義する方法について説明します。"
services: devtest-lab,virtual-machines
documentationcenter: na
author: tomarcher
manager: douge
editor: 
ms.assetid: 7756aa64-49ca-45a0-9f90-0fd101c7be85
ms.service: devtest-lab
ms.workload: na
ms.tgt_pltfrm: na
ms.devlang: na
ms.topic: article
ms.date: 09/12/2016
ms.author: tarcher
translationtype: Human Translation
ms.sourcegitcommit: 2ea002938d69ad34aff421fa0eb753e449724a8f
ms.openlocfilehash: 4222de44e426c449a42822994b1c15b44c3fec54


---
# <a name="define-lab-policies-in-azure-devtest-labs"></a>Azure DevTest Labs でのラボのポリシーの定義
> [!VIDEO https://channel9.msdn.com/Blogs/Windows-Azure/How-to-set-VM-policies-in-a-DevTest-Lab/player]
> 
> 

Azure DevTest Labs では、コストを制御し、ラボでの無駄を最小限にするためのキー ポリシーを指定できます。 これらのラボ ポリシーには、ユーザーごとおよびラボごとに作成された VM の最大数、およびさまざまな自動シャット ダウンおよび自動起動オプションの最大数が含まれます。 

## <a name="accessing-a-labs-policies-in-azure-devtest-labs"></a>Azure DevTest Labs でのラボのポリシーへのアクセス
次の手順は、Azure DevTest Labs でラボのポリシーを設定する方法を示します。

ラボのポリシーを表示 (および変更) するには、次の手順に従います。

1. [Azure ポータル](http://go.microsoft.com/fwlink/p/?LinkID=525040)にサインインします。
2. **[その他のサービス]** を選択し、一覧の **[DevTest Labs]** を選択します。
3. ラボの一覧で目的のラボを選択します。   
4. **[ポリシー設定]**を選択します。
5. **[ポリシー設定]** ブレードには、指定できる設定のメニューが含まれています。 
   
    ![ポリシー設定ブレード](./media/devtest-lab-set-lab-policy/policies.png)
   
    ポリシーの設定の詳細について確認するには、次の一覧から選択してください。
   
   * [許可される VM サイズ](#set-allowed-virtual-machine-sizes) - ラボで使用できる VM サイズの一覧を選択します。 ユーザーは、この一覧からのみ VM を作成できます。
   * [ユーザーごとの VM 数](#set-virtual-machines-per-user) - ユーザーが作成できる VM の最大数を指定します。 
   * [ラボごとの VM 数](#set-virtual-machines-per-lab) - ラボに作成できる VM の最大数を指定します。 
   * [自動シャットダウン](#set-auto-shutdown) - 現在のラボの VM を自動的にシャットダウンする時刻を指定します。
   * [自動開始](#set-auto-start) - 現在のラボの VM を自動的に開始する時刻を指定します。

## <a name="set-allowed-virtual-machine-sizes"></a>許可される仮想マシン サイズの設定
許可される VM サイズを設定するポリシーでは、ラボで使用可能な VM サイズを指定できるので、ラボの無駄を最小限に抑えるのに役立ちます。 このポリシーを有効にすると、この一覧の VM サイズだけを使用して VM を作成できます。

1. ラボの **[ポリシー設定]** ブレードで、**[Allowed virtual machines sizes (許可される仮想マシンのサイズ)]** を選択します。
   
    ![[許可される仮想マシンのサイズ]](./media/devtest-lab-set-lab-policy/allowed-vm-sizes.png)
2. このポリシーを有効にするには **[オン]** を選択し、無効にするには **[オフ]** を選択します。
3. このポリシーを有効にする場合は、ラボで作成できる 1 つ以上の VM サイズを選択します。
4. [ **保存**] を選択します。

## <a name="set-virtual-machines-per-user"></a>ユーザーごとの仮想マシンの設定
**[ユーザーごとの VM 数]** のポリシーでは、各ユーザーが作成できる VM の最大数を指定できます。 ユーザーの上限に達している場合、ユーザーが VM を作成しようとすると、VM を作成できないことを示すエラー メッセージが表示されます。 

1. ラボの **[ポリシー設定]** ブレードで、**[Virtual machines per user (ユーザーあたりの仮想マシン数)]** を選択します。
   
    ![ユーザーごとの VM 数](./media/devtest-lab-set-lab-policy/max-vms-per-user.png)
2. このポリシーを有効にするには **[オン]** を選択し、無効にするには **[オフ]** を選択します。
3. このポリシーを有効にする場合は、ユーザーが作成できる VM の最大数を示す数値を入力します。 
   無効な数値を入力すると、このフィールドに入力できる最大数が UI に表示されます。
4. [ **保存**] を選択します。

## <a name="set-virtual-machines-per-lab"></a>ラボごとの仮想マシンの設定
**ラボごとの VM 数** のポリシーでは、現在のラボで作成できる VM の最大数を指定することができます。 ラボの上限に達している場合、ユーザーが VM を作成しようとすると、VM を作成できないことを示すエラー メッセージが表示されます。 

1. ラボの **[ポリシー設定]** ブレードで、**[Virtual machines per lab (ラボあたりの仮想マシン数)]** を選択します。
   
    ![ラボごとの VM 数](./media/devtest-lab-set-lab-policy/total-vms-allowed.png)
2. このポリシーを有効にするには **[オン]** を選択し、無効にするには **[オフ]** を選択します。
3. このポリシーを有効にする場合は、現在のラボに作成できる VM の最大数を示す数値を入力します。 
   無効な数値を入力すると、このフィールドに入力できる最大数が UI に表示されます。
4. [ **保存**] を選択します。

## <a name="set-auto-shutdown"></a>自動シャットダウンの設定
自動シャットダウン ポリシーでは、このラボの VM をシャットダウンする時刻を指定できるので、ラボの無駄を最小限に抑えるのに役立ちます。

1. ラボの **[ポリシー設定]** ブレードで、**[自動シャットダウン]** を選択します。
   
    ![自動シャットダウン](./media/devtest-lab-set-lab-policy/auto-shutdown.png)
2. このポリシーを有効にするには **[オン]** を選択し、無効にするには **[オフ]** を選択します。
3. このポリシーを有効にする場合は、現在のラボのすべての VM をシャットダウンするローカル時刻を指定します。
4. [ **保存**] を選択します。
5. このポリシーを有効にすると、既定では現在のラボのすべての VM にこのポリシーが適用されます。 この設定を特定の VM から削除するには、その VM のブレードを開いて **[自動シャットダウン]** 設定を変更します。 

## <a name="set-auto-start"></a>自動開始の設定
自動開始のポリシーでは、現在のラボにある VM をいつ開始するか指定することができます。  

1. ラボの **[ポリシー設定]** ブレードで、**[Auto-start (自動開始)]** を選択します。
   
    ![自動開始](./media/devtest-lab-set-lab-policy/auto-start.png)
2. このポリシーを有効にするには **[オン]** を選択し、無効にするには **[オフ]** を選択します。
3. このポリシーを有効にする場合は、ローカルにスケジュール設定した開始時間と、それを適用する曜日を指定します。 
4. [ **保存**] を選択します。
5. このポリシーを有効にしても、現在のラボの VM に自動的に適用されることはありません。 この設定を特定の VM に適用するには、その VM のブレードを開いて **[自動開始]** 設定を変更します。 

[!INCLUDE [devtest-lab-try-it-out](../../includes/devtest-lab-try-it-out.md)]

## <a name="next-steps"></a>次のステップ
ラボに対して各種の VM ポリシー設定を定義および適用した後は、次に示すいくつかの操作を試してみてください。

* [コスト管理を構成する](devtest-lab-configure-cost-management.md) - **月間推定コスト傾向**グラフを使用して  
  現在のカレンダー月の現時点までの推定コストと月末の予測コストを表示する方法を示します。
* [カスタム イメージを作成する](devtest-lab-create-template.md) - VM を作成する場合は、ベースとしてカスタム イメージまたは Marketplace イメージを指定します。 この記事では、VHD ファイルからカスタム イメージを作成する方法について説明します。
* [Marketplace イメージを構成する](devtest-lab-configure-marketplace-images.md) - Azure DevTest Labs では、Azure Marketplace イメージを基にした VM を作成することができます。 この記事では、ラボで VM を作成する際に使用できるようにする Azure Marketplace イメージ (該当するものがある場合) を指定する方法について説明します。
* [ラボで VM を作成する](devtest-lab-add-vm-with-artifacts.md) - 基本イメージ (カスタムまたは Marketplace) から VM を作成する方法と、VM でアーティファクトを操作する方法について説明します。




<!--HONumber=Nov16_HO3-->


