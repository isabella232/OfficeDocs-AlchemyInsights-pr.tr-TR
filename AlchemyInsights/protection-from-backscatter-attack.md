---
title: Geri sıçrama saldırılarından koruma
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9779"
- "9005743"
ms.openlocfilehash: 8d9214fe2f5d55a21c72296421dd837d7f1d7e7d
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037182"
---
# <a name="protection-from-backscatter-attack"></a><span data-ttu-id="14b7f-102">Geri sıçrama saldırısını koruma</span><span class="sxs-lookup"><span data-stu-id="14b7f-102">Protection from Backscatter attack</span></span>

<span data-ttu-id="14b7f-103">Geri bildirim, gönderme olmadığınız iletiler için size gönderilen teslim edililmeyen raporlardır (NDR'ler veya geri dönen iletiler olarak da bilinir).</span><span class="sxs-lookup"><span data-stu-id="14b7f-103">Backscatter is non-delivery reports (also known as NDRs or bounce messages) you receive for messages that you did not send.</span></span> <span data-ttu-id="14b7f-104">İstenmeyen posta gönderenler, **Gönderen:** iletilerinin adresini ele verir ve çoğunlukla iletilerine güven vermek için gerçek e-posta adresleri kullanırlar.</span><span class="sxs-lookup"><span data-stu-id="14b7f-104">Spammers forge (spoof) the **From:** address of their messages, and they often use real email addresses to lend credibility to their messages.</span></span> <span data-ttu-id="14b7f-105">Dolayısıyla, istenmeyen posta gönderenlerin var olmayan alıcılara ileti göndermesi kaçınılmaz olduğunda, hedef e-posta sunucusu temelde NDR'deki teslim edilemeyen iletiyi Gönderen **adresine** sahte gönderene geri göndermeniz için kandırıldı.</span><span class="sxs-lookup"><span data-stu-id="14b7f-105">So, when spammers inevitably send messages to non-existent recipients, the destination email server is essentially tricked into returning the undeliverable message in an NDR to the forged sender in the **From:** address.</span></span>

<span data-ttu-id="14b7f-106">Ek Bilgiler [EOP'de Geri Alınan Bilgi'de bulunabilir.](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop)</span><span class="sxs-lookup"><span data-stu-id="14b7f-106">Additional Information can be found in [Backscatter in EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop).</span></span>

<span data-ttu-id="14b7f-107">**Geritter korumasını etkinleştirme**</span><span class="sxs-lookup"><span data-stu-id="14b7f-107">**Enabling Backscatter protection**</span></span>

<span data-ttu-id="14b7f-108">Backscatter korumasını etkinleştirmek için aşağıdaki yolu izleyin.</span><span class="sxs-lookup"><span data-stu-id="14b7f-108">To enable Backscatter protection, follow the path below.</span></span>

<span data-ttu-id="14b7f-109">**protection.office.com > Tehdit Yönetimi > İlkesi > Istenmeyen Posta Önleme > İstenmeyen Posta Özellikleri > İstenmeyen Posta özellikleri > İstenmeyen Posta olarak işaretle > NDR geri > "On" olarak ayarlayın**</span><span class="sxs-lookup"><span data-stu-id="14b7f-109">**protection.office.com > Threat Management > Policy > Antispam > Select the Spam Filter Policy and Edit policy > Spam properties > Mark as spam > NDR backscatter > Set it to “On”**</span></span>

<span data-ttu-id="14b7f-110">Bir hesabın güvenliği ihlal edilmiş olduğuna inanıyorsanız, aşağıdakilere bakın:</span><span class="sxs-lookup"><span data-stu-id="14b7f-110">If you believe an account has been compromised, see the following:</span></span>

- [<span data-ttu-id="14b7f-111">Güvenliği Tehlikeye E-posta Hesabını Yanıtla</span><span class="sxs-lookup"><span data-stu-id="14b7f-111">Responding to a Compromised Email Account</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account)
- [<span data-ttu-id="14b7f-112">Office 365'te Kısıtlanmış Kullanıcılar portaldan engellenen kullanıcıları kaldırma</span><span class="sxs-lookup"><span data-stu-id="14b7f-112">Removing blocked users from the Restricted Users portal in Office 365</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/removing-user-from-restricted-users-portal-after-spam)



