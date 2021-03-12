---
title: Kuruluş içinde e-posta iletilerini arama ve silme
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000260"
- "7257"
ms.openlocfilehash: e935b10083459b81fc58e12bb59c9511defefa6d
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750020"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a><span data-ttu-id="a39b2-102">Kuruluş içinde e-posta iletilerini arama ve silme</span><span class="sxs-lookup"><span data-stu-id="a39b2-102">Search for and delete email messages in your organization</span></span>

<span data-ttu-id="a39b2-103">Şu adımları izleyin:</span><span class="sxs-lookup"><span data-stu-id="a39b2-103">Follow these steps:</span></span>

1. <span data-ttu-id="a39b2-104">Genel yönetici değilseniz, iletileri aramak için hesabınız **eBulma Yöneticisi** rol grubuna veya Uyumluluk Arama yönetimi **rolüne eklenmiştir.**</span><span class="sxs-lookup"><span data-stu-id="a39b2-104">If you're not a global admin, to search for messages your account must be added to the **eDiscovery Manager role group** or **Compliance Search management role**.</span></span> <span data-ttu-id="a39b2-105">İletileri silmek için, Kuruluş Yönetimi rol grubuna **veya Arama** ve Temizleme yönetimi **rolüne katılmanız gerekir.**</span><span class="sxs-lookup"><span data-stu-id="a39b2-105">To delete messages, you'll need to join the **Organization Management role group** or the **Search and Purge management role**.</span></span> <span data-ttu-id="a39b2-106">Bu rollere izinler Güvenlik ve [uyumluluk & atanır.](https://protection.office.com)</span><span class="sxs-lookup"><span data-stu-id="a39b2-106">Permissions to these roles are assigned in the [Security & compliance center.](https://protection.office.com)</span></span>
2. <span data-ttu-id="a39b2-107">[Silinecek iletiyi](https://docs.microsoft.com/office365/securitycompliance/content-search) bulmak için içerik araması oluşturun.</span><span class="sxs-lookup"><span data-stu-id="a39b2-107">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
3. <span data-ttu-id="a39b2-108">[Güvenlik ve Uyumluluk & PowerShell'e bağlanın.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="a39b2-108">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span></span> <span data-ttu-id="a39b2-109">MFA kullanıyorsanız, şu yönergelere bakın: Çok faktörlü kimlik doğrulamasını & Güvenlik merkezi [PowerShell'e bağlanma](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="a39b2-109">If you're using MFA, see these instructions: [Connect to Security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)</span></span>
4. <span data-ttu-id="a39b2-110">İletiyi silin: `New-ComplianceSearchAction` cmdlet'i çalıştırarak iletiyi silin.</span><span class="sxs-lookup"><span data-stu-id="a39b2-110">Delete the message: run the `New-ComplianceSearchAction` cmdlet to delete the message.</span></span> <span data-ttu-id="a39b2-111">Silinen iletiler kullanıcının Kurtarılabilir Öğeler klasörüne taşınır.</span><span class="sxs-lookup"><span data-stu-id="a39b2-111">Deleted messages are moved to a user's Recoverable Items folder.</span></span> <span data-ttu-id="a39b2-112">Örnek komut için [3. Adıma bakın: İletiyi silme.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)</span><span class="sxs-lookup"><span data-stu-id="a39b2-112">For an example command, see [Step 3: Delete the message.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)</span></span>
