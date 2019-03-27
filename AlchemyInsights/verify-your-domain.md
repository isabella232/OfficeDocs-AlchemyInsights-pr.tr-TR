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
ms.custom: ''
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: d215f3af0cf4b46b12c8cb51a9572adb00f354e4
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/22/2019
ms.locfileid: "30766368"
---
# <a name="verify-your-domain"></a><span data-ttu-id="a3852-102">Verify your domain</span><span class="sxs-lookup"><span data-stu-id="a3852-102">Verify your domain</span></span>

 <span data-ttu-id="a3852-103">**Büyük olasılıkla kayıt Internet üzerinden güncelleştirilmiş taşınmadığından.**</span><span class="sxs-lookup"><span data-stu-id="a3852-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="a3852-104">Yeni kaydı görmemiz genellikle yalnızca birkaç dakika sürer, ancak bazı durumlarda bu işlem birkaç saate kadar sürebilir.</span><span class="sxs-lookup"><span data-stu-id="a3852-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="a3852-105">Size, zaten uzun süre bekledi, siz kopyalanır ve tam değer, DNS ana bilgisayar doğrulama TXT kaydı yapıştırılan olduğunu denetleyin.</span><span class="sxs-lookup"><span data-stu-id="a3852-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="a3852-106">Yaygın sorunlardan biri de kaydın "MS=" kısmının dahil edilmemesidir.</span><span class="sxs-lookup"><span data-stu-id="a3852-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="a3852-107">Bu kısmı da belirtmeniz gerekir!</span><span class="sxs-lookup"><span data-stu-id="a3852-107">We need that too!</span></span>
    
- <span data-ttu-id="a3852-108">Bazı DNS barındırıcılarında, İnternet'te güncelleştirilebilmesi için bölge dosyasını kaydetmek (DNS kaydının bulunduğu konuma) üzere ek bir adım uygulamanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="a3852-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="a3852-109">Office 365'in kaydı görüp doğrulayabilmesi için değişikliklerinizi kaydetmeyi unutmayın.</span><span class="sxs-lookup"><span data-stu-id="a3852-109">Make sure you've saved your changes so Office 365 can see and verify the record.</span></span>
    

