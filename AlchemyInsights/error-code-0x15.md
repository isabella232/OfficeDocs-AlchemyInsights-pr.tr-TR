---
title: Hata kodu 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Uzak Masaüstü Hizmetleri (RDS) dağıtımları üzerinde Office 2013 etkinleştirilirken bir hata almak, kayıt defterini düzenleyerek ADAL etkinleştirme düşünün.
ms.openlocfilehash: 4ef2943e5a529368fa2c614e4431cf180924fbb8
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36527087"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="4f3b3-103">Uzak Masaüstü Hizmetleri üzerine Office 2013 etkinleştirme hatası</span><span class="sxs-lookup"><span data-stu-id="4f3b3-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="4f3b3-104">Uzak Masaüstü Hizmetleri (RDS) dağıtımları üzerinde Office 2013 etkinleştirilirken bir hata almak, kayıt defterini düzenleyerek ADAL etkinleştirme düşünün.</span><span class="sxs-lookup"><span data-stu-id="4f3b3-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="4f3b3-105">**Kayıt defteri anahtarı**</span><span class="sxs-lookup"><span data-stu-id="4f3b3-105">**Registry key**</span></span>|<span data-ttu-id="4f3b3-106">**Tür**</span><span class="sxs-lookup"><span data-stu-id="4f3b3-106">**Type**</span></span>|<span data-ttu-id="4f3b3-107">**Değer**</span><span class="sxs-lookup"><span data-stu-id="4f3b3-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="4f3b3-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="4f3b3-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="4f3b3-109">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="4f3b3-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="4f3b3-110">1</span><span class="sxs-lookup"><span data-stu-id="4f3b3-110">1</span></span>  <br/> |

<span data-ttu-id="4f3b3-111">Daha fazla bilgi için bkz: [Etkinleştirmek Modern kimlik doğrulaması Windows cihazlarda Office 2013](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="4f3b3-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="4f3b3-112">ADAL Office 365 ProPlus ve Office 2016 varsayılan olarak etkindir.</span><span class="sxs-lookup"><span data-stu-id="4f3b3-112">ADAL is enabled by default in Office 365 ProPlus and Office 2016.</span></span> <span data-ttu-id="4f3b3-113">Uzak Masaüstü Hizmetleri (RDS), önceden Terminal Hizmetleri olarak biliniyordu.</span><span class="sxs-lookup"><span data-stu-id="4f3b3-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  