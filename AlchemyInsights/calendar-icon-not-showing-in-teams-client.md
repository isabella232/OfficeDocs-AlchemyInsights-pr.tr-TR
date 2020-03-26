---
title: Teams istemcisinde takvim simgesi gösterilmiyor
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "4375"
ms.openlocfilehash: 21692639fb746b2e5aab3dfc8894293d5dc890ac
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932381"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a><span data-ttu-id="15ffc-102">Teams istemcisinde takvim simgesi gösterilmiyor</span><span class="sxs-lookup"><span data-stu-id="15ffc-102">Calendar icon not showing in Teams client</span></span>

<span data-ttu-id="15ffc-103">Teams’teki Takvim Sekmesi Exchange Web Hizmetleri aracılığıyla Exchange posta kutusuna erişim gerektirir.</span><span class="sxs-lookup"><span data-stu-id="15ffc-103">The Calendar Tab in Teams requires access to an Exchange mailbox via Exchange Web Services.</span></span> <span data-ttu-id="15ffc-104">Exchange posta kutusu Çevrimiçi veya Şirket İçi olabilir.</span><span class="sxs-lookup"><span data-stu-id="15ffc-104">The Exchange mailbox can be Online or On-Premises.</span></span> <span data-ttu-id="15ffc-105">Takvim Sekmesini görmeyen Çevrimiçi kullanıcıların [Exchange Online posta kutusu lisansına sahip olduklarından ve posta kutusunun etkin olduğundan](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes) emin olun.</span><span class="sxs-lookup"><span data-stu-id="15ffc-105">For Online users who do not see the Calendar Tab, make sure they [are licensed for an Exchange Online mailbox and the mailbox is enabled](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span></span>

<span data-ttu-id="15ffc-106">Kullanıcının Exchange Online'da geçerli bir posta kutusu varsa, ancak Takvim sekmesini yine de göremiyorsa, bir ağ sorunuyla karşılaşmış olabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="15ffc-106">If the user has a valid mailbox in Exchange Online, but still cannot see the Calendar tab, you may be experiencing a network issue.</span></span> <span data-ttu-id="15ffc-107">[Microsoft Uzaktan Bağlantı Çözümleyicisi](https://testconnectivity.microsoft.com/)’ni kullanın, etkilenen kullanıcı için **Microsoft Exchange Web Hizmetleri Bağlantı Testleri**’ni çalıştırın.</span><span class="sxs-lookup"><span data-stu-id="15ffc-107">Use the [Microsoft Remote Connectivity Analyzer](https://testconnectivity.microsoft.com/) and run the **Microsoft Exchange Web Services Connectivity Tests** for the impacted user.</span></span>

<span data-ttu-id="15ffc-108">Son olarak, Takvim uygulamasının kullanıcıya uygulanan ilkeden (büyük olasılıkla **Global (Kuruluş genelinde varsayılan)**’den) kaldırılmadığından emin olmak için [Teams Uygulaması’nın Uygulama kurulum ilkelerini](https://admin.teams.microsoft.com/policies/app-setup) denetleyin.</span><span class="sxs-lookup"><span data-stu-id="15ffc-108">Finally check the [Teams Apps – App setup policies](https://admin.teams.microsoft.com/policies/app-setup) to ensure the Calendar app has not been removed from the policy applied to the user (most likely the **Global (Org-wide default)**.</span></span>

<span data-ttu-id="15ffc-109">Kullanıcılarınız Şirket İçinde yerleşikse, Karma yapılandırmanızın sağlıklı olduğundan emin olmalısınız.</span><span class="sxs-lookup"><span data-stu-id="15ffc-109">If your users are homed On-Premises, you need to confirm your Hybrid configuration is healthy.</span></span> <span data-ttu-id="15ffc-110">Sorunu gidermek için [Karma Yapılandırma Sihirbazı](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent)’nı kullanın.</span><span class="sxs-lookup"><span data-stu-id="15ffc-110">Use the [Hybrid Configuration Wizard](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) to troubleshoot.</span></span>

<span data-ttu-id="15ffc-111">[Teams’in Exchange 2016 CU3 veya üzerini gerektirdiğini](https://docs.microsoft.com/microsoftteams/exchange-teams-interact) unutmayın.</span><span class="sxs-lookup"><span data-stu-id="15ffc-111">Note that [Teams requires Exchange 2016 CU3 or higher](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span></span>
