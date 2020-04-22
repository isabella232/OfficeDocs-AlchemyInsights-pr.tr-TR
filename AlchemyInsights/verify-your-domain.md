---
title: Verify your domain
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
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
ms.openlocfilehash: 2c4d8e075d2cf7214b5ef005b856daf7fb0ed53c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43710463"
---
# <a name="verify-your-domain"></a><span data-ttu-id="6adf1-102">Verify your domain</span><span class="sxs-lookup"><span data-stu-id="6adf1-102">Verify your domain</span></span>

 <span data-ttu-id="6adf1-103">**Kayıt büyük olasılıkla Internet'te güncellenmedi.**</span><span class="sxs-lookup"><span data-stu-id="6adf1-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="6adf1-104">Yeni kaydı görmemiz genellikle yalnızca birkaç dakika sürer, ancak bazı durumlarda bu işlem birkaç saate kadar sürebilir.</span><span class="sxs-lookup"><span data-stu-id="6adf1-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="6adf1-105">Bu kadar beklediyseniz, tam değeri kopyalayıp DNS ana bilgisayarınızdaki TXT doğrulama kaydına yapıştırdığınızı iki kez kontrol edin.</span><span class="sxs-lookup"><span data-stu-id="6adf1-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="6adf1-106">Yaygın sorunlardan biri de kaydın "MS=" kısmının dahil edilmemesidir.</span><span class="sxs-lookup"><span data-stu-id="6adf1-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="6adf1-107">Bu kısmı da belirtmeniz gerekir!</span><span class="sxs-lookup"><span data-stu-id="6adf1-107">We need that too!</span></span>

- <span data-ttu-id="6adf1-108">Bazı DNS barındırıcılarında, İnternet'te güncelleştirilebilmesi için bölge dosyasını kaydetmek (DNS kaydının bulunduğu konuma) üzere ek bir adım uygulamanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="6adf1-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="6adf1-109">Microsoft'un kaydı görebilmesini ve doğrulayabilmesini sağlamak için değişikliklerinizi kaydettiğinizden emin olun.</span><span class="sxs-lookup"><span data-stu-id="6adf1-109">Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>
