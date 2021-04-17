---
title: Tüm e-posta yakalamaları oluşturma
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 2b9131a620139a93ddb844fd49d8fa2ed68e52c2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816220"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="b1857-102">Tüm e-posta yakalamaları oluşturma</span><span class="sxs-lookup"><span data-stu-id="b1857-102">Create an email catch all</span></span>

<span data-ttu-id="b1857-103">Tüm avların kullanımı kesinlikle önerilmez.</span><span class="sxs-lookup"><span data-stu-id="b1857-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="b1857-104">Gönderenlere geri dönmeleri ve iletilerinin adres olarak teslim alınamamasına ve bu şekilde eyleme geçilemelerine izin vermeleri daha iyidir.</span><span class="sxs-lookup"><span data-stu-id="b1857-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="b1857-105">Ayrıca, izlenen posta kutusunu yalnızca eski geçerli e-posta adreslerini yakalamak için sınırlandırabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="b1857-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="b1857-106">Tüm posta kutularına gelen tüm yakalamalar çok iyi bir istenmeyen posta alır ve yakın bir şekilde izlenmeyen postaların sayısı zamanla dolabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="b1857-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="b1857-107">(Alıcı sınırları vardır.)</span><span class="sxs-lookup"><span data-stu-id="b1857-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="b1857-108">Devam etmeye karar verdiyseniz şu adımları izleyin:</span><span class="sxs-lookup"><span data-stu-id="b1857-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="b1857-109">"Tüm Alıcı Türleri" & bir Dinamik Dağıtım Grubu grubu oluşturun.</span><span class="sxs-lookup"><span data-stu-id="b1857-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="b1857-110">E-postaları yakalamak için (örneğin, posta kutunuzu) yakalamak için özel catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="b1857-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="b1857-111">Belirli bir etki alanı için DomainType'ı "InternalRelay" olarak ayarlayın.</span><span class="sxs-lookup"><span data-stu-id="b1857-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="b1857-112">Tüm yakalamaları daha sonra kaldırırsanız, etki alanını Yetkili olarak ayar mutlaka ayarlayın.</span><span class="sxs-lookup"><span data-stu-id="b1857-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="b1857-113">Posta Akışı Aktarım Kuralı şöyle oluşturun:</span><span class="sxs-lookup"><span data-stu-id="b1857-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="b1857-114">Gönderen "Kuruluş Dışında" ise</span><span class="sxs-lookup"><span data-stu-id="b1857-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="b1857-115">İletiyi Yeniden Yönlendir Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="b1857-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="b1857-116">Alıcının grup üyesi olduğu dışında (allusers@domain.com Grubu tüm üyeleri içerir)</span><span class="sxs-lookup"><span data-stu-id="b1857-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="b1857-117">Yeni posta kutularının Dinamik Dağıtım Grubuna ek doğrulamak için emin olun</span><span class="sxs-lookup"><span data-stu-id="b1857-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
