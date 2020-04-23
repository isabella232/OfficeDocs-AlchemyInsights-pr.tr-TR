---
title: 1554 Winsock hatası 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: e8f62d97efc937518ef766b45e1747e83b7f99c3
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766189"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="f32f5-102">Winsock hatası 10061</span><span class="sxs-lookup"><span data-stu-id="f32f5-102">Winsock error 10061</span></span>

<span data-ttu-id="f32f5-103">Bu hata kodu, Microsoft'un hedef ana bilgisayarla bir TCP soketi (bağlantı) kuramadığı anlamına gelir.</span><span class="sxs-lookup"><span data-stu-id="f32f5-103">This error code means that Microsoft couldn't establish a TCP socket (connection) with the target host.</span></span> <span data-ttu-id="f32f5-104">Bu hatanın en olası nedeni güvenlik duvarı yapılandırmanızla ilgili bir sorundur.</span><span class="sxs-lookup"><span data-stu-id="f32f5-104">The most likely cause of this error is a problem with your firewall configuration.</span></span> <span data-ttu-id="f32f5-105">Sorunu gidermek için şu ayarları denetleyin:</span><span class="sxs-lookup"><span data-stu-id="f32f5-105">To fix the problem, check these settings:</span></span>

- <span data-ttu-id="f32f5-106">Güvenlik duvarı yapılandırmanızı Microsoft [365 URL'leri ve IP adres aralıklarında](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges) bulunan bilgilerle doğrulayın</span><span class="sxs-lookup"><span data-stu-id="f32f5-106">Verify your firewall configuration with the information in [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>

- <span data-ttu-id="f32f5-107">Hata Exchange Online Protection 'a (EOP) özgüyse, daha önce Exchange [Online Protection IP adreslerinde](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)bir değişiklik için bilgilendirilmeniz gerekirdi.</span><span class="sxs-lookup"><span data-stu-id="f32f5-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

- <span data-ttu-id="f32f5-108">Internet Servis Sağlayıcınızın (ISS) bağlantı noktasını engellemediğini doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="f32f5-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>

- <span data-ttu-id="f32f5-109">Bağlayıcılarınızdaki akıllı ana bilgisayar ve hedef sunucu ayarlarını doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="f32f5-109">Verify the smart host and target server settings in your connectors.</span></span>

<span data-ttu-id="f32f5-110">Microsoft 365'in *gelen* bağlantıları bu şekilde engellemediğini unutmayın.</span><span class="sxs-lookup"><span data-stu-id="f32f5-110">Note that Microsoft 365 doesn't block *incoming* connections in this manner.</span></span>
