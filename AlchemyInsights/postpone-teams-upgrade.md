---
title: Ekipleri yükseltme
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2737"
- "4000006"
ms.openlocfilehash: ae0611df247790200d0192e018ff5f0128f23cb4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741791"
---
# <a name="how-to-postpone-the-microsoft-driven-teams-upgrade"></a><span data-ttu-id="cb116-102">Microsoft 'un yönettiği ekipler yükseltmesini ertelemeyi bırakma</span><span class="sxs-lookup"><span data-stu-id="cb116-102">How to postpone the Microsoft-driven Teams upgrade</span></span>

<span data-ttu-id="cb116-103">**Önemli**: destek tanılaması kullanarak bunu sizin için düzeltmeye yardımcı olabiliriz ancak yeni yönetim merkezini kullanmıyorsanız.</span><span class="sxs-lookup"><span data-stu-id="cb116-103">**Important**: We can help fix this for you using a support diagnostic, but it looks like you are not using the New Admin Center.</span></span> <span data-ttu-id="cb116-104">Yeni yönetim merkezini kullanmak için, sağ üstteki **yeni yönetim merkezini** belirten geçiş</span><span class="sxs-lookup"><span data-stu-id="cb116-104">To use the New Admin Center, slide the toggle in the top right that says **new admin center** to the right.</span></span> <span data-ttu-id="cb116-105">Yeni yönetim merkezini kullanarak, **Yardım mı gerekiyor?** pencere öğesini tıklatın, "ekip yükseltmesini ertele" yazın ve ardından tanılama 'yı çalıştırmak için istemleri izleyin.</span><span class="sxs-lookup"><span data-stu-id="cb116-105">Using the New Admin Center, click the **Need Help?** widget, type "Postpone Teams Upgrade", then follow the prompts to run the diagnostic.</span></span>

<span data-ttu-id="cb116-106">Skype Kurumsal 'dan Microsoft ekipleri için Microsoft tabanlı bir otomatik yükseltme hakkında iletişim aldıysanız ve otomatik yükseltmeyi daha sonraki bir tarihe ertelemek istiyorsanız, genel yöneticiniz [Ekip Yöneticisi portalında](https://admin.teams.microsoft.com/dashboard) oturum açabilir ve Microsoft ekipleri yükseltme altında **durum Yenile** düğmesini seçtikten sonra **ertele** düğmesini seçin.</span><span class="sxs-lookup"><span data-stu-id="cb116-106">If you received communication about a Microsoft-driven automated upgrade from Skype for Business to Microsoft Teams, and you wish to postpone the automated upgrade to a later date, your Global Admin can log in to the [Teams Admin portal](https://admin.teams.microsoft.com/dashboard) and, after selecting the **Refresh Status** button under Microsoft Teams Upgrade, select the **Postpone** button.</span></span> <span data-ttu-id="cb116-107">Kiracınızın otomatik yükseltmesinin Microsoft ekipleri için yeni tarihini görmek için, ekip Yöneticisi portalı sayfasını yenileyin.</span><span class="sxs-lookup"><span data-stu-id="cb116-107">To see the new date for your tenant's automated upgrade to Microsoft Teams, refresh the Teams Admin portal page.</span></span>

<span data-ttu-id="cb116-108">**Not:** **Ertele** düğmesi yalnızca otomatik yükseltme ile ilgili ileti merkezi bildirimini aldığınızda kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="cb116-108">**Note:** The **Postpone** button will only be available if you have received the message center notification regarding the automated upgrade.</span></span> 

<span data-ttu-id="cb116-109">Genel Yöneticiler, geçerli yükseltme durumları hakkında daha fazla bilgi edinmek için [Get-CsTeamsUpgradeStatus](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) 'ı çalıştırabilir.</span><span class="sxs-lookup"><span data-stu-id="cb116-109">Global Admins can also run [Get-CsTeamsUpgradeStatus](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) to learn more about their current upgrade status.</span></span>
