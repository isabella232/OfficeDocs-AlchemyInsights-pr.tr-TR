---
title: Koşullu erişim ile Intune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 59f1aefaeec3d655b2388b00e7d58a8c2338504b
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29495010"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="6e478-102">Koşullu erişim ile Intune</span><span class="sxs-lookup"><span data-stu-id="6e478-102">Conditional Access with Intune</span></span>

<span data-ttu-id="6e478-103">**Koşullu erişim** kullanarak Intune ile 3 adımları gerektirir:</span><span class="sxs-lookup"><span data-stu-id="6e478-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="6e478-p101">Hangi kaynaklar korunur ve bu kaynaklara erişmek için karşılanması gereken koşulları gerekenleri tanımlayan bir **Koşullu erişim ilkesi** oluşturun. Örneğin, bir aygıtın şirket e-posta erişmeden önce uyumlu olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="6e478-p101">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources. For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="6e478-p102">Aygıt uyumlu olarak kabul edilmeden önce karşılanması gereken ayarları tanımlamak için bir **Uyumluluk İlkesi** oluşturun. Örneğin, bir aygıt uyumlu kabul edilmeden önce en az 6 basamaklı bir PIN olması gerekir.</span><span class="sxs-lookup"><span data-stu-id="6e478-p102">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant. For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="6e478-p103">**Uygunluk ilkeleri** hem de **Koşullu erişim ilkeleri** istenen kullanıcı grupları için hedeflenmiş sağlama. Bu, belirli kullanıcı gruplarına Azure Active Directory'de oluşturma gerektirebilir.</span><span class="sxs-lookup"><span data-stu-id="6e478-p103">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users. This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="6e478-110">Daha fazlasını okuyun</span><span class="sxs-lookup"><span data-stu-id="6e478-110">Read more:</span></span>
  
- [<span data-ttu-id="6e478-111">Koşullu erişim en iyi yöntemler</span><span class="sxs-lookup"><span data-stu-id="6e478-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="6e478-112">Koşullu erişim ile Başlarken</span><span class="sxs-lookup"><span data-stu-id="6e478-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

