---
title: 646 AADConnect nasıl yapılandırılatır
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 713cda26e55f07f0438cb9ebe5aa9da86c4ebb3a
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43722583"
---
# <a name="configure-sync-features"></a><span data-ttu-id="4792e-102">Eşitleme özelliklerini yapılandırma</span><span class="sxs-lookup"><span data-stu-id="4792e-102">Configure sync features</span></span>

<span data-ttu-id="4792e-103">Azure AD Connect varsayılan olarak etkinleştirilen veya daha sonra etkinleştirebileceğiniz birkaç özellik içerir.</span><span class="sxs-lookup"><span data-stu-id="4792e-103">Azure AD Connect includes several features that are enabled by default, or that you can enable later.</span></span> <span data-ttu-id="4792e-104">Bazı özellikler belirli ortamlarda ek yapılandırma gerektirir.</span><span class="sxs-lookup"><span data-stu-id="4792e-104">Some features require additional configuration in specific environments.</span></span>

- <span data-ttu-id="4792e-105">[Filtreleme,](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) nesnelerin Azure AD ile eşitlenerek sınırlandırılmalarını sınırlar.</span><span class="sxs-lookup"><span data-stu-id="4792e-105">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD.</span></span> <span data-ttu-id="4792e-106">Varsayılan olarak, tüm kullanıcılar, kişiler, gruplar ve Windows 10 bilgisayar hesapları eşitlenir.</span><span class="sxs-lookup"><span data-stu-id="4792e-106">By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized.</span></span> <span data-ttu-id="4792e-107">Etki alanlarına, BIZE veya diğer özniteliklere dayalı nesneleri içerebilir veya hariç tutabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="4792e-107">You can include or exclude objects based on domains, OUs, or other attributes.</span></span>

- <span data-ttu-id="4792e-108">[Parola karma eşitleme,](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) şirket içi Active Directory'den Azure AD'ye parola karmasını eşitler.</span><span class="sxs-lookup"><span data-stu-id="4792e-108">[Password hash synchronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD.</span></span> <span data-ttu-id="4792e-109">Bu, parola yönetiminin tek bir konumda yapılmasına izin verir, ancak hem şirket içinde hem de bulut ortamlarında aynı parolanın kullanılmasına olanak tanır.</span><span class="sxs-lookup"><span data-stu-id="4792e-109">This allows password management in one location, but use of the same password in both on-premises and cloud environments.</span></span> <span data-ttu-id="4792e-110">Etkin Dizin yetkili kaynak olduğundan, kendi parola ilkelerinizi kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="4792e-110">Because Active Directory is the authoritative source, you can use your own password policies.</span></span>

- <span data-ttu-id="4792e-111">[Self servis parola sıfırlama (SSPR),](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) kullanıcıların şirket içi parola ilkenizi uygularken bulutta kendi parolalarını sıfırlamalarına olanak tanır.</span><span class="sxs-lookup"><span data-stu-id="4792e-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span>

- <span data-ttu-id="4792e-112">[Aygıt geri yüklemesi,](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) Azure AD'deki kayıtlı aygıtların şirket içi Active Directory'ye yazılmasına izin verir, böylece koşullu erişim için kullanılabilirler.</span><span class="sxs-lookup"><span data-stu-id="4792e-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span>

- <span data-ttu-id="4792e-113">Çok fazla eşzamanlı nesne silme (eşitleme başına 500'den fazla nesne) önlemeye yardımcı olmak için varsayılan olarak [yanlışlıkla silmeleri](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) önlemek.</span><span class="sxs-lookup"><span data-stu-id="4792e-113">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization).</span></span> <span data-ttu-id="4792e-114">Kuruluşunuzun gereksinimlerini karşılamak için bu ayarı değiştirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="4792e-114">You can change this setting to meet the needs of your organization.</span></span>

- <span data-ttu-id="4792e-115">[Otomatik yükseltme,](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) ekspres yüklemeler için varsayılan olarak etkinleştirilir ve Azure AD Connect sürümünün her zaman geçerli olmasını sağlamaya yardımcı olur.</span><span class="sxs-lookup"><span data-stu-id="4792e-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span>
