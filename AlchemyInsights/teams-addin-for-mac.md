---
title: Mac için ekip eklentisi
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "9003233"
ms.openlocfilehash: 1e5f6d66386398ad8600f9383f9f7a1dcf0ce69f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670348"
---
# <a name="teams-add-in-for-mac"></a><span data-ttu-id="276ab-102">Mac için ekip eklentisi</span><span class="sxs-lookup"><span data-stu-id="276ab-102">Teams add-in for Mac</span></span>

<span data-ttu-id="276ab-103">Mac işletim sistemi kullanıcıları için eksik bir ekip eklentisi sorunlarını gidermek için aşağıdaki adımları izleyin:</span><span class="sxs-lookup"><span data-stu-id="276ab-103">To troubleshoot a missing Teams add-in for Mac operating system users, follow these steps:</span></span>

<span data-ttu-id="276ab-104">**Adım 1:** Şirket Içi karma Exchange 'niz varsa (2016 CU3 veya üstü gerekliyse) karma modern kimlik doğrulamasının doğru yapılandırıldığını onaylamak için Test-HMA.ps1 aracı 'nı kullanın.</span><span class="sxs-lookup"><span data-stu-id="276ab-104">**Step 1:** If you have Hybrid Exchange On-Premises (2016 CU3 or later required), use the Test-HMA.ps1 tool to confirm that Hybrid Modern Authentication is correctly configured.</span></span> <span data-ttu-id="276ab-105">Daha fazla bilgi için [iOS ve Android Için Outlook 'Ta karma modern kimlik doğrulama kurulumunu doğrulama](https://aka.ms/AA980zq)konusuna bakın.</span><span class="sxs-lookup"><span data-stu-id="276ab-105">For more info, see [Validating Hybrid Modern Authentication setup for Outlook for iOS and Android](https://aka.ms/AA980zq).</span></span>  

<span data-ttu-id="276ab-106">**Not** UPN adres biçimini kullanın (örneğin, [username@contoso.com](mailto:username@contoso.com)), etkialanı \ KullanıcıAdı.</span><span class="sxs-lookup"><span data-stu-id="276ab-106">**Note** Use the UPN address format (for example, [username@contoso.com](mailto:username@contoso.com)), not domain\username.</span></span> <span data-ttu-id="276ab-107">Exchange Online posta kutularına sahip kullanıcılar için bunu yapın.</span><span class="sxs-lookup"><span data-stu-id="276ab-107">Do this even for users with Exchange Online mailboxes.</span></span>

<span data-ttu-id="276ab-108">**Adım 2:** Kullanıcının **Araçlar**  >  **hesaplar**... Mac için Outlook 'ta, hesabı bulup seçin.</span><span class="sxs-lookup"><span data-stu-id="276ab-108">**Step 2:** Have the user go to **Tools** > **Accounts**... in Outlook for Mac, and find and select the account.</span></span> <span data-ttu-id="276ab-109">Listelenen kullanıcı adının UPN biçiminde olduğunu doğrulayın (örneğin, [username@contoso.com](mailto:username@contoso.com)).</span><span class="sxs-lookup"><span data-stu-id="276ab-109">Confirm the username listed is in UPN format (for example, [username@contoso.com](mailto:username@contoso.com)).</span></span>

<span data-ttu-id="276ab-110">**Adım 3:** Kullanıcının lisanslı bir Microsoft ekipleri kullanıcısı olduğunu onaylayın.</span><span class="sxs-lookup"><span data-stu-id="276ab-110">**Step 3:** Confirm the user is a licensed Microsoft Teams user.</span></span> <span data-ttu-id="276ab-111">Kullanıcı, Mac için Office 365 aboneliğini, ürün sürümü 16,24 veya sonrasını kullanıyor olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="276ab-111">The user must be using the Office 365 for Mac subscription, product version 16.24 or later.</span></span>