---
title: Gelen Kutusu Kuralı Denetim günlüklerini etkinliğinde belirle
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 1201a625948743cacfaa58410abeb4108ed2eb56
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539193"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="e53e4-102">Gelen Kutusu Kuralı Denetim günlüklerini etkinliğinde belirle</span><span class="sxs-lookup"><span data-stu-id="e53e4-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="e53e4-103">(Oluşturma, değiştirme ve silme gelen kutusu kuralları) gelen kutusu kuralı olayları görüntülemek için Denetim günlüğü aramayı Office 365 güvenlik & Uyumluluk Merkezi'ni kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="e53e4-103">You can use audit log search in the Office 365 Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="e53e4-104">[Office 365 güvenlik & Uyumluluk Merkezi](https://protection.office.com/)oturum açın.</span><span class="sxs-lookup"><span data-stu-id="e53e4-104">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="e53e4-105">**Arama**gidin > **Denetim günlüğü arama** sayfası.</span><span class="sxs-lookup"><span data-stu-id="e53e4-105">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="e53e4-106">**Başlangıç tarihi** ve **Bitiş tarihi** alanlarında tarih aralığını seçin.</span><span class="sxs-lookup"><span data-stu-id="e53e4-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="e53e4-107">**Exchange posta kutusu Aktiviteler** **Aktiviteler** alanında ayarlanır doğrulamak **InboxRule Yeni Oluştur/Değiştir/etkinleştir/gelen kutusu kuralı devre dışı**.</span><span class="sxs-lookup"><span data-stu-id="e53e4-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="e53e4-108">**Ara**' yı tıklatın.</span><span class="sxs-lookup"><span data-stu-id="e53e4-108">Click **Search**.</span></span>

<span data-ttu-id="e53e4-109">Sonuçlarda bir denetim kaydı seçin.</span><span class="sxs-lookup"><span data-stu-id="e53e4-109">In the results, select an audit record.</span></span> <span data-ttu-id="e53e4-110">Ayrıntılar çıkma **Daha fazla Bilgi'yi**tıklatın.</span><span class="sxs-lookup"><span data-stu-id="e53e4-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="e53e4-111">Gelen kutusu kuralı ayarları hakkında bilgi **parametreleri** alanında görüntülenir.</span><span class="sxs-lookup"><span data-stu-id="e53e4-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="e53e4-112">Daha fazla bilgi için bkz: [kullanıcı tarafından oluşturulan bir gelen kutusu kuralı olmadığını belirleme](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="e53e4-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
