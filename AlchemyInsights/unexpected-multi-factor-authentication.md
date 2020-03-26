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
ms.openlocfilehash: 8a912b32dee23e8c6eae0ad7bc72228d49ceeb92
ms.sourcegitcommit: 4f7ff981bbb3a98663cd164d0a10bb082cdf7ec9
ms.translationtype: HT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/25/2020
ms.locfileid: "42946851"
---
# <a name="unexpected-multi-factor-authentication"></a><span data-ttu-id="9ba49-102">Beklenmeyen çok faktörlü kimlik doğrulaması</span><span class="sxs-lookup"><span data-stu-id="9ba49-102">Unexpected multi-factor authentication</span></span>

<span data-ttu-id="9ba49-103">Kiracınız 21 Ekim 2019’dan sonra oluşturulduysa ve beklenmedik şekilde sizden MFA isteniyorsa, büyük olasılıkla kiracınızda [güvenlik varsayılanları](http://aka.ms/securitydefaults) etkindir.</span><span class="sxs-lookup"><span data-stu-id="9ba49-103">If your tenant was created after October 21st, 2019 and you're unexpectedly getting prompted for MFA, you likely have [security defaults](http://aka.ms/securitydefaults) enabled in your tenant.</span></span> 

<span data-ttu-id="9ba49-104">Güvenlik varsayılanlarını yönetmek için:</span><span class="sxs-lookup"><span data-stu-id="9ba49-104">To Manage security defaults:</span></span>

1. <span data-ttu-id="9ba49-105">Genel yönetici kimlik bilgilerinizle [yönetim merkezinde](https://go.microsoft.com/fwlink/p/?linkid=834822) oturum açın.</span><span class="sxs-lookup"><span data-stu-id="9ba49-105">Sign in to the [admin center](https://go.microsoft.com/fwlink/p/?linkid=834822) with your Global admin credentials.</span></span>

2. <span data-ttu-id="9ba49-106">[Azure Active Directory Özellikleri](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties)’ne gidin.</span><span class="sxs-lookup"><span data-stu-id="9ba49-106">Go to [Azure Active Directory Properties](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).</span></span>

3. <span data-ttu-id="9ba49-107">Sayfanın alt kısmında **Güvenlik varsayılanlarını yönet**’i seçin.</span><span class="sxs-lookup"><span data-stu-id="9ba49-107">At the bottom of the page, click **Manage Security defaults**.</span></span>

4. <span data-ttu-id="9ba49-108">Güvenlik varsayılanlarını etkinleştirmek için **Evet**’i, güvenlik varsayılanlarını devre dışı bırakmak için **Hayır**’ı seçin.</span><span class="sxs-lookup"><span data-stu-id="9ba49-108">Click **Yes** to enable security defaults and **No** to disable security defaults.</span></span>
