---
title: Verify your domain
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "47"
- "48"
- "8"
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: 5bd6c32a246db9dfcdb475368ade0441df4dc9c3
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/28/2019
ms.locfileid: "35365437"
---
# <a name="verify-your-domain"></a><span data-ttu-id="e3c82-102">Verify your domain</span><span class="sxs-lookup"><span data-stu-id="e3c82-102">Verify your domain</span></span>

 <span data-ttu-id="e3c82-103">**Büyük olasılıkla kayıt Internet üzerinden güncelleştirilmiş taşınmadığından.**</span><span class="sxs-lookup"><span data-stu-id="e3c82-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="e3c82-104">Yeni kaydı görmemiz genellikle yalnızca birkaç dakika sürer, ancak bazı durumlarda bu işlem birkaç saate kadar sürebilir.</span><span class="sxs-lookup"><span data-stu-id="e3c82-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="e3c82-105">Size, zaten uzun süre bekledi, siz kopyalanır ve tam değer, DNS ana bilgisayar doğrulama TXT kaydı yapıştırılan olduğunu denetleyin.</span><span class="sxs-lookup"><span data-stu-id="e3c82-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="e3c82-106">Yaygın sorunlardan biri de kaydın "MS=" kısmının dahil edilmemesidir.</span><span class="sxs-lookup"><span data-stu-id="e3c82-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="e3c82-107">Bu kısmı da belirtmeniz gerekir!</span><span class="sxs-lookup"><span data-stu-id="e3c82-107">We need that too!</span></span>

- <span data-ttu-id="e3c82-108">Bazı DNS barındırıcılarında, İnternet'te güncelleştirilebilmesi için bölge dosyasını kaydetmek (DNS kaydının bulunduğu konuma) üzere ek bir adım uygulamanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="e3c82-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="e3c82-109">Office 365'in kaydı görüp doğrulayabilmesi için değişikliklerinizi kaydetmeyi unutmayın.</span><span class="sxs-lookup"><span data-stu-id="e3c82-109">Make sure you've saved your changes so Office 365 can see and verify the record.</span></span>
