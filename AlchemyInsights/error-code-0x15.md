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
ms.openlocfilehash: e2249d8ebbd2313c64dda5656a3243fa76d97a9a
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/28/2019
ms.locfileid: "35388265"
---
<span data-ttu-id="65a93-103">Uzak Masaüstü Hizmetleri (RDS) dağıtımları üzerinde Office 2013 etkinleştirilirken bir hata almak, kayıt defterini düzenleyerek ADAL etkinleştirme düşünün.</span><span class="sxs-lookup"><span data-stu-id="65a93-103">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="65a93-104">**Kayıt defteri anahtarı**</span><span class="sxs-lookup"><span data-stu-id="65a93-104">**Registry key**</span></span>|<span data-ttu-id="65a93-105">**Tür**</span><span class="sxs-lookup"><span data-stu-id="65a93-105">**Type**</span></span>|<span data-ttu-id="65a93-106">**Değer**</span><span class="sxs-lookup"><span data-stu-id="65a93-106">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="65a93-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="65a93-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="65a93-108">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="65a93-108">REG_DWORD</span></span>  <br/> |<span data-ttu-id="65a93-109">1</span><span class="sxs-lookup"><span data-stu-id="65a93-109">1</span></span>  <br/> |

<span data-ttu-id="65a93-110">Daha fazla bilgi için bkz: [Etkinleştirmek Modern kimlik doğrulaması Windows cihazlarda Office 2013](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="65a93-110">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="65a93-111">ADAL Office 365 ProPlus ve Office 2016 varsayılan olarak etkindir.</span><span class="sxs-lookup"><span data-stu-id="65a93-111">ADAL is enabled by default in Office 365 ProPlus and Office 2016.</span></span> <span data-ttu-id="65a93-112">> Uzak Masaüstü Hizmetleri (RDS), önceden Terminal Hizmetleri olarak biliniyordu.</span><span class="sxs-lookup"><span data-stu-id="65a93-112">>  Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  