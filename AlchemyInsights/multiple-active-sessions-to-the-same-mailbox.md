---
title: Aynı posta kutusuna birden çok etkin oturum
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1836"
- "9000248"
ms.openlocfilehash: d2fd3f20346012baed21efd4900ca4cf73391d91
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439724"
---
# <a name="multiple-active-sessions-to-the-same-mailbox"></a><span data-ttu-id="01828-102">Aynı posta kutusuna birden çok etkin oturum</span><span class="sxs-lookup"><span data-stu-id="01828-102">Multiple active sessions to the same mailbox</span></span>

<span data-ttu-id="01828-103">Exchange kaynaklarının kullanımını denetlemek için posta kutusunun bir "bütçesi" vardır.</span><span class="sxs-lookup"><span data-stu-id="01828-103">To control usage of Exchange resources, a mailbox has a "budget."</span></span>

<span data-ttu-id="01828-104">Bütçe nin üzerindeki özel durum aşağıdaki koşullar tarafından tetiklenebilir, ancak bununla sınırlı değildir:</span><span class="sxs-lookup"><span data-stu-id="01828-104">The over-budget exception can be triggered by, but is not limited to, the following circumstances:</span></span>

- <span data-ttu-id="01828-105">Aynı Outlook Web Uygulaması oturumu içinde birkaç tarayıcı sekmesi açılır.</span><span class="sxs-lookup"><span data-stu-id="01828-105">A few browser tabs are opened within the same Outlook Web App session.</span></span>

- <span data-ttu-id="01828-106">Aynı posta kutusuna birkaç etkin Outlook Web Uygulaması oturumu.</span><span class="sxs-lookup"><span data-stu-id="01828-106">A few active Outlook Web App sessions to the same mailbox.</span></span>

- <span data-ttu-id="01828-107">Birkaç diğer istemci uygulaması (Outlook, Outlook Mobile, üçüncü taraf istemci uygulaması) posta kutusuna aynı anda erişir.</span><span class="sxs-lookup"><span data-stu-id="01828-107">A few other client applications (Outlook, Outlook Mobile, a third party client app) access the mailbox at the same time.</span></span>

- <span data-ttu-id="01828-108">Arama isteklerini yürütme gibi uzun süren işlemler başka bir etkin posta kutusu oturumundagerçekleştirilir.</span><span class="sxs-lookup"><span data-stu-id="01828-108">Long running operations, such as executing search requests, are performed from another active mailbox session.</span></span>

