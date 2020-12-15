---
title: İOS için cep telefonu/ıpados veya Android için Microsoft Edge 'i dağıtma
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003919"
- "6974"
ms.openlocfilehash: 98ab637b6ca0f2b3cfa98ae897d6ed1d9f36c3cd
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49679947"
---
# <a name="deploy-microsoft-edge-for-mobile-for-iosipados-or-android"></a><span data-ttu-id="55e6c-102">İOS için cep telefonu/ıpados veya Android için Microsoft Edge 'i dağıtma</span><span class="sxs-lookup"><span data-stu-id="55e6c-102">Deploy Microsoft Edge for Mobile for iOS/iPadOS or Android</span></span>

<span data-ttu-id="55e6c-103">Aşağıda özetlenen Kılavuzlu senaryo, iOS, ıpados ve Android cihazları kullanıcılarına Microsoft Edge atamanıza yardımcı olacaktır.</span><span class="sxs-lookup"><span data-stu-id="55e6c-103">The guided scenario summarized below will help you assign Microsoft Edge to users of iOS, iPadOS, and Android devices.</span></span> <span data-ttu-id="55e6c-104">Bu adımları tamamladıktan sonra, Microsoft Intune ilkeleri Microsoft 'un iş için aşağıdaki özelliklerini etkinleştirir:</span><span class="sxs-lookup"><span data-stu-id="55e6c-104">After you complete these steps, Microsoft Intune policies will enable the following features of Microsoft Edge for business:</span></span>

- <span data-ttu-id="55e6c-105">Çift kimlik</span><span class="sxs-lookup"><span data-stu-id="55e6c-105">Dual identity</span></span>
- <span data-ttu-id="55e6c-106">Microsoft Intune uygulama koruma ilkesiyle tümleştirme</span><span class="sxs-lookup"><span data-stu-id="55e6c-106">Integration with Microsoft Intune app protection policy</span></span>
- <span data-ttu-id="55e6c-107">Azure Active Directory uygulama proxy 'Si ile tümleştirme</span><span class="sxs-lookup"><span data-stu-id="55e6c-107">Integration with Azure Active Directory Application Proxy</span></span>
- <span data-ttu-id="55e6c-108">Yönetilen sık kullanılanlar ve giriş sayfası kısayolları</span><span class="sxs-lookup"><span data-stu-id="55e6c-108">Managed favorites and home page shortcuts</span></span>

> [!NOTE]
> <span data-ttu-id="55e6c-109">Kullanıcıların mobil cihazları kaydetenler 'i engellerse, Bu Kılavuzlu senaryo çalışmaz ve kullanıcıların Microsoft Edge 'i kendilerine yüklemesi gerekir.</span><span class="sxs-lookup"><span data-stu-id="55e6c-109">If you blocked users from enrolling mobile devices, this guided scenario will not work and the users will need to install Microsoft Edge on their own.</span></span>

<span data-ttu-id="55e6c-110">İOS için cep telefonu/ıpados veya Android için Microsoft Edge 'i dağıtmak için bkz:</span><span class="sxs-lookup"><span data-stu-id="55e6c-110">To deploy Microsoft Edge for Mobile for iOS/iPadOS or Android, see:</span></span>

1. [<span data-ttu-id="55e6c-111">Önkoşullar</span><span class="sxs-lookup"><span data-stu-id="55e6c-111">Prerequisites</span></span>](https://go.microsoft.com/fwlink/?linkid=2133027)
2. [<span data-ttu-id="55e6c-112">Giriş</span><span class="sxs-lookup"><span data-stu-id="55e6c-112">Introduction</span></span>](https://go.microsoft.com/fwlink/?linkid=2133520)
3. [<span data-ttu-id="55e6c-113">Öğrenmenize</span><span class="sxs-lookup"><span data-stu-id="55e6c-113">Basics</span></span>](https://go.microsoft.com/fwlink/?linkid=2133421)
4. [<span data-ttu-id="55e6c-114">Yapılandırmalarını</span><span class="sxs-lookup"><span data-stu-id="55e6c-114">Configuration</span></span>](https://go.microsoft.com/fwlink/?linkid=2133521)
5. [<span data-ttu-id="55e6c-115">Atamalarla</span><span class="sxs-lookup"><span data-stu-id="55e6c-115">Assignments</span></span>](https://go.microsoft.com/fwlink/?linkid=2132869)
6. [<span data-ttu-id="55e6c-116">Gözden geçirme ve oluşturma</span><span class="sxs-lookup"><span data-stu-id="55e6c-116">Review and creation</span></span>](https://go.microsoft.com/fwlink/?linkid=2133522)
