---
title: Masaüstü Analytics on-boarding sırasında erişim belirteç hatasını doğrulayan bir hata oluştu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 7472af5c4e19e5697b5fb4802ed1cbb2c74f1d19
ms.sourcegitcommit: f1fad2129d09660ec42dbce03ce2c6b4cfc9555a
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/18/2019
ms.locfileid: "40741298"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="f51ab-102">Masaüstü Analytics onboarding sırasında "Erişim belirteci doğrulama hatası" hatası oluştu</span><span class="sxs-lookup"><span data-stu-id="f51ab-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="f51ab-103">Kimlik doğrulama belirteci süresi dolduğunda bu hata normalde gözlenir.</span><span class="sxs-lookup"><span data-stu-id="f51ab-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="f51ab-104">Genellikle, sayfanın yenilenmesi belirteci yeniler.</span><span class="sxs-lookup"><span data-stu-id="f51ab-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="f51ab-105">Ancak, yerleşik Masaüstü Analitiği için kullanılan hesaba uygulanan Koşullu Erişim ilkeleri varsa, bu sorun devam edebilir.</span><span class="sxs-lookup"><span data-stu-id="f51ab-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="f51ab-106">Masaüstü Analitiği onboarding için kullanılan hesapiçin oturum açma hatası olup olmadığını görmek için Azure Portalı'ndaki Azure REKLAM Oturum Açma günlüğünü inceleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="f51ab-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="f51ab-107">Koşullu Erişim hakkında daha fazla bilgi [için, Koşullu Erişim dağıtımınızı planlayın'ı ziyaret edin.](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)</span><span class="sxs-lookup"><span data-stu-id="f51ab-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>