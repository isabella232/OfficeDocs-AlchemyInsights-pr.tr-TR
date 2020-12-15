---
title: Microsoft Edge 'de otomatik olarak oturum açma
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
ms.openlocfilehash: 68a1119abd0a3f687b6448bb6e58c6485c239c0f
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/08/2020
ms.locfileid: "49678819"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a><span data-ttu-id="c4a13-102">Microsoft Edge 'de otomatik olarak oturum açma</span><span class="sxs-lookup"><span data-stu-id="c4a13-102">Sign in to Microsoft Edge automatically</span></span>

<span data-ttu-id="c4a13-103">Microsoft Edge, kullanıcının cihazının nasıl yapılandırıldığına bağlı olarak bir kullanıcı için işletim sisteminin varsayılan hesabını kullanır.</span><span class="sxs-lookup"><span data-stu-id="c4a13-103">Microsoft Edge uses the OS's default account to automatically sign in a user according to how the user's device is configured.</span></span> 

<span data-ttu-id="c4a13-104">Her cihaz yapılandırması türünün senaryoları ve bağımlı Kullanıcı oturum açma süreci aşağıda açıklanmıştır:</span><span class="sxs-lookup"><span data-stu-id="c4a13-104">The scenarios of each type of device configuration and its dependent user sign-in process are described below:</span></span>

1. <span data-ttu-id="c4a13-105">**Cihaz karma/AAD-J**: Bu seçenek Windows 10, alt düzey Windows ve ilgili sunucu sürümlerinde kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="c4a13-105">**The device is hybrid/AAD-J**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="c4a13-106">Kullanıcılar Azure Active Directory (AD) hesaplarıyla otomatik olarak imzalanır.</span><span class="sxs-lookup"><span data-stu-id="c4a13-106">Users are automatically signed in with their Azure Active Directory (AD)accounts.</span></span>
2. <span data-ttu-id="c4a13-107">**Cihaz etki alanına bağlı**: Bu seçenek Windows 10, alt düzey Windows ve ilgili sunucu sürümlerinde kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="c4a13-107">**The device is domain-joined**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="c4a13-108">Varsayılan olarak, etki alanı hesabı olan kullanıcılar otomatik olarak imzalanır; otomatik oturum açmayı etkinleştirmek için **ConfigureOnPremisesAccountAutoSignIn** ilkesini kullanın.</span><span class="sxs-lookup"><span data-stu-id="c4a13-108">By default, users with domain accounts are not signed in automatically; to enable automatic sign-in for them, use the **ConfigureOnPremisesAccountAutoSignIn** policy.</span></span> <span data-ttu-id="c4a13-109">Azure AD hesapları olan kullanıcılar için otomatik oturum açmayı etkinleştirmek üzere, onlara karma olarak katılma seçeneğini dikkate alın.</span><span class="sxs-lookup"><span data-stu-id="c4a13-109">To enable automatic sign-in for users with Azure AD accounts, consider hybrid-joining their devices.</span></span>
3. <span data-ttu-id="c4a13-110">**İşletim sisteminin varsayılan hesabı bir Microsoft hesabıdır**: Bu seçenek WINDOWS 10 yalnızca RS3 (sürüm 1709, derleme 10.0.16299) ve sonraki sürümlerde kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="c4a13-110">**The OS's default account is a Microsoft account**: This option is available on Windows 10 RS3 (version 1709, build 10.0.16299) and later versions.</span></span> <span data-ttu-id="c4a13-111">Senaryo kurumsal cihazlarda gerçekleşmiyor olabilir.</span><span class="sxs-lookup"><span data-stu-id="c4a13-111">The scenario is unlikely to occur on enterprise devices.</span></span> <span data-ttu-id="c4a13-112">Ancak, işletim sisteminin varsayılan hesabı bir Microsoft hesabındanda, Microsoft Edge kullanıcının Microsoft hesabıyla otomatik olarak oturum açmasını sağlayacaktır.</span><span class="sxs-lookup"><span data-stu-id="c4a13-112">However, if the OS's default account is a Microsoft account, then Microsoft Edge will automatically sign in the user with the Microsoft account.</span></span>
 
 
