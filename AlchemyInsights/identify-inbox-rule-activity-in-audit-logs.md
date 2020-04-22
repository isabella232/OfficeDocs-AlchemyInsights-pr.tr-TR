---
title: Denetim günlüklerinde gelen kutusu kuralı etkinliğini belirleme
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: f946510539b3d28f2ceeec1546cbffce8bd352fd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716444"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="b2e01-102">Denetim günlüklerinde gelen kutusu kuralı etkinliğini belirleme</span><span class="sxs-lookup"><span data-stu-id="b2e01-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="b2e01-103">Gelen kutusu kural olaylarını görüntülemek (gelen kutusu kurallarını oluşturma, değiştirme ve silme) görüntülemek için Microsoft 365 Güvenlik & Uyumluluk Merkezi'ndeki denetim günlüğü aramasını kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="b2e01-103">You can use audit log search in the Microsoft 365 Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="b2e01-104">[Microsoft 365 Güvenlik & Uyumluluk Merkezi'nde](https://protection.office.com/)oturum açın.</span><span class="sxs-lookup"><span data-stu-id="b2e01-104">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="b2e01-105">**Arama** > **Denetimi günlüğü arama** sayfasına gidin.</span><span class="sxs-lookup"><span data-stu-id="b2e01-105">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="b2e01-106">**Başlangıç tarihi** ve Bitiş **tarihi** alanlarındaki tarih aralığını seçin.</span><span class="sxs-lookup"><span data-stu-id="b2e01-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="b2e01-107">**Exchange Posta Kutusu Etkinlikleri**altında, **Etkinlikler** alanının Yeni Gelen Kutusu **Kuralı Oluştur/değiştir/etkinleştir/devre dışı bırak kuralı**olarak ayarlanmış olduğunu doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="b2e01-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="b2e01-108">**Arama'yı**tıklatın.</span><span class="sxs-lookup"><span data-stu-id="b2e01-108">Click **Search**.</span></span>

<span data-ttu-id="b2e01-109">Sonuçlarda, bir denetim kaydı seçin.</span><span class="sxs-lookup"><span data-stu-id="b2e01-109">In the results, select an audit record.</span></span> <span data-ttu-id="b2e01-110">Ayrıntılarflyout, daha **fazla bilgi**tıklatın.</span><span class="sxs-lookup"><span data-stu-id="b2e01-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="b2e01-111">Gelen kutusu kuralı ayarları hakkındaki bilgiler **Parametreler** alanında görüntülenir.</span><span class="sxs-lookup"><span data-stu-id="b2e01-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="b2e01-112">Daha fazla bilgi için bkz: [Bir kullanıcının gelen kutusu kuralı oluşturmuş olup olmadığını belirleme](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="b2e01-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
