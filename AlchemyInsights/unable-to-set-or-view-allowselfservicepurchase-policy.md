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
ms.openlocfilehash: a9b6e36e8034e71b3e72c49e3cc68a126ef97aca
ms.sourcegitcommit: cb9505f9eca032af3a4194c68d18c91789365690
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 02/16/2020
ms.locfileid: "42091782"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="c8e92-102">AllowSelfServicePurchase ilkesini ayarlayamıyor veya görüntüleyemiyor</span><span class="sxs-lookup"><span data-stu-id="c8e92-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="c8e92-103">AllowSelfServicePurchase ilkesini ayarlamaya veya görüntülemeye çalışırken aşağıdaki hata iletisini alırsınız:</span><span class="sxs-lookup"><span data-stu-id="c8e92-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="c8e92-104">*HandleError : PolicyId 'AllowSelfServicePurchase' ile ürün ilkesi alınamadı, ErrorMessage - Altta yatan bağlantı kapatıldı: Gönderimde beklenmeyen bir hata oluştu.*</span><span class="sxs-lookup"><span data-stu-id="c8e92-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="c8e92-105">Bunun nedeni, Aktarım Katmanı Güvenliği'nin (TLS) eski bir sürümü olabilir.</span><span class="sxs-lookup"><span data-stu-id="c8e92-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="c8e92-106">MSCommerce hizmetini bağlamak için TLS 1.2 veya daha büyük bir şekilde kullanmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="c8e92-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="c8e92-107">TLS protokolünü etkinleştirmek/1,2 olarak ayarlamak, doğrulamak ve yeniden denemek için aşağıdaki adımları deneyin.</span><span class="sxs-lookup"><span data-stu-id="c8e92-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="c8e92-108">PowerShell komut isteminde (PS\) C: TLS protokolünü sürüm 1.2'ye ayarlamak için aşağıdaki komutu girin:</span><span class="sxs-lookup"><span data-stu-id="c8e92-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    <span data-ttu-id="c8e92-109">\[Net.ServicePointManager]::SecurityProtocol = \[Net.SecurityProtocolType]::Tls12</span><span class="sxs-lookup"><span data-stu-id="c8e92-109">\[Net.ServicePointManager]::SecurityProtocol = \[Net.SecurityProtocolType]::Tls12</span></span>

2. <span data-ttu-id="c8e92-110">Kullanımdaki TLS protokolünü aşağıdaki komutla doğrulayın:</span><span class="sxs-lookup"><span data-stu-id="c8e92-110">Verify the TLS protocol(s) in use, with the following command:</span></span>

    <span data-ttu-id="c8e92-111">\[Net.ServicePointManager]::SecurityProtocol</span><span class="sxs-lookup"><span data-stu-id="c8e92-111">\[Net.ServicePointManager]::SecurityProtocol</span></span> 

3. <span data-ttu-id="c8e92-112">Gerektiğinde Get or Update komutlarını yeniden deneyin.</span><span class="sxs-lookup"><span data-stu-id="c8e92-112">Retry the Get or Update commands as needed.</span></span>

