---
title: 1554 Winsock hata 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 4f8007bd8ccb4666260c75fdca15dd0b14eb4e96
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698882"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="959ca-102">Winsock hatası 10061</span><span class="sxs-lookup"><span data-stu-id="959ca-102">Winsock error 10061</span></span>

<span data-ttu-id="959ca-103">Bu hata kodu, Microsoft 'un hedef ana bilgisayarla TCP yuvası (bağlantı) kurmadığı anlamına gelir.</span><span class="sxs-lookup"><span data-stu-id="959ca-103">This error code means that Microsoft couldn't establish a TCP socket (connection) with the target host.</span></span> <span data-ttu-id="959ca-104">Bu hatanın en olası nedeni, güvenlik duvarı yapılandırmanızla ilgili bir sorundur.</span><span class="sxs-lookup"><span data-stu-id="959ca-104">The most likely cause of this error is a problem with your firewall configuration.</span></span> <span data-ttu-id="959ca-105">Sorunu çözmek için şu ayarları işaretleyin:</span><span class="sxs-lookup"><span data-stu-id="959ca-105">To fix the problem, check these settings:</span></span>

- <span data-ttu-id="959ca-106">Güvenlik duvarı yapılandırmanızı [Microsoft 365 URL 'lerinde ve IP adresi aralıklarıyla](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges) doğrulama</span><span class="sxs-lookup"><span data-stu-id="959ca-106">Verify your firewall configuration with the information in [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>

- <span data-ttu-id="959ca-107">Hata, Exchange Online Protection (EOP) için gerekliyse, daha önce [Exchange Online PROTECTION IP adreslerinde](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)bir değişiklik yapmanız istenir.</span><span class="sxs-lookup"><span data-stu-id="959ca-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

- <span data-ttu-id="959ca-108">Internet servis sağlayıcınızın (ISP) bağlantı noktasını engellemediğini doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="959ca-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>

- <span data-ttu-id="959ca-109">Bağlayıcılarınızın akıllı ana bilgisayar ve hedef sunucu ayarlarını doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="959ca-109">Verify the smart host and target server settings in your connectors.</span></span>

<span data-ttu-id="959ca-110">Microsoft 365, *gelen* bağlantıları bu şekilde engellemez.</span><span class="sxs-lookup"><span data-stu-id="959ca-110">Note that Microsoft 365 doesn't block *incoming* connections in this manner.</span></span>
