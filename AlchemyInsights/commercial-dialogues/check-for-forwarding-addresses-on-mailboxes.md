---
title: Posta kutularına adresleri iletmeyi denetleme
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 17/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 1b0a6c8fe368196f2d1f9811aea895c2c024b2e6
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50483927"
---
# <a name="check-for-forwarding-addresses-on-mailboxes"></a><span data-ttu-id="d2d70-102">Posta kutularına adresleri iletmeyi denetleme</span><span class="sxs-lookup"><span data-stu-id="d2d70-102">Check for forwarding addresses on mailboxes</span></span>

<span data-ttu-id="d2d70-103">Bazen bilgisayar korsanları kullanıcıların e-posta iletilerini kendilerine iletir, bu nedenle öncelikle posta kutusunda adreslerin ve kuralların ilet olup denetlememiz gerekir.</span><span class="sxs-lookup"><span data-stu-id="d2d70-103">Sometimes hackers forward users' email messages to themselves, so first we'll check for forwarding addresses and rules on the mailbox.</span></span> <span data-ttu-id="d2d70-104">Daha sonra denetim günlüklerini kontrol edeceğim.</span><span class="sxs-lookup"><span data-stu-id="d2d70-104">Then we'll check the audit logs.</span></span> <span data-ttu-id="d2d70-105">Adresleri şu şekilde kontrol edin:</span><span class="sxs-lookup"><span data-stu-id="d2d70-105">Here's how to check for forwarding addresses:</span></span>

1. <span data-ttu-id="d2d70-106">Kullanıcıları **Etkin**  >  **Kullanıcılar'ı seçin.**</span><span class="sxs-lookup"><span data-stu-id="d2d70-106">Select **Users** > **Active users**.</span></span>
1. <span data-ttu-id="d2d70-107">Hesabı güvenliği ihlal edilmiş olan kullanıcıyı seçin.</span><span class="sxs-lookup"><span data-stu-id="d2d70-107">Select the user whose account has been compromised.</span></span>
1. <span data-ttu-id="d2d70-108">Görüntülenen açılır iletide, Posta **Ayarları'nın genişletin** ve ardından E-posta iletme **için** **Düzenle'ye tıklayın.**</span><span class="sxs-lookup"><span data-stu-id="d2d70-108">In the flyout that appears, expand **Mail Settings**, and then click **Edit** for **Email forwarding**.</span></span>
1. <span data-ttu-id="d2d70-109">Tanımadınız tüm iletme adreslerini kaldırın.</span><span class="sxs-lookup"><span data-stu-id="d2d70-109">Remove any forwarding addresses you don't recognize.</span></span>