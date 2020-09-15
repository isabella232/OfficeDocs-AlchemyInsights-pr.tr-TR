---
title: 646 AADConnect 'i yapılandırma
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 6327e42b74283d732247c9a847c68db72082c56a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704509"
---
# <a name="configure-sync-features"></a><span data-ttu-id="a60c8-102">Eşitleme özelliklerini yapılandırma</span><span class="sxs-lookup"><span data-stu-id="a60c8-102">Configure sync features</span></span>

<span data-ttu-id="a60c8-103">Azure AD Connect, varsayılan olarak etkinleştirilen veya daha sonra etkinleştirebileceğiniz çeşitli özellikler içerir.</span><span class="sxs-lookup"><span data-stu-id="a60c8-103">Azure AD Connect includes several features that are enabled by default, or that you can enable later.</span></span> <span data-ttu-id="a60c8-104">Bazı özellikler belirli ortamlarda ek yapılandırma gerektirir.</span><span class="sxs-lookup"><span data-stu-id="a60c8-104">Some features require additional configuration in specific environments.</span></span>

- <span data-ttu-id="a60c8-105">[Filtreleme](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) sınırları nesneler Azure AD ile eşitlenir.</span><span class="sxs-lookup"><span data-stu-id="a60c8-105">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD.</span></span> <span data-ttu-id="a60c8-106">Varsayılan olarak, tüm kullanıcılar, kişiler, gruplar ve Windows 10 bilgisayar hesapları eşitlenir.</span><span class="sxs-lookup"><span data-stu-id="a60c8-106">By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized.</span></span> <span data-ttu-id="a60c8-107">Etki alanları, kuruluş birimleri veya diğer özniteliklere göre nesneleri ekleyebilir veya dışlayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="a60c8-107">You can include or exclude objects based on domains, OUs, or other attributes.</span></span>

- <span data-ttu-id="a60c8-108">[Parola karması eşitleme](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) , parola karmasını şirket Içi Active Directory 'den Azure AD 'ye eşitler.</span><span class="sxs-lookup"><span data-stu-id="a60c8-108">[Password hash synchronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD.</span></span> <span data-ttu-id="a60c8-109">Bu, tek bir konumda parola yönetimine olanak tanır, ancak şirket içi ve bulut ortamlarında aynı parolanın kullanılmasını sağlar.</span><span class="sxs-lookup"><span data-stu-id="a60c8-109">This allows password management in one location, but use of the same password in both on-premises and cloud environments.</span></span> <span data-ttu-id="a60c8-110">Active Directory, yetkili kaynak olduğundan, kendi parola ilkelerinizi kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="a60c8-110">Because Active Directory is the authoritative source, you can use your own password policies.</span></span>

- <span data-ttu-id="a60c8-111">[Self servis parola sıfırlama (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) , şirket içi parola ilkenizi uygularken kullanıcıların kendi parolalarını kendi parolalarını sıfırlamalarına olanak tanır.</span><span class="sxs-lookup"><span data-stu-id="a60c8-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span>

- <span data-ttu-id="a60c8-112">[Cihaz geri yazma](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) , Azure AD 'deki kaydettirilmiş cihazların, şirket Içi Active Directory 'ye geri yazılmasına olanak tanır, böylece koşullu erişim için kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="a60c8-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span>

- <span data-ttu-id="a60c8-113">Çok sayıda eşzamanlı nesne silme işlemi yapılmasını engellemeye yardımcı olmak için [yanlışlıkla silme Işlemlerini önleyin](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) (eşitleme başına 500 nesnelerden fazla).</span><span class="sxs-lookup"><span data-stu-id="a60c8-113">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization).</span></span> <span data-ttu-id="a60c8-114">Kuruluşunuzun gereksinimlerini karşılayacak şekilde bu ayarı değiştirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="a60c8-114">You can change this setting to meet the needs of your organization.</span></span>

- <span data-ttu-id="a60c8-115">[Otomatik yükseltme](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) , hızlı yüklemeler için varsayılan olarak etkinleştirilir ve Azure AD Connect sürümünüzün her zaman güncel olmasını sağlamaya yardımcı olur.</span><span class="sxs-lookup"><span data-stu-id="a60c8-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span>
