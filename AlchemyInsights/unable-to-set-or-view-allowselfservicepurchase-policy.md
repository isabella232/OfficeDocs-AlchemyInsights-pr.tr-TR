---
title: AllowSelfServicePurchase ilkesini ayarlayamıyor veya görüntüleyemiyor
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 587a05cccbc71a970d4bd7723bff0df0c3b64ccc
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158581"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="ddfe2-102">AllowSelfServicePurchase ilkesini ayarlayamıyor veya görüntüleyemiyor</span><span class="sxs-lookup"><span data-stu-id="ddfe2-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="ddfe2-103">AllowSelfServicePurchase ilkesini ayarlamaya veya görüntülemeye çalışırken aşağıdaki hata iletisini alırsınız:</span><span class="sxs-lookup"><span data-stu-id="ddfe2-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="ddfe2-104">*HandleError : PolicyId 'AllowSelfServicePurchase' ile ürün ilkesi alınamadı, ErrorMessage - Altta yatan bağlantı kapatıldı: Gönderimde beklenmeyen bir hata oluştu.*</span><span class="sxs-lookup"><span data-stu-id="ddfe2-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="ddfe2-105">Bunun nedeni, Aktarım Katmanı Güvenliği'nin (TLS) eski bir sürümü olabilir.</span><span class="sxs-lookup"><span data-stu-id="ddfe2-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="ddfe2-106">MSCommerce hizmetini bağlamak için TLS 1.2 veya daha büyük bir şekilde kullanmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="ddfe2-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="ddfe2-107">TLS protokolünü etkinleştirmek/1,2 olarak ayarlamak, doğrulamak ve yeniden denemek için aşağıdaki adımları deneyin.</span><span class="sxs-lookup"><span data-stu-id="ddfe2-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="ddfe2-108">PowerShell komut isteminde (PS\) C: TLS protokolünü sürüm 1.2'ye ayarlamak için aşağıdaki komutu girin:</span><span class="sxs-lookup"><span data-stu-id="ddfe2-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="ddfe2-109">Kullanımdaki TLS protokolünü aşağıdaki komutla doğrulayın:</span><span class="sxs-lookup"><span data-stu-id="ddfe2-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="ddfe2-110">Gerektiğinde Get or Update komutlarını yeniden deneyin.</span><span class="sxs-lookup"><span data-stu-id="ddfe2-110">Retry the Get or Update commands as needed.</span></span>

