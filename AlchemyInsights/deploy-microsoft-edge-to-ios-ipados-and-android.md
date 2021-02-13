---
title: Microsoft Edge'i iOS, iPadOS ve Android'e dağıtma
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8241"
- "9004604"
ms.openlocfilehash: 524e87ab57e29823361053093708c83831f19687
ms.sourcegitcommit: 03378c78eadac5d950802dcbacc328bca3314032
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 02/10/2021
ms.locfileid: "50194584"
---
# <a name="deploy-microsoft-edge-to-ios-ipados-and-android"></a><span data-ttu-id="e2074-102">Microsoft Edge'i iOS, iPadOS ve Android'e dağıtma</span><span class="sxs-lookup"><span data-stu-id="e2074-102">Deploy Microsoft Edge to iOS, iPadOS, and Android</span></span>

<span data-ttu-id="e2074-103">Aşağıda özetlenen kılavuzlu senaryo, Microsoft Edge'i iOS, iPadOS ve Android cihazları kullanıcılarına atamanıza yardımcı olur.</span><span class="sxs-lookup"><span data-stu-id="e2074-103">The guided scenario summarized below will help you assign Microsoft Edge to users of iOS, iPadOS, and Android devices.</span></span>

> [!NOTE]
> <span data-ttu-id="e2074-104">Kullanıcıların mobil cihazları kaydetmesini engellemiş olursanız, bu kılavuzlu senaryo işe yaramadı ve kullanıcıların Microsoft Edge'i kendi başına yüklemeleri gerekir.</span><span class="sxs-lookup"><span data-stu-id="e2074-104">If you blocked users from enrolling mobile devices, this guided scenario won't work and the users will need to install Microsoft Edge on their own.</span></span>

<span data-ttu-id="e2074-105">Rehberli senaryo aşağıdaki adımları içerir:</span><span class="sxs-lookup"><span data-stu-id="e2074-105">The guided scenario involves the following steps:</span></span>

1. [<span data-ttu-id="e2074-106">Önkoşullar</span><span class="sxs-lookup"><span data-stu-id="e2074-106">Prerequisites</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#prerequisites)
2. [<span data-ttu-id="e2074-107">Giriş</span><span class="sxs-lookup"><span data-stu-id="e2074-107">Introduction</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-1---introduction)
3. [<span data-ttu-id="e2074-108">Temel Bilgiler</span><span class="sxs-lookup"><span data-stu-id="e2074-108">Basics</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-2---basics)
4. [<span data-ttu-id="e2074-109">Yapılandırma</span><span class="sxs-lookup"><span data-stu-id="e2074-109">Configuration</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-3---configuration)
5. [<span data-ttu-id="e2074-110">Ödevler</span><span class="sxs-lookup"><span data-stu-id="e2074-110">Assignments</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-4---assignments)
6. [<span data-ttu-id="e2074-111">Gözden geçirme ve oluşturma</span><span class="sxs-lookup"><span data-stu-id="e2074-111">Review and creation</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-5---review--create)

<span data-ttu-id="e2074-112">Rehberli senaryoda adımları tamamlandıktan sonra, Microsoft Intune ilkeleri microsoft Edge İş'in aşağıdaki özelliklerini etkinleştirir:</span><span class="sxs-lookup"><span data-stu-id="e2074-112">After you complete the steps in the guided scenario, Microsoft Intune policies will enable the following features of Microsoft Edge for business:</span></span>

- <span data-ttu-id="e2074-113">Çift kimlik</span><span class="sxs-lookup"><span data-stu-id="e2074-113">Dual identity</span></span>
- <span data-ttu-id="e2074-114">Microsoft Intune uygulama koruma ilkesiyle tümleştirme</span><span class="sxs-lookup"><span data-stu-id="e2074-114">Integration with Microsoft Intune app protection policy</span></span>
- <span data-ttu-id="e2074-115">Azure Active Directory Uygulama Ara Sunucusu ile tümleştirme</span><span class="sxs-lookup"><span data-stu-id="e2074-115">Integration with Azure Active Directory Application Proxy</span></span>
- <span data-ttu-id="e2074-116">Yönetilen sık kullanılanlar ve giriş sayfası kısayolları</span><span class="sxs-lookup"><span data-stu-id="e2074-116">Managed favorites and home page shortcuts</span></span>
