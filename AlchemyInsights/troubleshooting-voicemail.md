---
title: 'Sesli mesaj sorunlarını giderme '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7564"
ms.openlocfilehash: a2d26da512838ae112c352fe21366074b69fa224
ms.sourcegitcommit: 3802f2f4db4f53a408a360187db67f2296448c21
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/09/2020
ms.locfileid: "49679107"
---
# <a name="troubleshooting-voicemail"></a><span data-ttu-id="b4f65-102">Sesli mesaj sorunlarını giderme</span><span class="sxs-lookup"><span data-stu-id="b4f65-102">Troubleshooting Voicemail</span></span>

<span data-ttu-id="b4f65-103">Meşgul olan meşgul özelliğinin bilerek yapıldığından emin olun.</span><span class="sxs-lookup"><span data-stu-id="b4f65-103">Ensure that the Busy on Busy feature is intentional.</span></span>

<span data-ttu-id="b4f65-104">Bu özellik bu kullanıcıya gerekmiyorsa:</span><span class="sxs-lookup"><span data-stu-id="b4f65-104">If this feature is not needed on this user:</span></span>

1. <span data-ttu-id="b4f65-105">[Ekipler Yönetim Merkezi](https://admin.teams.microsoft.com/policies/calling)'ne gidin.</span><span class="sxs-lookup"><span data-stu-id="b4f65-105">Go to [Teams Admin center](https://admin.teams.microsoft.com/policies/calling).</span></span>
1. <span data-ttu-id="b4f65-106">Sol RAIL 'de,   >    >  **çağrı ilkesindeki\*\*\*\*ilkeleri yönetme**</span><span class="sxs-lookup"><span data-stu-id="b4f65-106">On the left rail navigate **Voice** > **Calling policies** > **Manage Policies** on the **Calling Policy**.</span></span>
1. <span data-ttu-id="b4f65-107">**Kullanıcıları Yönet**'i seçin.</span><span class="sxs-lookup"><span data-stu-id="b4f65-107">Select **Manage Users**.</span></span>
1. <span data-ttu-id="b4f65-108">Kullanıcıya çağrı yapın ve arama Ilkesini **meşgul iken** **meşgul olarak** meşgul olan bir görüşme</span><span class="sxs-lookup"><span data-stu-id="b4f65-108">Search for user and change the Calling Policy to one that has **Busy on Busy is available when in a call** to **Off**.</span></span>
1. <span data-ttu-id="b4f65-109">**Uygula**'ya tıklayın.</span><span class="sxs-lookup"><span data-stu-id="b4f65-109">Click **Apply**.</span></span>
> [!NOTE]
> <span data-ttu-id="b4f65-110">İlkelerde yapılan değişikliklerin çoğaltılması 24 saate kadar sürebilir.</span><span class="sxs-lookup"><span data-stu-id="b4f65-110">Changes to policies can take up to 24 hours to replicate.</span></span>

<span data-ttu-id="b4f65-111">Bu özellik hakkında daha fazla bilgi için başvuru bölümüne bakın: [kullanımda meşgul, bir çağrıdayken kullanılabilir](https://docs.microsoft.com/microsoftteams/teams-calling-policy#busy-on-busy-is-available-while-in-a-call).</span><span class="sxs-lookup"><span data-stu-id="b4f65-111">For more information on this feature refer to: [Busy on Busy is available while in a call](https://docs.microsoft.com/microsoftteams/teams-calling-policy#busy-on-busy-is-available-while-in-a-call).</span></span>
