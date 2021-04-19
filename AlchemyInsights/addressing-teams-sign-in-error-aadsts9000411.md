---
title: Teams oturum açma hatasını ele aADSTS9000411
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: 7b0e90e3fea716df649ec906ad8b3008386684be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822007"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a><span data-ttu-id="62eca-102">Teams oturum açma hatasını ele aADSTS9000411</span><span class="sxs-lookup"><span data-stu-id="62eca-102">Addressing Teams sign-in error AADSTS9000411</span></span>

<span data-ttu-id="62eca-103">Microsoft Teams'de oturum aken şu hatayı alabilirsiniz: Üzgünüz, ancak AADSTS9000411'da oturum a açmayla ilgili sorun gidermeyle ilgili bir sorun oluştu: İstek düzgün **biçimlendir değil. "Login_hint" parametresi çoğaltıldı.**</span><span class="sxs-lookup"><span data-stu-id="62eca-103">When signing in to Microsoft Teams, you may receive the error: **Sorry, but we're having trouble with signing you in AADSTS9000411: The request is not properly formatted. The parameter "login_hint" is duplicated.**</span></span>

<span data-ttu-id="62eca-104">Bu sorunu gidermek için lütfen Microsoft Teams istemcilerinizi güncelleştirilir.</span><span class="sxs-lookup"><span data-stu-id="62eca-104">To address this issue, please ensure your Microsoft Teams clients are updated.</span></span> <span data-ttu-id="62eca-105">İstemcinizi güncelleştirme hakkında daha fazla bilgi için bkz. [Microsoft Teams'i güncelleştirme.](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)</span><span class="sxs-lookup"><span data-stu-id="62eca-105">For more information on updating your client, see [Update Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

<span data-ttu-id="62eca-106">İstemcinizi herhangi bir nedenden dolayı güncelleştire değilken, istemciyi kapatsanız önbelleğe alınan verilerin çoğunu temiz olur.</span><span class="sxs-lookup"><span data-stu-id="62eca-106">If you cannot update your client for some reason, logging off the client will clear most cached data.</span></span> <span data-ttu-id="62eca-107">Ancak logoff/oturum açma sonrasında da sorun yaşıyorsanız, Teams'den çıkın ve lütfen şunları yaparak istemci önbelleğinizi temizleyin:</span><span class="sxs-lookup"><span data-stu-id="62eca-107">However, if you still have issues after logoff/logon, quit Teams and please clear your client cache by doing the following:</span></span>
1. <span data-ttu-id="62eca-108">Microsoft Teams'i kapatın.</span><span class="sxs-lookup"><span data-stu-id="62eca-108">Close Microsoft Teams.</span></span>
2. <span data-ttu-id="62eca-109">%appdata%\microsoft\teams klasörüne gidin ve tüm dosyaları silin.</span><span class="sxs-lookup"><span data-stu-id="62eca-109">Go to: %appdata%\microsoft\teams and delete all the files.</span></span>
3. <span data-ttu-id="62eca-110">Microsoft Teams'i yeniden açın.</span><span class="sxs-lookup"><span data-stu-id="62eca-110">Reopen Microsoft Teams.</span></span>
