---
title: AllowSelfServicePurchase ilkesi ayarlanamıyor veya görüntüden silinemiyor
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 8dac2bdc20905cf37fc30317d9b371bfd755f452
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826111"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="c9d3d-102">AllowSelfServicePurchase ilkesi ayarlanamıyor veya görüntüden silinemiyor</span><span class="sxs-lookup"><span data-stu-id="c9d3d-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="c9d3d-103">AllowSelfServicePurchase ilkesi ayarlamaya veya görüntülemeye çalışırken, aşağıdaki hata iletisini alısınız:</span><span class="sxs-lookup"><span data-stu-id="c9d3d-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="c9d3d-104">*HandleError: PolicyId 'AllowSelfServicePurchase', ErrorMessage ile ürün ilkesi alınamadı - Temel bağlantı kapatıldı: Gönderme sırasında beklenmeyen bir hata oluştu.*</span><span class="sxs-lookup"><span data-stu-id="c9d3d-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="c9d3d-105">Bunun nedeni Aktarım Katmanı Güvenliği'nin (TLS) eski bir sürümü olabilir.</span><span class="sxs-lookup"><span data-stu-id="c9d3d-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="c9d3d-106">MSCommerce hizmetine bağlanmak için TLS 1.2 veya daha yeni bir değer kullan gerekir.</span><span class="sxs-lookup"><span data-stu-id="c9d3d-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="c9d3d-107">TLS protokolünü 1,2 olarak etkinleştirmek/ayarlamak, doğrulamak ve yeniden denemek için aşağıdaki adımları deneyin.</span><span class="sxs-lookup"><span data-stu-id="c9d3d-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="c9d3d-108">PowerShell komut isteminde (PS C: TLS protokolünü sürüm 1.2 olarak ayarlamak için \) aşağıdaki komutu girin:</span><span class="sxs-lookup"><span data-stu-id="c9d3d-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="c9d3d-109">Kullanımda OLAN TLS protokollerini şu komutu kullanarak doğrulayın:</span><span class="sxs-lookup"><span data-stu-id="c9d3d-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="c9d3d-110">Al veya Güncelleştir komutlarını gerektiğinde yeniden deneyin.</span><span class="sxs-lookup"><span data-stu-id="c9d3d-110">Retry the Get or Update commands as needed.</span></span>

