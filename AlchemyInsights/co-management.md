---
title: Birlikte yönetim
ms.author: pebaum
author: pebaum
manager: mnirkhe
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1556"
- "9000080"
ms.openlocfilehash: a10f2d9ee8617cf194c61492be69064d53242318
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/19/2021
ms.locfileid: "50896815"
---
# <a name="co-management"></a><span data-ttu-id="a804a-102">Birlikte yönetim</span><span class="sxs-lookup"><span data-stu-id="a804a-102">Co-management</span></span>

<span data-ttu-id="a804a-103">**Config Manager Karma'dan Intune'a geçişin önkoşulları**</span><span class="sxs-lookup"><span data-stu-id="a804a-103">**Prerequisites for migrating from Config Manager Hybrid to Intune**</span></span>

- <span data-ttu-id="a804a-104">Bu [makaleyi gözden geçirin.](https://docs.microsoft.com/mem/configmgr/mdm/understand/what-happened-to-hybrid)</span><span class="sxs-lookup"><span data-stu-id="a804a-104">Review [this article](https://docs.microsoft.com/mem/configmgr/mdm/understand/what-happened-to-hybrid).</span></span>
- <span data-ttu-id="a804a-105">[Kullanıcılarınıza Intune lisansı ekleyin.](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign)</span><span class="sxs-lookup"><span data-stu-id="a804a-105">[Add an Intune license to your users](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign).</span></span>
- <span data-ttu-id="a804a-106">Birlikte yönetim [yapılandıran Edge](https://www.microsoft.com/edge) tarayıcısını kullanın.</span><span class="sxs-lookup"><span data-stu-id="a804a-106">Use the [Edge browser](https://www.microsoft.com/edge) when configuring Co-management.</span></span>

<span data-ttu-id="a804a-107">Burada, yollu, adım adım bir Ortak yönetim kurulum deneyimi [bulunabilir.](https://admin.microsoft.com/AdminPortal/Home?#/modernonboarding/comanagesetupguide)</span><span class="sxs-lookup"><span data-stu-id="a804a-107">A guided, step-by-step Co-management setup experience can be found [here](https://admin.microsoft.com/AdminPortal/Home?#/modernonboarding/comanagesetupguide).</span></span>

<span data-ttu-id="a804a-108">**Intune tarafından yönetilen cihazlara Config Manager istemcisini yükleme**</span><span class="sxs-lookup"><span data-stu-id="a804a-108">**How to I install the Config Manager client on Intune-managed devices**</span></span>

<span data-ttu-id="a804a-109">[Intune MDM tarafından yönetilen Windows cihazlarına bakın.](https://docs.microsoft.com/mem/configmgr/core/clients/deploy/deploy-clients-to-windows-computers#bkmk_mdm)</span><span class="sxs-lookup"><span data-stu-id="a804a-109">See [Intune MDM-managed Windows devices](https://docs.microsoft.com/mem/configmgr/core/clients/deploy/deploy-clients-to-windows-computers#bkmk_mdm).</span></span>

<span data-ttu-id="a804a-110">**Yalnızca MDM yetkilisini değiştirmek istediğimde ne olacak?**</span><span class="sxs-lookup"><span data-stu-id="a804a-110">**What if I just want to change MDM authority?**</span></span>

<span data-ttu-id="a804a-111">MDM Yetkili bir destek durumu açılmadan değiştirilebilir.</span><span class="sxs-lookup"><span data-stu-id="a804a-111">MDM Authority can be changed without opening a support case.</span></span> <span data-ttu-id="a804a-112">MDM yetkilinizi değiştirme konusunda yardımcı olmak için lütfen aşağıdaki belgeleri gözden geçirin:</span><span class="sxs-lookup"><span data-stu-id="a804a-112">Please review the following documentation to assist in changing your MDM authority:</span></span>

- [<span data-ttu-id="a804a-113">MDM Yetkilisini Yapılandırma Yöneticisi'den Intune tek başına olarak değiştirme</span><span class="sxs-lookup"><span data-stu-id="a804a-113">Change MDM Authority from Configuration Manager to Intune standalone</span></span>](https://docs.microsoft.com/mem/configmgr/mdm/understand/what-happened-to-hybrid)
- [<span data-ttu-id="a804a-114">MDM yetkilisini Intune tek başına yetkilisini Yapılandırma Yöneticisi olarak değiştirme</span><span class="sxs-lookup"><span data-stu-id="a804a-114">Change MDM authority from Intune standalone to Configuration Manager</span></span>](https://docs.microsoft.com/mem/configmgr/mdm/understand/what-happened-to-hybrid)
