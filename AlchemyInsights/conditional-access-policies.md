---
title: Koşullu Erişim ilkeleri
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002357"
- "4583"
ms.openlocfilehash: 569507318b499cdbcf2a1cd75e84046953f62212
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: HT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706077"
---
# <a name="conditional-access-policies"></a><span data-ttu-id="497f4-102">Koşullu Erişim ilkeleri</span><span class="sxs-lookup"><span data-stu-id="497f4-102">Conditional Access policies</span></span>

<span data-ttu-id="497f4-103">Koşullu Erişim ortamınızdaki uygulamalara erişim denetimini zorunlu tutmanızı sağlayan bir Azure AD özelliğidir. Erişim tamamen belirli koşullara dayanır ve merkezi bir konumdan yönetilir.</span><span class="sxs-lookup"><span data-stu-id="497f4-103">Conditional Access is a capability of Azure AD that enables you to enforce controls on the access to apps in your environment, all based on specific conditions and managed from a central location.</span></span>

<span data-ttu-id="497f4-104">[Azure AD Koşullu Erişimi](https://docs.microsoft.com/azure/active-directory/conditional-access/) hakkında daha fazla bilgi edinin.</span><span class="sxs-lookup"><span data-stu-id="497f4-104">Learn more about [Azure AD Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span></span>  

<span data-ttu-id="497f4-105">**Not**: Kiracınız 21 Ekim 2019’dan sonra oluşturulduysa ve beklenmedik şekilde sizden MFA isteniyorsa, büyük olasılıkla kiracınızda [güvenlik varsayılanları](https://aka.ms/securitydefaults) etkindir.</span><span class="sxs-lookup"><span data-stu-id="497f4-105">**Note**: If your tenant was created after October 21st, 2019 and you're unexpectedly getting prompted for MFA, you likely have [security defaults](https://aka.ms/securitydefaults) enabled in your tenant.</span></span>

<span data-ttu-id="497f4-106">**Güvenlik varsayılanlarını yönetme**</span><span class="sxs-lookup"><span data-stu-id="497f4-106">**To Manage security defaults**</span></span>

1. <span data-ttu-id="497f4-107">Genel yönetici kimlik bilgilerinizle [yönetim merkezinde](https://go.microsoft.com/fwlink/p/?linkid=834822) oturum açın.</span><span class="sxs-lookup"><span data-stu-id="497f4-107">Sign in to the [admin center](https://go.microsoft.com/fwlink/p/?linkid=834822) with your Global admin credentials.</span></span>

2. <span data-ttu-id="497f4-108">[Azure Active Directory Özellikleri](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties)’ne gidin.</span><span class="sxs-lookup"><span data-stu-id="497f4-108">Go to [Azure Active Directory Properties](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).</span></span>

3. <span data-ttu-id="497f4-109">Sayfanın alt kısmında **Güvenlik varsayılanlarını yönet**’i seçin.</span><span class="sxs-lookup"><span data-stu-id="497f4-109">At the bottom of the page, click **Manage Security defaults**.</span></span>

4. <span data-ttu-id="497f4-110">Güvenlik varsayılanlarını etkinleştirmek için **Evet**’i veya güvenlik varsayılanlarını devre dışı bırakmak için **Hayır**’ı seçin.</span><span class="sxs-lookup"><span data-stu-id="497f4-110">Click **Yes** to enable security defaults or **No** to disable security defaults.</span></span>
