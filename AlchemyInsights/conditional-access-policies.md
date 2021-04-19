---
title: Koşullu Erişim ilkeleri
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002357"
- "4583"
ms.openlocfilehash: af95627d07d41add54f03c9254562b9be4e05d9b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51817300"
---
# <a name="conditional-access-policies"></a><span data-ttu-id="ece3e-102">Koşullu Erişim ilkeleri</span><span class="sxs-lookup"><span data-stu-id="ece3e-102">Conditional Access policies</span></span>

<span data-ttu-id="ece3e-103">Koşullu Erişim ortamınızdaki uygulamalara erişim denetimini zorunlu tutmanızı sağlayan bir Azure AD özelliğidir. Erişim tamamen belirli koşullara dayanır ve merkezi bir konumdan yönetilir.</span><span class="sxs-lookup"><span data-stu-id="ece3e-103">Conditional Access is a capability of Azure AD that enables you to enforce controls on the access to apps in your environment, all based on specific conditions and managed from a central location.</span></span>

<span data-ttu-id="ece3e-104">[Azure AD Koşullu Erişimi](https://docs.microsoft.com/azure/active-directory/conditional-access/) hakkında daha fazla bilgi edinin.</span><span class="sxs-lookup"><span data-stu-id="ece3e-104">Learn more about [Azure AD Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span></span>  

<span data-ttu-id="ece3e-105">**Not**: Kiracınız 21 Ekim 2019’dan sonra oluşturulduysa ve beklenmedik şekilde sizden MFA isteniyorsa, büyük olasılıkla kiracınızda [güvenlik varsayılanları](https://aka.ms/securitydefaults) etkindir.</span><span class="sxs-lookup"><span data-stu-id="ece3e-105">**Note**: If your tenant was created after October 21st, 2019 and you're unexpectedly getting prompted for MFA, you likely have [security defaults](https://aka.ms/securitydefaults) enabled in your tenant.</span></span>

<span data-ttu-id="ece3e-106">**Güvenlik varsayılanlarını yönetme**</span><span class="sxs-lookup"><span data-stu-id="ece3e-106">**To Manage security defaults**</span></span>

1. <span data-ttu-id="ece3e-107">Genel yönetici kimlik bilgilerinizle [yönetim merkezinde](https://go.microsoft.com/fwlink/p/?linkid=834822) oturum açın.</span><span class="sxs-lookup"><span data-stu-id="ece3e-107">Sign in to the [admin center](https://go.microsoft.com/fwlink/p/?linkid=834822) with your Global admin credentials.</span></span>

2. <span data-ttu-id="ece3e-108">[Azure Active Directory Özellikleri](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties)’ne gidin.</span><span class="sxs-lookup"><span data-stu-id="ece3e-108">Go to [Azure Active Directory Properties](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).</span></span>

3. <span data-ttu-id="ece3e-109">Sayfanın alt kısmında **Güvenlik varsayılanlarını yönet**’i seçin.</span><span class="sxs-lookup"><span data-stu-id="ece3e-109">At the bottom of the page, click **Manage Security defaults**.</span></span>

4. <span data-ttu-id="ece3e-110">Güvenlik varsayılanlarını etkinleştirmek için **Evet**’i veya güvenlik varsayılanlarını devre dışı bırakmak için **Hayır**’ı seçin.</span><span class="sxs-lookup"><span data-stu-id="ece3e-110">Click **Yes** to enable security defaults or **No** to disable security defaults.</span></span>
