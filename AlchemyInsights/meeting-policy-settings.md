---
title: Toplantı ilkesi ayarları
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
- "9000734"
- "2657"
ms.openlocfilehash: 24a55417df0f89063fbdd9ade6d104be4f8ab49c
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704626"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="6d022-102">Microsoft Teams'de toplantı ilkelerini yönetme</span><span class="sxs-lookup"><span data-stu-id="6d022-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="6d022-103">**Not: İlke değişikliklerinin kullanıcılar için etkili bir şekilde 24 saat kadar sürebilir.**</span><span class="sxs-lookup"><span data-stu-id="6d022-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="6d022-104">Yeni oluşturulan ilkelerde hemen değişiklik yapmayabileceksiniz; 4 saat bekleyin ve yeni oluşturulan ilkeyi yeniden değiştirmeyi deneyin.</span><span class="sxs-lookup"><span data-stu-id="6d022-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="6d022-105">Toplantı ilkeleri, kuruluşta kullanıcılar tarafından zamanlanan toplantılarda toplantı katılımcılarına kullanılabilen özellikleri kontrol etmek için kullanılır.</span><span class="sxs-lookup"><span data-stu-id="6d022-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="6d022-106">Toplantı ilkelerinin bazı özellikleri henüz Teams yönetim merkezinde uygulanmamış olabilir (bunlar, belgelerde "çok yakında" olarak etiketlenmiş olabilir).</span><span class="sxs-lookup"><span data-stu-id="6d022-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="6d022-107">Bu durumda veya Microsoft Teams yönetim merkezinde "İlkeyi şu anda güncelleştireemedik ancak daha sonra yeniden deneyin" gibi bir hata alıyorsanız, Teams toplantı ilkeleri oluşturmak veya değiştirmek için PowerShell'i kullanmanızı öneririz.</span><span class="sxs-lookup"><span data-stu-id="6d022-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="6d022-108">Toplantı ilkeleri hakkında daha fazla bilgi için aşağıdaki kaynaklara bakın:</span><span class="sxs-lookup"><span data-stu-id="6d022-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="6d022-109">İlke oluşturma, değişiklik yapma ve kullanıcıları ilkeye atama hakkında bilgi edinmek için [Bkz. Teams'de toplantı ilkelerini yönetme.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)</span><span class="sxs-lookup"><span data-stu-id="6d022-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="6d022-110">PowerShell cmdlet'lerini kullanarak ilke değişiklikleri yapmak için [Teams PowerShell'e Genel Bakış'a bakın.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)</span><span class="sxs-lookup"><span data-stu-id="6d022-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="6d022-111">Teams toplantı ilkeleri için [Skype Kurumsal PowerShell modülünü](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) kullanmalıdır.</span><span class="sxs-lookup"><span data-stu-id="6d022-111">You need to use the [Skype for Business PowerShell module](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="6d022-112">Daha fazla [bilgi için \*-CsTeamsMeetingPolicy cmdlet'lerinin](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) belgelerini gözden geçirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="6d022-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

