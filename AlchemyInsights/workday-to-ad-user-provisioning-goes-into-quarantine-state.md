---
title: İşGünü'nde AD Kullanıcı Hazırlama karantina durumuna gidiyor
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8471"
- "9004687"
ms.openlocfilehash: 0fc519c8170de498c9bcb1fc41a76116bda48b1f
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482907"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a><span data-ttu-id="75de6-102">İşGünü'nde AD Kullanıcı Hazırlama karantina durumuna gidiyor</span><span class="sxs-lookup"><span data-stu-id="75de6-102">Workday to AD User Provisioning goes into quarantine state</span></span>

<span data-ttu-id="75de6-103">**İşGünü'nde AD Kullanıcı Hazırlama karantina durumuna gidiyor ve AD'de hiçbir kullanıcı oluşturulamıyor**</span><span class="sxs-lookup"><span data-stu-id="75de6-103">**Workday to AD User Provisioning goes into quarantine state and no users are created in AD**</span></span>

<span data-ttu-id="75de6-104">İşGünü'nde AD Kullanıcı Hazırlama işi karantina durumuna geldi ve denetim günlükleri hata iletisiyle dışarı aktarma hatası olaylarını **gösteriyor: OperationsError-SvcErr: İşlem hatası oluştu. Dizin hizmeti için üstün başvuru yapılandırılmamış. Bu nedenle dizin hizmeti, bu ormanın dışındaki nesnelere başvuru yapamaz.**</span><span class="sxs-lookup"><span data-stu-id="75de6-104">The Workday to AD User Provisioning job has gone into quarantine state and the audit logs show export failure events with the error message **Error: OperationsError-SvcErr: An operation error occurred. No superior reference has been configured for the directory service. The directory service is therefore unable to issue referrals to objects outside this forest**.</span></span> <span data-ttu-id="75de6-105">Bu hata genellikle Active Directory Kapsayıcı OU'su doğru ayarlanmamışsa veya **parentDistinguishedName** için kullanılan İfade Eşlemesinde sorun varsa ortaya konur.</span><span class="sxs-lookup"><span data-stu-id="75de6-105">This error usually shows up if the Active Directory Container OU is not set correctly or if there are issues with the Expression Mapping used for **parentDistinguishedName**.</span></span>

<span data-ttu-id="75de6-106">Yazım hataları için Yeni Kullanıcılar için **Varsayılan** OU parametresini kontrol edin.</span><span class="sxs-lookup"><span data-stu-id="75de6-106">Check the Default OU for **New Users** parameter for typos.</span></span> <span data-ttu-id="75de6-107">Belirtilen OU'nun AD'nizin içinde zaten var olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="75de6-107">Ensure that the specified OU already exists in your AD.</span></span> <span data-ttu-id="75de6-108">Öznitelik eşlemesinde **parentDistinguishedName** kullanıyorsanız, her zaman AD etki alanı içinde bilinen bir kapsayıcıyı değerlendirdiğinden emin olun.</span><span class="sxs-lookup"><span data-stu-id="75de6-108">If you are using **parentDistinguishedName** in the attribute mapping, ensure that it always evaluates to a known container within the AD domain.</span></span> <span data-ttu-id="75de6-109">Oluşturulan değeri görmek için denetim günlüklerinde Dışarı Aktar olayına bakın.</span><span class="sxs-lookup"><span data-stu-id="75de6-109">Check the Export event in the audit logs to see the generated value.</span></span>

<span data-ttu-id="75de6-110">Otomatik sağlama için iş günü yapılandırma hakkında daha fazla ayrıntı için öğreticiye bakın: Otomatik kullanıcı [sağlama için İşGünü'ne yapılandırma.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)</span><span class="sxs-lookup"><span data-stu-id="75de6-110">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>

