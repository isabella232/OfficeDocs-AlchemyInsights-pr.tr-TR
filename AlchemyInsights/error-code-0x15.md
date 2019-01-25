---
title: Hata kodu 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Uzak Masaüstü Hizmetleri (RDS) dağıtımları üzerinde Office 2013 etkinleştirilirken bir hata almak, kayıt defterini düzenleyerek ADAL etkinleştirme düşünün.
ms.openlocfilehash: 89f9270169e13fd7706f7826c624ef8ae4d47b3f
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29499402"
---
<span data-ttu-id="f194c-103">Uzak Masaüstü Hizmetleri (RDS) dağıtımları üzerinde Office 2013 etkinleştirilirken bir hata almak, kayıt defterini düzenleyerek ADAL etkinleştirme düşünün.</span><span class="sxs-lookup"><span data-stu-id="f194c-103">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span> 
  
|<span data-ttu-id="f194c-104">**Kayıt defteri anahtarı**</span><span class="sxs-lookup"><span data-stu-id="f194c-104">**Registry key**</span></span>|<span data-ttu-id="f194c-105">**Tür**</span><span class="sxs-lookup"><span data-stu-id="f194c-105">**Type**</span></span>|<span data-ttu-id="f194c-106">**Değer**</span><span class="sxs-lookup"><span data-stu-id="f194c-106">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="f194c-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="f194c-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="f194c-108">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="f194c-108">REG_DWORD</span></span>  <br/> |<span data-ttu-id="f194c-109">1.</span><span class="sxs-lookup"><span data-stu-id="f194c-109">1</span></span>  <br/> |
   
<span data-ttu-id="f194c-110">Daha fazla bilgi için bkz: [Etkinleştirmek Modern kimlik doğrulaması Windows cihazlarda Office 2013](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="f194c-110">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="f194c-p101">ADAL Office 365 ProPlus ve Office 2016 varsayılan olarak etkindir. > Uzak Masaüstü Hizmetleri (RDS), önceden Terminal Hizmetleri olarak biliniyordu.</span><span class="sxs-lookup"><span data-stu-id="f194c-p101">ADAL is enabled by default in Office 365 ProPlus and Office 2016. >  Remote Desktop Services (RDS) was previously named Terminal Services.</span></span> 
  

