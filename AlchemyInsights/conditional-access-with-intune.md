---
title: Koşullu erişim ile Intune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 2e778bf4fbdb766700fb24b3405b4ddce89253f7
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29935977"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="ac8ca-102">Koşullu erişim ile Intune</span><span class="sxs-lookup"><span data-stu-id="ac8ca-102">Conditional Access with Intune</span></span>

<span data-ttu-id="ac8ca-103">**Koşullu erişim** kullanarak Intune ile 3 adımları gerektirir:</span><span class="sxs-lookup"><span data-stu-id="ac8ca-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="ac8ca-p101">Hangi kaynaklar korunur ve bu kaynaklara erişmek için karşılanması gereken koşulları gerekenleri tanımlayan bir **Koşullu erişim ilkesi** oluşturun. Örneğin, bir aygıtın şirket e-posta erişmeden önce uyumlu olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="ac8ca-p101">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources. For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="ac8ca-p102">Aygıt uyumlu olarak kabul edilmeden önce karşılanması gereken ayarları tanımlamak için bir **Uyumluluk İlkesi** oluşturun. Örneğin, bir aygıt uyumlu kabul edilmeden önce en az 6 basamaklı bir PIN olması gerekir.</span><span class="sxs-lookup"><span data-stu-id="ac8ca-p102">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant. For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="ac8ca-p103">**Uygunluk ilkeleri** hem de **Koşullu erişim ilkeleri** istenen kullanıcı grupları için hedeflenmiş sağlama. Bu, belirli kullanıcı gruplarına Azure Active Directory'de oluşturma gerektirebilir.</span><span class="sxs-lookup"><span data-stu-id="ac8ca-p103">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users. This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="ac8ca-110">Daha fazla bilgi edinin:</span><span class="sxs-lookup"><span data-stu-id="ac8ca-110">Read more:</span></span>
  
- [<span data-ttu-id="ac8ca-111">Koşullu erişim en iyi yöntemler</span><span class="sxs-lookup"><span data-stu-id="ac8ca-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="ac8ca-112">Koşullu erişim ile Başlarken</span><span class="sxs-lookup"><span data-stu-id="ac8ca-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

