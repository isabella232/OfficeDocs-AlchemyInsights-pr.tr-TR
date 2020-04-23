---
title: Beklenmeyen çok faktörlü kimlik doğrulaması
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: ''
ms.custom:
- "1300007"
- "4372"
ms.openlocfilehash: a664bd709062ec1335ebcf1f9adddc8aef917ac1
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: HT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766621"
---
# <a name="unexpected-multi-factor-authentication"></a><span data-ttu-id="94981-102">Beklenmeyen çok faktörlü kimlik doğrulaması</span><span class="sxs-lookup"><span data-stu-id="94981-102">Unexpected multi-factor authentication</span></span>

<span data-ttu-id="94981-103">Kiracınız 21 Ekim 2019’dan sonra oluşturulduysa ve beklenmedik şekilde sizden MFA isteniyorsa, büyük olasılıkla kiracınızda [güvenlik varsayılanları](https://aka.ms/securitydefaults) etkindir.</span><span class="sxs-lookup"><span data-stu-id="94981-103">If your tenant was created after October 21st, 2019 and you're unexpectedly getting prompted for MFA, you likely have [security defaults](https://aka.ms/securitydefaults) enabled in your tenant.</span></span> 

<span data-ttu-id="94981-104">Güvenlik varsayılanlarını yönetmek için:</span><span class="sxs-lookup"><span data-stu-id="94981-104">To Manage security defaults:</span></span>

1. <span data-ttu-id="94981-105">Genel yönetici kimlik bilgilerinizle [yönetim merkezinde](https://go.microsoft.com/fwlink/p/?linkid=834822) oturum açın.</span><span class="sxs-lookup"><span data-stu-id="94981-105">Sign in to the [admin center](https://go.microsoft.com/fwlink/p/?linkid=834822) with your Global admin credentials.</span></span>

2. <span data-ttu-id="94981-106">[Azure Active Directory Özellikleri](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties)’ne gidin.</span><span class="sxs-lookup"><span data-stu-id="94981-106">Go to [Azure Active Directory Properties](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).</span></span>

3. <span data-ttu-id="94981-107">Sayfanın alt kısmında **Güvenlik varsayılanlarını yönet**’i seçin.</span><span class="sxs-lookup"><span data-stu-id="94981-107">At the bottom of the page, click **Manage Security defaults**.</span></span>

4. <span data-ttu-id="94981-108">Güvenlik varsayılanlarını etkinleştirmek için **Evet**’i, güvenlik varsayılanlarını devre dışı bırakmak için **Hayır**’ı seçin.</span><span class="sxs-lookup"><span data-stu-id="94981-108">Click **Yes** to enable security defaults and **No** to disable security defaults.</span></span>
