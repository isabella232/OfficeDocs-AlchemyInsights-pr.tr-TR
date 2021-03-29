---
title: Posta kutularına adresleri iletmeyi denetleme
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 3abd45230360c61ecb62e4b7a39d1b0b547271fc
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403331"
---
# <a name="check-for-forwarding-addresses-on-mailboxes"></a><span data-ttu-id="dc408-102">Posta kutularına adresleri iletmeyi denetleme</span><span class="sxs-lookup"><span data-stu-id="dc408-102">Check for forwarding addresses on mailboxes</span></span>

<span data-ttu-id="dc408-103">Bazen bilgisayar korsanları kullanıcıların e-posta iletilerini kendilerine iletir, bu nedenle öncelikle posta kutusunda adreslerin ve kuralların ilet olup denetlememiz gerekir.</span><span class="sxs-lookup"><span data-stu-id="dc408-103">Sometimes hackers forward users' email messages to themselves, so first we'll check for forwarding addresses and rules on the mailbox.</span></span> <span data-ttu-id="dc408-104">Daha sonra denetim günlüklerini kontrol edeceğim.</span><span class="sxs-lookup"><span data-stu-id="dc408-104">Then we'll check the audit logs.</span></span> <span data-ttu-id="dc408-105">Adresleri şu şekilde kontrol edin:</span><span class="sxs-lookup"><span data-stu-id="dc408-105">Here's how to check for forwarding addresses:</span></span>

1. <span data-ttu-id="dc408-106">Kullanıcıları **Etkin**  >  **Kullanıcılar'ı seçin.**</span><span class="sxs-lookup"><span data-stu-id="dc408-106">Select **Users** > **Active users**.</span></span>
1. <span data-ttu-id="dc408-107">Hesabı güvenliği ihlal edilmiş olan kullanıcıyı seçin.</span><span class="sxs-lookup"><span data-stu-id="dc408-107">Select the user whose account has been compromised.</span></span>
1. <span data-ttu-id="dc408-108">Görüntülenen açılır iletide, Posta **Ayarları'nın genişletin** ve ardından E-posta iletme **için** **Düzenle'ye tıklayın.**</span><span class="sxs-lookup"><span data-stu-id="dc408-108">In the flyout that appears, expand **Mail Settings**, and then click **Edit** for **Email forwarding**.</span></span>
1. <span data-ttu-id="dc408-109">Tanımadınız tüm iletme adreslerini kaldırın.</span><span class="sxs-lookup"><span data-stu-id="dc408-109">Remove any forwarding addresses you don't recognize.</span></span>