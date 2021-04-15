---
title: Verify your domain
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "47"
- "48"
- "8"
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: 4a34de7fa2aaaae365cf4562d31590d4b5fb7544
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51771011"
---
# <a name="verify-your-domain"></a><span data-ttu-id="9ae2e-102">Verify your domain</span><span class="sxs-lookup"><span data-stu-id="9ae2e-102">Verify your domain</span></span>

 <span data-ttu-id="9ae2e-103">**Kayıt büyük olasılıkla İnternet genelinde güncelleştirilmedi.**</span><span class="sxs-lookup"><span data-stu-id="9ae2e-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="9ae2e-104">Yeni kaydı görmemiz genellikle yalnızca birkaç dakika sürer, ancak bazı durumlarda bu işlem birkaç saate kadar sürebilir.</span><span class="sxs-lookup"><span data-stu-id="9ae2e-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="9ae2e-105">Zaten bu kadar uzun bir süre beklediysanız, DNS ana ekleyebilirsiniz ve değeri TXT doğrulama kaydına aynı şekilde kopyap yapıştırmış o kadar çok şey olduğunu bir kez daha kontrol edin.</span><span class="sxs-lookup"><span data-stu-id="9ae2e-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="9ae2e-106">Yaygın sorunlardan biri de kaydın "MS=" kısmının dahil edilmemesidir.</span><span class="sxs-lookup"><span data-stu-id="9ae2e-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="9ae2e-107">Bu kısmı da belirtmeniz gerekir!</span><span class="sxs-lookup"><span data-stu-id="9ae2e-107">We need that too!</span></span>

- <span data-ttu-id="9ae2e-108">Bazı DNS barındırıcılarında, İnternet'te güncelleştirilebilmesi için bölge dosyasını kaydetmek (DNS kaydının bulunduğu konuma) üzere ek bir adım uygulamanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="9ae2e-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="9ae2e-109">Microsoft'un kaydı görmesi ve doğrulaysı için değişikliklerinizi kaydetmeyi sağlar.</span><span class="sxs-lookup"><span data-stu-id="9ae2e-109">Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>
