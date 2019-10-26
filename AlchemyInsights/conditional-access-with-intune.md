---
title: Intune ile Koşullu Erişim
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: e147e7460ee6a786e577a43c0b8355fc27ee367b
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/25/2019
ms.locfileid: "36505014"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="6d1e2-102">Intune ile Koşullu Erişim</span><span class="sxs-lookup"><span data-stu-id="6d1e2-102">Conditional Access with Intune</span></span>

<span data-ttu-id="6d1e2-103">**Koşullu Erişimi** Intune ile kullanmak 3 adım gerektirir:</span><span class="sxs-lookup"><span data-stu-id="6d1e2-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="6d1e2-104">Hangi kaynakların korunduğunu ve bu kaynaklara erişmek için hangi koşulların karşılanması gerektiğini tanımlayan **koşullu erişim ilkesi** oluşturun.</span><span class="sxs-lookup"><span data-stu-id="6d1e2-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="6d1e2-105">Örneğin, bir aygıtın şirket e-postasına erişmeden önce uyumlu olması gerekir.</span><span class="sxs-lookup"><span data-stu-id="6d1e2-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="6d1e2-106">Aygıt uyumlu kabul edilmeden önce karşılanması gereken ayarları tanımlamak için bir **Uyumluluk İlkesi** oluşturun.</span><span class="sxs-lookup"><span data-stu-id="6d1e2-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="6d1e2-107">Örneğin, bir aygıtın uyumlu kabul edilmeden önce en az 6 basamaklı bir iğneye sahip olması gerekir.</span><span class="sxs-lookup"><span data-stu-id="6d1e2-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="6d1e2-108">Hem **Uyumluluk İlkeleri'nin** hem de **Koşullu Erişim İlkelerinin** istenilen kullanıcı gruplarına hedef olmasını sağlamak.</span><span class="sxs-lookup"><span data-stu-id="6d1e2-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="6d1e2-109">Bu, Azure Etkin Dizini'nde belirli kullanıcı grupları oluşturulmasını gerektirebilir.</span><span class="sxs-lookup"><span data-stu-id="6d1e2-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="6d1e2-110">Devamını oku:</span><span class="sxs-lookup"><span data-stu-id="6d1e2-110">Read more:</span></span>
  
- [<span data-ttu-id="6d1e2-111">Koşullu Erişim en iyi uygulamalar</span><span class="sxs-lookup"><span data-stu-id="6d1e2-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="6d1e2-112">Koşullu Erişim ile başlarken</span><span class="sxs-lookup"><span data-stu-id="6d1e2-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

