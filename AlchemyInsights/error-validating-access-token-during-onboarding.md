---
title: Desktop Analytics'e kabul edilirken erişim belirteci hatasını doğrulama hatası oluştu
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 12e5906ba8cbc76ba1fd99dde1cf76396c3a6942
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813708"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="697ab-102">Desktop Analytics ekleme sırasında "Erişim belirteci doğrulayla ilgili bir hata oluştu" hatası</span><span class="sxs-lookup"><span data-stu-id="697ab-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="697ab-103">Bu hata normalde kimlik doğrulama belirtecin süresi dolduğunda gözlemlenir.</span><span class="sxs-lookup"><span data-stu-id="697ab-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="697ab-104">Genellikle, sayfa yenilendiğinde belirteci yeniler.</span><span class="sxs-lookup"><span data-stu-id="697ab-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="697ab-105">Bununla birlikte, tahtada Desktop Analytics'e kullanılan hesaba uygulanmış herhangi bir Koşullu Erişim ilkesi varsa bu sorun kalıcı olabilir.</span><span class="sxs-lookup"><span data-stu-id="697ab-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="697ab-106">Desktop Analytics ekleme için kullanılan hesapta herhangi bir oturum açma hatası olup kontrol etmek için Azure Portal'daki Azure AD Oturum Açma günlüklerini gözden geçirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="697ab-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="697ab-107">Koşullu Erişim hakkında daha fazla bilgi için Koşullu Erişim [dağıtımınızı planlama .](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)</span><span class="sxs-lookup"><span data-stu-id="697ab-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>