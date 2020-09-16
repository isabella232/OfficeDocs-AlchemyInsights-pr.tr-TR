---
title: AllowSelfServicePurchase ilkesi ayarlanamıyor veya gösterilemiyor
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 5ec16b3071f95ef52af2771e95137116222a3c5b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47735219"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="dedd6-102">AllowSelfServicePurchase ilkesi ayarlanamıyor veya gösterilemiyor</span><span class="sxs-lookup"><span data-stu-id="dedd6-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="dedd6-103">AllowSelfServicePurchase ilkesini ayarlamaya veya görüntülemeye çalışırken aşağıdaki hata iletisini alırsınız:</span><span class="sxs-lookup"><span data-stu-id="dedd6-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="dedd6-104">*HandleError: PolicyId ' AllowSelfServicePurchase ' ile ürün ilkesi alınamadı, ErrorMessage-temeldeki bağlantı kapatıldı: gönderme sırasında beklenmeyen bir hata oluştu.*</span><span class="sxs-lookup"><span data-stu-id="dedd6-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="dedd6-105">Bu, taşıma katmanı güvenliğinin (TLS) eski bir sürümü olabilir.</span><span class="sxs-lookup"><span data-stu-id="dedd6-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="dedd6-106">MSCommerce hizmetini bağlamak için, TLS 1,2 veya üzerini kullanmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="dedd6-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="dedd6-107">TLS protokolünü 1,2, doğrulama ve yeniden deneyin.</span><span class="sxs-lookup"><span data-stu-id="dedd6-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="dedd6-108">PowerShell komut isteminde (PS C: \) TLS protokolünü sürüm 1,2 olarak ayarlamak için aşağıdaki komutu girin:</span><span class="sxs-lookup"><span data-stu-id="dedd6-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="dedd6-109">Aşağıdaki komutla, kullanımdaki TLS protokollerini doğrulayın:</span><span class="sxs-lookup"><span data-stu-id="dedd6-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="dedd6-110">Gerektiğinde Al veya Güncelleştir komutlarını yeniden deneyin.</span><span class="sxs-lookup"><span data-stu-id="dedd6-110">Retry the Get or Update commands as needed.</span></span>

