---
title: Hata kodu 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Uzak Masaüstü Hizmetleri (RDS) dağıtımlarında Office 2013 ' i etkinleştirirken hata alıyorsanız, kayıt defterini düzenleyerek ADAL 'i etkinleştirmeyi düşünebilirsiniz.
ms.openlocfilehash: deb2ac4b0fb6a7b2e0045ff1b0ba95ad6e5e4a3a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709207"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="dd68f-103">Uzak Masaüstü Hizmetleri 'nde Office 2013 etkinleştirme hatası</span><span class="sxs-lookup"><span data-stu-id="dd68f-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="dd68f-104">Uzak Masaüstü Hizmetleri (RDS) dağıtımlarında Office 2013 ' i etkinleştirirken hata alıyorsanız, kayıt defterini düzenleyerek ADAL 'i etkinleştirmeyi düşünebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="dd68f-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="dd68f-105">**Kayıt defteri anahtarı**</span><span class="sxs-lookup"><span data-stu-id="dd68f-105">**Registry key**</span></span>|<span data-ttu-id="dd68f-106">**Tür**</span><span class="sxs-lookup"><span data-stu-id="dd68f-106">**Type**</span></span>|<span data-ttu-id="dd68f-107">**Değer**</span><span class="sxs-lookup"><span data-stu-id="dd68f-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="dd68f-108">HKEY_CURRENT_USER \Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="dd68f-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="dd68f-109">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="dd68f-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="dd68f-110">2</span><span class="sxs-lookup"><span data-stu-id="dd68f-110">1</span></span>  <br/> |

<span data-ttu-id="dd68f-111">Daha fazla bilgi için [Windows cihazlarında Office 2013 Için modern kimlik doğrulamasını etkinleştirme](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)konusuna bakın.</span><span class="sxs-lookup"><span data-stu-id="dd68f-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="dd68f-112">ADAL, kurumsal ve Office 2016 için Microsoft 365 uygulamalarında varsayılan olarak etkinleştirilmiştir.</span><span class="sxs-lookup"><span data-stu-id="dd68f-112">ADAL is enabled by default in Microsoft 365 Apps for enterprise and Office 2016.</span></span> <span data-ttu-id="dd68f-113">Uzak Masaüstü Hizmetleri (RDS) daha önce Terminal Hizmetleri olarak adlandırıyordu.</span><span class="sxs-lookup"><span data-stu-id="dd68f-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  