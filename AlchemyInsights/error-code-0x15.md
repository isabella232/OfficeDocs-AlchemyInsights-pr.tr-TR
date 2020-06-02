---
title: Hata Kodu 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Uzak Masaüstü Hizmetleri (RDS) dağıtımlarında Office 2013'ü etkinleştirirken bir hata alıyorsanız, kayıt defterini düzenleyerek ADAL'ı etkinleştirmeyi düşünün.
ms.openlocfilehash: 468d13e59602cf173ed2e17af44c66babfc28703
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506866"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="1fd8e-103">Uzak Masaüstü Hizmetlerinde Office 2013 etkinleştirme sırasında hata</span><span class="sxs-lookup"><span data-stu-id="1fd8e-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="1fd8e-104">Uzak Masaüstü Hizmetleri (RDS) dağıtımlarında Office 2013'ü etkinleştirirken bir hata alıyorsanız, kayıt defterini düzenleyerek ADAL'ı etkinleştirmeyi düşünün.</span><span class="sxs-lookup"><span data-stu-id="1fd8e-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="1fd8e-105">**Kayıt defteri anahtarı**</span><span class="sxs-lookup"><span data-stu-id="1fd8e-105">**Registry key**</span></span>|<span data-ttu-id="1fd8e-106">**Tür**</span><span class="sxs-lookup"><span data-stu-id="1fd8e-106">**Type**</span></span>|<span data-ttu-id="1fd8e-107">**Değer**</span><span class="sxs-lookup"><span data-stu-id="1fd8e-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="1fd8e-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Ortak\Kimlik\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="1fd8e-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="1fd8e-109">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="1fd8e-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="1fd8e-110">1</span><span class="sxs-lookup"><span data-stu-id="1fd8e-110">1</span></span>  <br/> |

<span data-ttu-id="1fd8e-111">Daha fazla bilgi için windows [aygıtlarında Office 2013 için Modern Kimlik Doğrulamasını Etkinleştir'e](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)bakın.</span><span class="sxs-lookup"><span data-stu-id="1fd8e-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="1fd8e-112">ADAL, kurumsal ve Office 2016 için Microsoft 365 Apps'ta varsayılan olarak etkinleştirilir.</span><span class="sxs-lookup"><span data-stu-id="1fd8e-112">ADAL is enabled by default in Microsoft 365 Apps for enterprise and Office 2016.</span></span> <span data-ttu-id="1fd8e-113">Uzak Masaüstü Hizmetleri (RDS) daha önce Terminal Hizmetleri olarak adlandırıldı.</span><span class="sxs-lookup"><span data-stu-id="1fd8e-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  