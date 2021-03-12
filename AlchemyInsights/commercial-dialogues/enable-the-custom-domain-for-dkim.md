---
title: DKIM için özel etki alanını etkinleştirme
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 1a21101602f47dcb5c9b607d7bbccfacec00f43a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749214"
---
# <a name="enable-the-custom-domain-for-dkim"></a><span data-ttu-id="5852e-102">DKIM için özel etki alanını etkinleştirme</span><span class="sxs-lookup"><span data-stu-id="5852e-102">Enable the custom domain for DKIM</span></span>

<span data-ttu-id="5852e-103">Özel etki alanlarınız için CNAME kayıtlarını oluşturdukta, etki alanını etkinleştirmeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="5852e-103">After you create the CNAME records for your custom domains, you need to enable the domain.</span></span>

<span data-ttu-id="5852e-104">Etki alanını etkinleştirmek için aşağıdaki adımları uygulayın:</span><span class="sxs-lookup"><span data-stu-id="5852e-104">To enable the domain, perform the following steps:</span></span>

1. <span data-ttu-id="5852e-105">Exchange yönetim [merkezine gidin.](https://outlook.office365.com/ecp/)</span><span class="sxs-lookup"><span data-stu-id="5852e-105">Navigate to the [Exchange admin center](https://outlook.office365.com/ecp/).</span></span>
2. <span data-ttu-id="5852e-106">Sol bölmede, koruma **ve dkim > seçin.**</span><span class="sxs-lookup"><span data-stu-id="5852e-106">In the left pane, select **protection > dkim**.</span></span>
3. <span data-ttu-id="5852e-107">Etki alanını seçin ve dkIM imzaları olan bu etki alanı için **İmzala altında** Etkinleştir'e **tıklayın.**</span><span class="sxs-lookup"><span data-stu-id="5852e-107">Select the domain, and then under **Sign messages for this domain with DKIM signatures**, click **Enable**.</span></span> <span data-ttu-id="5852e-108">Her etki alanı için bu adımı yineler.</span><span class="sxs-lookup"><span data-stu-id="5852e-108">Repeat this step for each domain.</span></span>

