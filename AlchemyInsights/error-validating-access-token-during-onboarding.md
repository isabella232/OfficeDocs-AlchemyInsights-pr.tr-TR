---
title: Masaüstü analizi sırasında erişim belirteci hatası doğrulanırken hata oluştu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 45c6fb1a1632799a07c028c0791b6b8e77635293
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783571"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="983dc-102">Masaüstü analitik ekleme sırasında "erişim belirteci doğrulanırken hata oluştu" hatası</span><span class="sxs-lookup"><span data-stu-id="983dc-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="983dc-103">Bu hata normalde kimlik doğrulama belirtecinin süresi dolduğunda izlenir.</span><span class="sxs-lookup"><span data-stu-id="983dc-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="983dc-104">Genellikle, sayfayı yenilemek belirteci yeniler.</span><span class="sxs-lookup"><span data-stu-id="983dc-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="983dc-105">Ancak, yerleşik masaüstü analizinde kullanılan hesaba herhangi bir koşullu erişim ilkesi uygulanmışsa bu sorun devam edebilir.</span><span class="sxs-lookup"><span data-stu-id="983dc-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="983dc-106">Masaüstü Analizi ekleme için kullanılan hesabın oturum açma hataları olup olmadığını görmek için Azure portalında Azure AD oturum açma günlüklerini gözden geçirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="983dc-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="983dc-107">Koşullu erişim hakkında daha fazla bilgi için [koşullu erişim dağıtımınızı planlayın](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)sayfasını ziyaret edin.</span><span class="sxs-lookup"><span data-stu-id="983dc-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>