---
title: Tümünü yakala
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 262d2c6a7181d94094f3d840c4ba3ebd07000cf4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47713006"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="10892-102">Tümünü yakala</span><span class="sxs-lookup"><span data-stu-id="10892-102">Create an email catch all</span></span>

<span data-ttu-id="10892-103">Tümünü yakala 'nın kullanımı kesinlikle önerilmez.</span><span class="sxs-lookup"><span data-stu-id="10892-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="10892-104">Gönderene geri sıçrama sağlamak daha iyidir, gönderenlere ileti teslim edilebilmeleri için iletileri adreslenmiş olarak teslim edilemedi.</span><span class="sxs-lookup"><span data-stu-id="10892-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="10892-105">İzlenen posta kutusunu yalnızca önceden geçerli olan e-posta adresleriyle da sınırlayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="10892-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="10892-106">Tüm catch posta kutuları istenmeyen bir istenmeyen posta alır ve yakın zamanda izlenmediğini de doldurabilir.</span><span class="sxs-lookup"><span data-stu-id="10892-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="10892-107">(Alan sınırlamaları vardır.)</span><span class="sxs-lookup"><span data-stu-id="10892-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="10892-108">Devam etmeye karar verirseniz, şu adımları izleyin:</span><span class="sxs-lookup"><span data-stu-id="10892-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="10892-109">"Tüm alıcı türleri" & dinamik dağıtım grubu oluşturun.</span><span class="sxs-lookup"><span data-stu-id="10892-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="10892-110">E-postaları yakalamak için adanmış bir posta kutusu oluşturun (örneğin, catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="10892-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="10892-111">İlgili etki alanı için, DomainType 'ı "ınternalrelay" olarak ayarlayın.</span><span class="sxs-lookup"><span data-stu-id="10892-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="10892-112">Daha sonra tümünü kaldırırsanız, etki alanını yetkili olarak ayarladığınızdan emin olun.</span><span class="sxs-lookup"><span data-stu-id="10892-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="10892-113">Şu şekilde bir mailflow aktarım kuralı oluşturun:</span><span class="sxs-lookup"><span data-stu-id="10892-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="10892-114">Gönderen "kuruluşun dışına" ise</span><span class="sxs-lookup"><span data-stu-id="10892-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="10892-115">İletiyi Catchall@domain.com 'e yönlendirme</span><span class="sxs-lookup"><span data-stu-id="10892-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="10892-116">Alıcının üyesi olması dışında (dağıtım grubu tüm üyeleri içerir)</span><span class="sxs-lookup"><span data-stu-id="10892-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="10892-117">Dinamik dağıtım grubuna yeni posta kutularının eklendiğini doğrulama</span><span class="sxs-lookup"><span data-stu-id="10892-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
