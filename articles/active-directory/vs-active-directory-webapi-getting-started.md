---
title: "Azure Active Directory と Visual Studio 接続済みサービスの概要 (WebApi プロジェクト) | Microsoft Docs"
description: "Visual Studio 接続済みサービスを使用して Azure Active Directory を接続または作成した後に、Web API プロジェクトで Azure AD の使用を開始する方法について説明します。"
services: active-directory
documentationcenter: 
author: TomArcher
manager: douge
editor: 
ms.assetid: bf1eb32d-25cd-4abf-8679-2ead299fedaa
ms.service: active-directory
ms.workload: web
ms.tgt_pltfrm: vs-getting-started
ms.devlang: na
ms.topic: article
ms.date: 11/18/2016
ms.author: tarcher
translationtype: Human Translation
ms.sourcegitcommit: 2ea002938d69ad34aff421fa0eb753e449724a8f
ms.openlocfilehash: 05a507e328bb79e976ebccfdfae0dc2d7c82f374


---
# <a name="get-started-with-azure-active-directory-and-visual-studio-connected-services-webapi-projects"></a>Azure Active Directory と Visual Studio 接続済みサービスの概要 (Web API プロジェクト)
> [!div class="op_single_selector"]
> * [作業の開始](vs-active-directory-webapi-getting-started.md)
> * [変更内容](vs-active-directory-webapi-what-happened.md)
> 
> 

## <a name="requiring-authentication-to-access-controllers"></a>コントローラーへのアクセスに対して認証を要求する
プロジェクトに含まれるすべてのコントローラーには、 **Authorize** 属性が設定されています。 この属性により、ユーザーがこれらのコントローラーによって定義された API にアクセスする際に認証が求められます。 これらのコントローラーに匿名でアクセスできるようにするには、コントローラーからこの属性を削除します。 より細かなレベルでアクセス許可を設定するには、コントローラー クラスではなく、認証を必要とするそれぞれのメソッドに対してこの属性を割り当てます。

[Azure Active Directory の詳細を確認する](https://azure.microsoft.com/services/active-directory/)




<!--HONumber=Nov16_HO3-->


