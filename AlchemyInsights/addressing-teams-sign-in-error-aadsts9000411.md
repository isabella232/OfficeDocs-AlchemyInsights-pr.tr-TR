---
title: Adresleme Takımlar oturum açma hatası AADSTS9000411
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: b70f1320ea1dfa29e6fa489bd02acfcd1d92971b
ms.sourcegitcommit: 88d2918aa51f4ba10771527380c3e0db0f5a9147
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/20/2020
ms.locfileid: "44358366"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a><span data-ttu-id="270cf-102">Adresleme Takımlar oturum açma hatası AADSTS9000411</span><span class="sxs-lookup"><span data-stu-id="270cf-102">Addressing Teams sign-in error AADSTS9000411</span></span>

<span data-ttu-id="270cf-103">Microsoft Teams'de oturum açtığınızda hata alabilirsiniz: **Üzgünüz, ancak AADSTS9000411'de imzalamanızda sorun yaşıyoruz: İstek düzgün biçimlendirilmemiştir. "login_hint" parametresi çoğaltılır.**</span><span class="sxs-lookup"><span data-stu-id="270cf-103">When signing in to Microsoft Teams, you may receive the error: **Sorry, but we're having trouble with signing you in AADSTS9000411: The request is not properly formatted. The parameter "login_hint" is duplicated.**</span></span>

<span data-ttu-id="270cf-104">Bu sorunu gidermek için lütfen Microsoft Teams istemcilerinizin güncelleştirdiğinden emin olun.</span><span class="sxs-lookup"><span data-stu-id="270cf-104">To address this issue, please ensure your Microsoft Teams clients are updated.</span></span> <span data-ttu-id="270cf-105">İstemcinizi güncelleştirme hakkında daha fazla bilgi için Microsoft [Ekiplerini Güncelleştir'e](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)bakın.</span><span class="sxs-lookup"><span data-stu-id="270cf-105">For more information on updating your client, see [Update Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

<span data-ttu-id="270cf-106">İstemcinizi bir nedenle güncelleştiremiyorsanız, istemcinin oturumu kapatılır, önbelleğe alınan çoğu veriyi temizler.</span><span class="sxs-lookup"><span data-stu-id="270cf-106">If you cannot update your client for some reason, logging off the client will clear most cached data.</span></span> <span data-ttu-id="270cf-107">Ancak, oturum kapatma/oturum açma sonrasında hala sorunlarınız varsa, Takımlar'dan çıkın ve lütfen aşağıdakileri yaparak istemci önbelleğinizi temizleyin:</span><span class="sxs-lookup"><span data-stu-id="270cf-107">However, if you still have issues after logoff/logon, quit Teams and please clear your client cache by doing the following:</span></span>
1. <span data-ttu-id="270cf-108">Microsoft Ekiplerini kapatın.</span><span class="sxs-lookup"><span data-stu-id="270cf-108">Close Microsoft Teams.</span></span>
2. <span data-ttu-id="270cf-109">Şuna gidin: %appdata%\microsoft\teams ve tüm dosyaları silin.</span><span class="sxs-lookup"><span data-stu-id="270cf-109">Go to: %appdata%\microsoft\teams and delete all the files.</span></span>
3. <span data-ttu-id="270cf-110">Microsoft Ekiplerini yeniden açın.</span><span class="sxs-lookup"><span data-stu-id="270cf-110">Reopen Microsoft Teams.</span></span>
