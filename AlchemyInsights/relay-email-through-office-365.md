---
title: Office 365 üzerinden e-posta geçişi
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 9/21/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 84443cf1c93e9b19249c573704bc520eaa1c8f48
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: HT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36553010"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email-using-office-365"></a><span data-ttu-id="8183a-102">Office 365 kullanarak e-posta göndermek için çok işlevli cihazı veya uygulamayı ayarlama</span><span class="sxs-lookup"><span data-stu-id="8183a-102">Set up a multifunction device or application to send email using Office 365</span></span>

<span data-ttu-id="8183a-103">Seçenekler ve adımlar hakkında bilgi edinmek için bkz. [Office 365 kullanarak e-posta göndermek için çok işlevli cihazı veya uygulamayı ayarlama](https://support.office.com/article/69f58e99-c550-4274-ad18-c805d654b4c4).</span><span class="sxs-lookup"><span data-stu-id="8183a-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Office 365](https://support.office.com/article/69f58e99-c550-4274-ad18-c805d654b4c4).</span></span>
  
<span data-ttu-id="8183a-104">**Not:** Yakın zamanda çalışmayı durduran bir cihaz veya uygulamanız varsa, lütfen kısa süre önce planlandığı gibi [3DES şifrelemesini devre dışı bırakmaya](https://docs.microsoft.com/office365/securitycompliance/technical-reference-details-about-encryption) başladığımızı aklınızda bulundurun.</span><span class="sxs-lookup"><span data-stu-id="8183a-104">**Note:** If you have a device or application which recently stopped working, please note we have recently begun [disabling the 3DES cipher](https://docs.microsoft.com/office365/securitycompliance/technical-reference-details-about-encryption) as planned.</span></span> <span data-ttu-id="8183a-105">Etkilenen cihazları görmek için [SMTP Kimlik Doğrulama İstemcileri raporuna](https://protection.office.com/mailflow/dashboard) gidin.</span><span class="sxs-lookup"><span data-stu-id="8183a-105">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span> <span data-ttu-id="8183a-106">Yaygın hatalar şunlara benzer olabilir: Kimlik doğrulama başarısızlığı/hatası, TLS başarısızlığı/hatası, Şifreleme algoritması hatası, Algoritma uyuşmazlığı veya Bağlantı kesildi.</span><span class="sxs-lookup"><span data-stu-id="8183a-106">Common errors could be similar to: Authentication failure/error, TLS failure/error, Cipher algorithm error, Algorithm mismatch, or Connection dropped.</span></span> <span data-ttu-id="8183a-107">Sorunu çözmek için:</span><span class="sxs-lookup"><span data-stu-id="8183a-107">To resolve the issue:</span></span>
 - <span data-ttu-id="8183a-108">**Windows Server 2003 IIS SMTP artık çalışmayacak - Windows’un daha yeni bir sürümü gereklidir.**</span><span class="sxs-lookup"><span data-stu-id="8183a-108">**Windows Server 2003 IIS SMTP will no longer work – a newer version of Windows is required.**</span></span>  
 - <span data-ttu-id="8183a-109">Modern bir şifrelemenin desteklenip desteklenmediğini veya bir güncelleştirme olup olmadığını öğrenmek için lütfen uygulama veya cihaz satıcınıza başvurun.</span><span class="sxs-lookup"><span data-stu-id="8183a-109">Please check with your application or device vendor to see if a modern cipher is supported or if there is an update.</span></span>
