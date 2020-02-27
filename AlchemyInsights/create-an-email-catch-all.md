---
title: Tümeği yakalama e-posta sıyrık oluşturma
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 35f31c1662547d57c2fc9978ffb495ac29abcc01
ms.sourcegitcommit: 67015549afcbe05f3b77ea314e2ef7e0e439f9f2
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 02/26/2020
ms.locfileid: "42286311"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="a838b-102">Tümeği yakalama e-posta sıyrık oluşturma</span><span class="sxs-lookup"><span data-stu-id="a838b-102">Create an email catch all</span></span>

<span data-ttu-id="a838b-103">Bir yakalama tüm kullanımı şiddetle önerilmez.</span><span class="sxs-lookup"><span data-stu-id="a838b-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="a838b-104">Gönderene, gönderenlere, iletilerinin adreslendirilen şekilde teslim edilemediğini bildirilmesi ne kadar önemli yse, bu nedenle işlem yapabilmeleri için geri sıçrama sağlamak daha iyidir.</span><span class="sxs-lookup"><span data-stu-id="a838b-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="a838b-105">Ayrıca, izlenen posta kutusunu yalnızca daha önce geçerli olan e-posta adreslerini yakalamak için sınırlayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="a838b-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="a838b-106">Herhangi bir yakalamak tüm posta kutusu spam iyi bir anlaşma alırsınız ve sonunda yakından izlenmezeğer doldurabilir.</span><span class="sxs-lookup"><span data-stu-id="a838b-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="a838b-107">(Alma sınırları vardır.)</span><span class="sxs-lookup"><span data-stu-id="a838b-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="a838b-108">Devam etmeye karar verirseniz, aşağıdaki adımları izleyin:</span><span class="sxs-lookup"><span data-stu-id="a838b-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="a838b-109">Dinamik Dağıtım Grubu oluşturma & "Tüm Alıcı Türleri" içerir.</span><span class="sxs-lookup"><span data-stu-id="a838b-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="a838b-110">Örneğin, catchall@domain.com e-postaları yakalamak için özel bir Posta Kutusu oluşturun.</span><span class="sxs-lookup"><span data-stu-id="a838b-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="a838b-111">Belirli etki alanı için DomainType'ı "InternalRelay" olarak ayarlayın.</span><span class="sxs-lookup"><span data-stu-id="a838b-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="a838b-112">Daha sonra tüm yakalamayı kaldırırsanız, etki alanını Yetkili'ye geri ayarladığınızdan emin olun.</span><span class="sxs-lookup"><span data-stu-id="a838b-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="a838b-113">Posta Akışı Aktarım Kuralı'nı aşağıdaki gibi oluşturun:</span><span class="sxs-lookup"><span data-stu-id="a838b-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="a838b-114">Gönderen "Kuruluş Dışında" ise</span><span class="sxs-lookup"><span data-stu-id="a838b-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="a838b-115">İletiyi Catchall@domain.com'a yönlendirme</span><span class="sxs-lookup"><span data-stu-id="a838b-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="a838b-116">Alıcı allusers@domain.com üyesi yse (Dağıtım Grubu tüm üyeleri içerir)</span><span class="sxs-lookup"><span data-stu-id="a838b-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="a838b-117">Dinamik Dağıtım Grubuna yeni posta kutularının eklenmesini doğrulamayı sağlamak</span><span class="sxs-lookup"><span data-stu-id="a838b-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
