---
title: 646 AADConnect biçimde nasıl yapılandırılır
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: e4ba295cd0661c3454180dd6a15895123840389e
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28317561"
---
# <a name="configure-sync-features"></a><span data-ttu-id="fca4d-102">Eşitleme özellikleri yapılandırma</span><span class="sxs-lookup"><span data-stu-id="fca4d-102">Configure sync features</span></span>

<span data-ttu-id="fca4d-p101">Azure AD Bağlan varsayılan olarak etkin veya daha sonra etkinleştirmek üzere çeşitli özellikler içerir. Bazı özellikler belirli ortamlarda ek yapılandırma gerektirir.</span><span class="sxs-lookup"><span data-stu-id="fca4d-p101">Azure AD Connect includes several features that are enabled by default, or that you can enable later. Some features require additional configuration in specific environments.</span></span>
  
- <span data-ttu-id="fca4d-p102">Azure AD için [filtreleme](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) sınırları nesneler eşitlenir. Bilgisayar hesapları, varsayılan, tüm kullanıcılar, kişiler, gruplar ve Windows 10 tarafından eşitlenir. Ekleyebilir veya etki alanları, kuruluş birimleri veya diğer öznitelikleri temel nesneleri hariç tut.</span><span class="sxs-lookup"><span data-stu-id="fca4d-p102">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD. By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized. You can include or exclude objects based on domains, OUs, or other attributes.</span></span> 
    
- <span data-ttu-id="fca4d-p103">[Parola karma eşitleme](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) yerinde Active Directory'den Azure AD parola karma eşitler. Bu parola yönetimi tek bir yerde verir, ancak her ikisi de aynı parola kullanımını yerinde ve ortamlar bulut. Active Directory yetkili kaynak olduğu için kendi parola ilkelerini kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="fca4d-p103">[Password hash syncronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD. This allows password management in one location, but use of the same password in both on-premises and cloud environments. Because Active Directory is the authoritative source, you can use your own password policies.</span></span> 
    
- <span data-ttu-id="fca4d-111">[Kendi kendine parola sıfırlama (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) hala yerinde, parola ilkesi uygulanırken bulut kendi parolalarını sıfırlamak kullanıcılar sağlar.</span><span class="sxs-lookup"><span data-stu-id="fca4d-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span> 
    
- <span data-ttu-id="fca4d-112">[Geri yazma aygıtı](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) Azure AD yerinde Active Directory'ye koşullu erişim için kullanılacak şekilde yeniden yazılması için kayıtlı aygıtlar sağlar.</span><span class="sxs-lookup"><span data-stu-id="fca4d-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span> 
    
- <span data-ttu-id="fca4d-p104">[Silmeleri Engelle yanlışlıkla](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) çok fazla sayıda eşzamanlı nesne silme (eşitleme başına 500'den fazla nesneleri) önlemek için varsayılan olarak etkindir. Kuruluşunuzun gereksinimlerini karşılamak için bu ayarı değiştirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="fca4d-p104">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization). You can change this setting to meet the needs of your organization.</span></span> 
    
- <span data-ttu-id="fca4d-115">[Otomatik yükseltme](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) hızlı yüklemeler için varsayılan olarak etkindir ve yardımcı Azure AD Bağlan sürümünüzün her zaman güncel olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="fca4d-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span> 
    

