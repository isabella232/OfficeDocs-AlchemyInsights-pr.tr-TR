---
title: Karma ortam için ileti şifrelemeyi yapılandırma
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 22c2468b7639680b447b6464431a79b69f7198c3
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747945"
---
# <a name="configure-message-encryption-for-a-hybrid-environment"></a><span data-ttu-id="b5595-102">Karma ortam için ileti şifrelemeyi yapılandırma</span><span class="sxs-lookup"><span data-stu-id="b5595-102">Configure message encryption for a hybrid environment</span></span>

<span data-ttu-id="b5595-103">Karma Exchange ortamları için, şirket içi kullanıcılar office İleti Şifrelemesi (OME) kullanarak şifrelenmiş e-posta gönderemelerini, ancak e-posta Exchange Online üzerinden yönlendirildiklerini gösterir.</span><span class="sxs-lookup"><span data-stu-id="b5595-103">For hybrid Exchange environments, on-premises users can send encrypted email using Office Message Encryption (OME) only if email is routed through Exchange Online.</span></span>

<span data-ttu-id="b5595-104">OME kullanarak e-postaları şifrelemek için aşağıdaki adımları uygulayın:</span><span class="sxs-lookup"><span data-stu-id="b5595-104">To encrypt emails using OME, perform the following steps:</span></span>

1. <span data-ttu-id="b5595-105">Karma [ortamınızı ayarlamak için](https://docs.microsoft.com/Exchange/hybrid-configuration-wizard) Karma Yapılandırma sihirbazını kullanın.</span><span class="sxs-lookup"><span data-stu-id="b5595-105">Use the [Hybrid Configuration wizard](https://docs.microsoft.com/Exchange/hybrid-configuration-wizard) to set up your hybrid environment.</span></span> <span data-ttu-id="b5595-106">Şifrelemeyi ayarlamaya özel adımlar gerekmez.</span><span class="sxs-lookup"><span data-stu-id="b5595-106">No special steps are required for setting up encryption.</span></span>
2. <span data-ttu-id="b5595-107">[Posta akış kurallarınızı her zaman olduğu gibi](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email) şifreleme için ayarlayın.</span><span class="sxs-lookup"><span data-stu-id="b5595-107">[Set up your mail flow rules for encryption](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email) like you normally would.</span></span>


