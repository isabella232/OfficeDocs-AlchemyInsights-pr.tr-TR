---
title: Hata kodu 550 5.7.501 Erişim reddedildi, spam kötüye kullanımı algılandı
ms.author: chrisda
author: chrisda
ms.date: 6/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "351"
- "3100015"
ms.assetid: 3105905c-e7a0-42a7-9c5a-61dc56a1d6fc
ms.openlocfilehash: 545cab07cc7c49def849be20bb6363da228a5393
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/25/2019
ms.locfileid: "36740161"
---
# <a name="550-57501-access-denied-spam-abuse-detected"></a><span data-ttu-id="3c59e-102">550 5.7.501 Erişim reddedildi, spam kötüye kullanımı algılandı</span><span class="sxs-lookup"><span data-stu-id="3c59e-102">550 5.7.501 Access denied, spam abuse detected</span></span>

<span data-ttu-id="3c59e-103">Genellikle, bu ileti, kullanıcılar Office 365'teki yeni kiracılara atanan ilk *.onmicrosoft.com* etki alanını kullanarak IP adreslerinden e-posta iletileri gönderdiğinde oluşur.</span><span class="sxs-lookup"><span data-stu-id="3c59e-103">Typically, this message occurs when users send email messages from IP addresses using the initial *.onmicrosoft.com* domain that's assigned to new tenants in Office 365.</span></span> <span data-ttu-id="3c59e-104">Bu sorunu çözmenin en kolay yolu:</span><span class="sxs-lookup"><span data-stu-id="3c59e-104">The easiest way to resolve this problem is to:</span></span>

1. <span data-ttu-id="3c59e-105">[Kiracınıza bir etki alanı ekleyin.](https://docs.microsoft.com//office365/admin/setup/add-domain)</span><span class="sxs-lookup"><span data-stu-id="3c59e-105">[Add a domain to your tenant](https://docs.microsoft.com//office365/admin/setup/add-domain).</span></span>

2. <span data-ttu-id="3c59e-106">[Kullanıcılarınızın birincil e-posta adresini](https://docs.microsoft.com//office365/admin/add-users/change-a-user-name-and-email-address) yeni eklediğiniz yeni özel etki alanıyla değiştirin.</span><span class="sxs-lookup"><span data-stu-id="3c59e-106">[Change your users' primary email address](https://docs.microsoft.com//office365/admin/add-users/change-a-user-name-and-email-address) to the new custom domain you just added.</span></span>
