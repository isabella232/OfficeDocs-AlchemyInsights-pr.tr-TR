---
title: IP adresi ve denetim günlüklerini istemcisinde belirle
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1367
ms.assetid: ''
ms.openlocfilehash: 7e30a638de5926aa11b8ae637613a48076d7bdc9
ms.sourcegitcommit: ffe2f489b1ac3aae62aa784c959da6a41c3261eb
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/17/2019
ms.locfileid: "31909643"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="71b32-102">IP adresi ve denetim günlüklerini istemcisinde belirle</span><span class="sxs-lookup"><span data-stu-id="71b32-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="71b32-103">Bir kullanıcı veya yönetici tarafından bir etkinlik karşılık gelen IP adresini denetim günlüklerinde gösterilir.</span><span class="sxs-lookup"><span data-stu-id="71b32-103">The IP address that corresponds to an activity by a user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="71b32-104">İstemci bilgileri de kaydedilir.</span><span class="sxs-lookup"><span data-stu-id="71b32-104">The client information is also logged.</span></span> <span data-ttu-id="71b32-105">Bu tür bilgileri tanımlamak üzere adımlar şunlardır</span><span class="sxs-lookup"><span data-stu-id="71b32-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="71b32-106">Oturum [Office 365 güvenlik & Uyumluluk Merkezi](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="71b32-106">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="71b32-107">**Arama ve araştırma'yı** tıklatın ve **Denetim günlüğü Ara**' yı seçin.</span><span class="sxs-lookup"><span data-stu-id="71b32-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

   <span data-ttu-id="71b32-108">Belirli bir etkinlik ilgileniyorsanız, **etkinlikler** listesinden seçin.</span><span class="sxs-lookup"><span data-stu-id="71b32-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="71b32-109">Aksi halde, tüm etkinlikleri seçilen kullanıcı için (varsayılan ayar) döndürülür.</span><span class="sxs-lookup"><span data-stu-id="71b32-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="71b32-110">**Not**: Bazı aktiviteler **Aktiviteler** menüde; kullanılamayabilir Ancak, bu öğeleri denetleme **Sonuçları göster tüm etkinlikler için** seçili olarak (varsayılan ayar) ise döndürülür.</span><span class="sxs-lookup"><span data-stu-id="71b32-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="71b32-111">Kullanıcıadı **Kullanıcılar** alanında belirtin, etkinlik için uygun tarih aralığını seçin ve sonra **Ara**' yı tıklatın.</span><span class="sxs-lookup"><span data-stu-id="71b32-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="71b32-112">Sonuçları, sonuçlar bölmesinde bu etkinlik için IP adresini görebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="71b32-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="71b32-113">**Ayrıntılar** çıkma (örneğin, istemci, gerçekleştirilen eylem vb. kullanıcı) ayrıntılı bilgileri görmek için denetim kaydı seçin.</span><span class="sxs-lookup"><span data-stu-id="71b32-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="71b32-114">Daha fazla bilgi için bkz: [tehlikeye atılan hesabın erişmek için kullanılan bilgisayarın IP adresini bulma](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span><span class="sxs-lookup"><span data-stu-id="71b32-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
