---
title: Toplantı ilkesi ayarları
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "2657"
ms.openlocfilehash: 39151d3a56cc09a8ae2dd77fb7bf1e99066cc77a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825463"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="22a4b-102">Microsoft Teams'de toplantı ilkelerini yönetme</span><span class="sxs-lookup"><span data-stu-id="22a4b-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="22a4b-103">**Not: İlke değişikliklerinin kullanıcılarda etkiliksi 24 saate kadar sürebilir.**</span><span class="sxs-lookup"><span data-stu-id="22a4b-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="22a4b-104">Yeni oluşturulan ilkelerde hemen değişiklik yapmayabileceksiniz; 4 saat bekleyin ve yeni oluşturulan ilkeyi yeniden değiştirmeyi deneyin.</span><span class="sxs-lookup"><span data-stu-id="22a4b-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="22a4b-105">Toplantı ilkeleri, kuruluşta kullanıcılar tarafından zamanlanan toplantılarda toplantı katılımcılarına kullanılabilen özellikleri denetlemede kullanılır.</span><span class="sxs-lookup"><span data-stu-id="22a4b-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="22a4b-106">Toplantı ilkelerinin bazı özellikleri henüz Teams yönetim merkezinde uygulanmamış olabilir (bunlar, belgelerde "çok yakında" olarak etiketlenmiş olabilir).</span><span class="sxs-lookup"><span data-stu-id="22a4b-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="22a4b-107">Bu durumda ya da Microsoft Teams yönetim merkezinde "İlkeyi şu anda güncelleştire miyiz" gibi bir hata alıyorsanız Teams toplantı ilkelerini oluşturmak veya değiştirmek için PowerShell'i kullanmanızı öneririz.</span><span class="sxs-lookup"><span data-stu-id="22a4b-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="22a4b-108">Toplantı ilkeleri hakkında daha fazla bilgi için aşağıdaki kaynaklara bakın:</span><span class="sxs-lookup"><span data-stu-id="22a4b-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="22a4b-109">İlke oluşturma, değişiklik yapma ve kullanıcıları ilkeye atama hakkında bilgi edinmek için bkz. [Teams'te toplantı ilkelerini yönetme.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)</span><span class="sxs-lookup"><span data-stu-id="22a4b-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="22a4b-110">PowerShell cmdlet'lerini kullanarak ilke değişiklikleri yapmak için bkz. [Teams PowerShell'e Genel Bakış.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)</span><span class="sxs-lookup"><span data-stu-id="22a4b-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="22a4b-111">Teams toplantı ilkeleri için [Skype Kurumsal PowerShell modülünü](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) kullanmelisiniz.</span><span class="sxs-lookup"><span data-stu-id="22a4b-111">You need to use the [Skype for Business PowerShell module](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="22a4b-112">Daha fazla [bilgi için \*-CsTeamsMeetingPolicy cmdlet'leri belgelerini](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) gözden geçirme.</span><span class="sxs-lookup"><span data-stu-id="22a4b-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

