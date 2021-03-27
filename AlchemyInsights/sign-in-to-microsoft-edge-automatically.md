---
title: Microsoft Edge'de otomatik olarak oturum açma
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003848"
- "6898"
- "8333"
- "9004625"
ms.openlocfilehash: 6021991c125f5cb2a33ce8db8fe7717b528bf49b
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398749"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a><span data-ttu-id="abab9-102">Microsoft Edge'de otomatik olarak oturum açma</span><span class="sxs-lookup"><span data-stu-id="abab9-102">Sign in to Microsoft Edge automatically</span></span>

<span data-ttu-id="abab9-103">Microsoft Edge, kullanıcının cihazına göre otomatik olarak oturum açması için işletim sistemi varsayılan hesabını kullanır.</span><span class="sxs-lookup"><span data-stu-id="abab9-103">Microsoft Edge uses the OS default account to automatically sign in a user according to how the user's device is configured.</span></span> 

<span data-ttu-id="abab9-104">Cihaz yapılandırmasının her türüyle bağımlı kullanıcı oturum açma işleminin senaryoları aşağıda açıklanmıştır:</span><span class="sxs-lookup"><span data-stu-id="abab9-104">The scenarios of each type of device configuration and its dependent user sign-in process are described below:</span></span>

- <span data-ttu-id="abab9-105">**Cihaz karma/AAD-J**: Bu seçenek Windows 10, düşük düzey Windows ve buna karşılık gelen sunucu sürümlerinde kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="abab9-105">**The device is hybrid/AAD-J**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="abab9-106">Kullanıcılar, Azure Active Directory (AD) hesaplarıyla otomatik olarak oturum açılır.</span><span class="sxs-lookup"><span data-stu-id="abab9-106">Users are automatically signed in with their Azure Active Directory (AD)accounts.</span></span>
- <span data-ttu-id="abab9-107">**Cihaz etki alanına katılmış durumdadır:** Bu seçenek Windows 10, alt düzey Windows ve buna karşılık gelen sunucu sürümlerinde kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="abab9-107">**The device is domain-joined**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="abab9-108">Varsayılan olarak, etki alanı hesabı olan kullanıcılar otomatik olarak oturum alanmaz; otomatik oturum açma özelliğini etkinleştirmek için **ConfigureOnPremisesAccountAutoSignIn ilkesi kullanın.**</span><span class="sxs-lookup"><span data-stu-id="abab9-108">By default, users with domain accounts are not signed in automatically; to enable automatic sign-in for them, use the **ConfigureOnPremisesAccountAutoSignIn** policy.</span></span> <span data-ttu-id="abab9-109">Azure AD hesapları olan kullanıcılar için otomatik oturum açma özelliğini etkinleştirmek için cihazlarına karma katılmayı göz önünde bulundurabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="abab9-109">To enable automatic sign-in for users with Azure AD accounts, consider hybrid-joining their devices.</span></span>
- <span data-ttu-id="abab9-110">**OS'un** varsayılan hesabı bir Microsoft hesabıdır: Bu seçenek Windows 10 RS3 (sürüm 1709, derleme 10.0.16299) ve sonraki sürümlerde kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="abab9-110">**The OS's default account is a Microsoft account**: This option is available on Windows 10 RS3 (version 1709, build 10.0.16299) and later versions.</span></span> <span data-ttu-id="abab9-111">Senaryonun kurumsal cihazlarda gerçekleşmesi olası değildir.</span><span class="sxs-lookup"><span data-stu-id="abab9-111">The scenario is unlikely to occur on enterprise devices.</span></span> <span data-ttu-id="abab9-112">Bununla birlikte, işletim sistemi varsayılan hesabı bir Microsoft hesabı ise, Microsoft Edge otomatik olarak kullanıcının Microsoft hesabıyla oturum açmasını sağlar.</span><span class="sxs-lookup"><span data-stu-id="abab9-112">However, if the OS default account is a Microsoft account, then Microsoft Edge will automatically sign in the user with the Microsoft account.</span></span>
 
 
