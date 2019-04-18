---
title: Gelen Kutusu Kuralı Denetim günlüklerini etkinliğinde belirle
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1368
ms.assetid: ''
ms.openlocfilehash: 9339d9c58056f568dc994b75bffe39f2c8bbdd34
ms.sourcegitcommit: ffe2f489b1ac3aae62aa784c959da6a41c3261eb
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/17/2019
ms.locfileid: "31909642"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="78a07-102">Gelen Kutusu Kuralı Denetim günlüklerini etkinliğinde belirle</span><span class="sxs-lookup"><span data-stu-id="78a07-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="78a07-103">Gelen kutusu kuralı olayları (oluşturma, değiştirme ve silme gelen kutusu kuralları) görüntülemek için güvenlik & Uyumluluk Merkezi Denetim günlüğü aramayı kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="78a07-103">You can use audit log search in the Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="78a07-104">Oturum [Office 365 güvenlik & Uyumluluk Merkezi](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="78a07-104">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="78a07-105">**Arama ve araştırma'yı** tıklatın ve **Denetim günlüğü Ara**' yı seçin.</span><span class="sxs-lookup"><span data-stu-id="78a07-105">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="78a07-106">**Başlangıç tarihi** ve **Bitiş tarihi** alanlarında tarih aralığını seçin.</span><span class="sxs-lookup"><span data-stu-id="78a07-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="78a07-107">**Exchange posta kutusu Aktiviteler** **Aktiviteler** alanında ayarlanır doğrulamak **InboxRule Yeni Oluştur/Değiştir/etkinleştir/gelen kutusu kuralı devre dışı**.</span><span class="sxs-lookup"><span data-stu-id="78a07-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="78a07-108">**Ara**' yı tıklatın.</span><span class="sxs-lookup"><span data-stu-id="78a07-108">Click **Search**.</span></span>

<span data-ttu-id="78a07-109">Sonuçlarda bir denetim kaydı seçin.</span><span class="sxs-lookup"><span data-stu-id="78a07-109">In the results, select an audit record.</span></span> <span data-ttu-id="78a07-110">Ayrıntılar çıkma **Daha fazla Bilgi'yi**tıklatın.</span><span class="sxs-lookup"><span data-stu-id="78a07-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="78a07-111">Gelen kutusu kuralı ayarları hakkında bilgi **parametreleri** alanında görüntülenir.</span><span class="sxs-lookup"><span data-stu-id="78a07-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="78a07-112">Daha fazla bilgi için bkz: [kullanıcı tarafından oluşturulan bir gelen kutusu kuralı olmadığını belirleme](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="78a07-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
