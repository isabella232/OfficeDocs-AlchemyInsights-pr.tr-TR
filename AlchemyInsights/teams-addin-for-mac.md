---
title: Teams için bir eklenti
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
- "6166"
- "9003233"
- "9002573"
ms.openlocfilehash: 45df4381688335f10f6699d8b5ff1aaafd6f7257
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/20/2021
ms.locfileid: "52582090"
---
# <a name="teams-add-in-for-mac"></a><span data-ttu-id="6e405-102">Teams için bir eklenti</span><span class="sxs-lookup"><span data-stu-id="6e405-102">Teams add-in for Mac</span></span>

<span data-ttu-id="6e405-103">Mac işletim sistemi Teams eksik hatayla ilgili sorunları gidermek için şu adımları izleyin:</span><span class="sxs-lookup"><span data-stu-id="6e405-103">To troubleshoot a missing Teams add-in for Mac operating system users, follow these steps:</span></span>

<span data-ttu-id="6e405-104">**1. Adım:** Karma Kimlik Exchange Şirket İçi (2016 CU3 veya sonrası gerekli) kullanıyorsanız, Karma Modern Kimlik Doğrulaması'nın doğru yapılandırıldığından emin olmak için Test-HMA.ps1 aracını kullanın.</span><span class="sxs-lookup"><span data-stu-id="6e405-104">**Step 1:** If you have Hybrid Exchange On-Premises (2016 CU3 or later required), use the Test-HMA.ps1 tool to confirm that Hybrid Modern Authentication is correctly configured.</span></span> <span data-ttu-id="6e405-105">Daha fazla bilgi için [bkz. iOS](https://aka.ms/TestHMAEAS)ve Android için Outlook Karma Modern Kimlik Doğrulama kurulumu doğrulama.</span><span class="sxs-lookup"><span data-stu-id="6e405-105">For more info, see [Validating Hybrid Modern Authentication setup for Outlook for iOS and Android](https://aka.ms/TestHMAEAS).</span></span>  

<span data-ttu-id="6e405-106">**Not** ETKIalanı\kullanıcıadı değil UPN [adres biçimini (örneğin, username@contoso.com)](mailto:username@contoso.com)kullanın.</span><span class="sxs-lookup"><span data-stu-id="6e405-106">**Note** Use the UPN address format (for example, [username@contoso.com](mailto:username@contoso.com)), not domain\username.</span></span> <span data-ttu-id="6e405-107">Bu, e-posta kutusu Exchange Online alın.</span><span class="sxs-lookup"><span data-stu-id="6e405-107">Do this even for users with Exchange Online mailboxes.</span></span>

<span data-ttu-id="6e405-108">**2. Adım:** Kullanıcının Araçlar Hesapları   >  ... oturum Mac için Outlook hesabı bulup seçin.</span><span class="sxs-lookup"><span data-stu-id="6e405-108">**Step 2:** Have the user go to **Tools** > **Accounts**... in Outlook for Mac, and find and select the account.</span></span> <span data-ttu-id="6e405-109">Listelenen kullanıcı adlarının UPN biçiminde olduğunu [](mailto:username@contoso.com)onaylayın (örneğin, username@contoso.com).</span><span class="sxs-lookup"><span data-stu-id="6e405-109">Confirm the username listed is in UPN format (for example, [username@contoso.com](mailto:username@contoso.com)).</span></span>

<span data-ttu-id="6e405-110">**3. Adım:** Kullanıcının lisanslı bir kullanıcı olduğunu Microsoft Teams onaylayın.</span><span class="sxs-lookup"><span data-stu-id="6e405-110">**Step 3:** Confirm the user is a licensed Microsoft Teams user.</span></span> <span data-ttu-id="6e405-111">Kullanıcının Mac için Office 365, ürün sürümü 16.24 veya sonraki bir sürümünü kullanıyor olması gerekir.</span><span class="sxs-lookup"><span data-stu-id="6e405-111">The user must be using the Office 365 for Mac subscription, product version 16.24 or later.</span></span>