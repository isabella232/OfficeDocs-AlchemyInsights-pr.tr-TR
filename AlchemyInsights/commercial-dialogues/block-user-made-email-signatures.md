---
title: Kullanıcı tarafından yapılan e-posta imzalarını engelleme
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200009"
- "7310"
ms.openlocfilehash: dab7eacb617c8f3a8bd63634e974166b6e448d75
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50483362"
---
# <a name="block-user-made-email-signatures"></a><span data-ttu-id="26355-102">Kullanıcı tarafından yapılan e-posta imzalarını engelleme</span><span class="sxs-lookup"><span data-stu-id="26355-102">Block user-made email signatures</span></span>

<span data-ttu-id="26355-103">Aşağıdaki çözüm yalnızca Web üzerinde Outlook'ta oluşturulmuş e-posta imzaları için geçerlidir.</span><span class="sxs-lookup"><span data-stu-id="26355-103">The following solution only applies to email signatures created in Outlook on the web.</span></span> <span data-ttu-id="26355-104">Outlook uygulamasındaki imzaları yalnızca şirket içi Exchange Server'nız varsa engelleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="26355-104">You can only block signatures in the Outlook app if you have an on-premises Exchange Server.</span></span>

1. <span data-ttu-id="26355-105">Yönetim merkezinde Exchange Yönetim **merkezleri'ni**  >  **seçin.**</span><span class="sxs-lookup"><span data-stu-id="26355-105">In the admin center, choose **Admin centers** > **Exchange**.</span></span>
2. <span data-ttu-id="26355-106">İzinler   >  **Outlook Web App ilkelerine tıklayın.**</span><span class="sxs-lookup"><span data-stu-id="26355-106">Click **permissions** > **Outlook Web App policies**.</span></span>
3. <span data-ttu-id="26355-107">İlkeyi seçin ve düzenlemek için kalem simgesine tıklayın.</span><span class="sxs-lookup"><span data-stu-id="26355-107">Select the policy, and then click the pencil icon to edit it.</span></span>
4. <span data-ttu-id="26355-108">Diğer   >  **seçenekler'e tıklayın.**</span><span class="sxs-lookup"><span data-stu-id="26355-108">Click **features** > **More options**.</span></span>
5. <span data-ttu-id="26355-109">Kullanıcı **deneyimi altında,** E-posta **imzası onay** kutusunu temizleyin ve Kaydet'e **tıklayın.**</span><span class="sxs-lookup"><span data-stu-id="26355-109">Under **User experience**, clear the **Email signature** check box, and then click **Save**.</span></span>

<span data-ttu-id="26355-110">**Önemli:** Bu onay kutusunu temizlemeden önce bir imza eklenmişse, kullanıcı bu imzayı kullanmaya devam ediyor olabilir.</span><span class="sxs-lookup"><span data-stu-id="26355-110">**Important:** If a signature was added before clearing this check box, the user will still be able to use it.</span></span> <span data-ttu-id="26355-111">Kaldırmalarını iste.</span><span class="sxs-lookup"><span data-stu-id="26355-111">Ask them to remove it.</span></span>
