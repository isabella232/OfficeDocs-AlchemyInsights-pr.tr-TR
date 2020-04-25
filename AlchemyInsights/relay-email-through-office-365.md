---
title: Microsoft 365 üzerinden e-posta geçişi
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 4b36caf1841c5292d269812f4ab5ca16a46fbc81
ms.sourcegitcommit: 6a3748f5c05693ca0c19a829287cb8f30635940c
ms.translationtype: HT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43785215"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a><span data-ttu-id="a550f-102">E-posta göndermek için bir çok işlevli cihazı veya uygulamayı ayarlama</span><span class="sxs-lookup"><span data-stu-id="a550f-102">Set up a multifunction device or application to send email</span></span>

<span data-ttu-id="a550f-103">Seçenekleriniz ve adımlar hakkında bilgi edinmek için bkz. [Microsoft 365 kullanarak e-posta göndermek için bir çok işlevli cihazı veya uygulamayı ayarlama](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-office-3).</span><span class="sxs-lookup"><span data-stu-id="a550f-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-office-3).</span></span>
  
<span data-ttu-id="a550f-104">**Not:** Yakın zamanda çalışmayı durduran bir cihaz veya uygulamanız varsa, lütfen kısa süre önce planlandığı gibi [3DES şifrelemesini devre dışı bırakmaya](https://docs.microsoft.com/office365/securitycompliance/technical-reference-details-about-encryption) başladığımızı aklınızda bulundurun.</span><span class="sxs-lookup"><span data-stu-id="a550f-104">**Note:** If you have a device or application that recently stopped working, please note we have recently begun [disabling the 3DES cipher](https://docs.microsoft.com/office365/securitycompliance/technical-reference-details-about-encryption) as planned.</span></span> <span data-ttu-id="a550f-105">Etkilenen cihazları görmek için [SMTP Kimlik Doğrulama İstemcileri raporuna](https://protection.office.com/mailflow/dashboard) gidin.</span><span class="sxs-lookup"><span data-stu-id="a550f-105">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span> <span data-ttu-id="a550f-106">Yaygın hatalar şunlara benzer olabilir: Kimlik doğrulama başarısızlığı/hatası, TLS başarısızlığı/hatası, Şifreleme algoritması hatası, Algoritma uyuşmazlığı veya Bağlantı kesildi.</span><span class="sxs-lookup"><span data-stu-id="a550f-106">Common errors could be similar to: Authentication failure/error, TLS failure/error, Cipher algorithm error, Algorithm mismatch, or Connection dropped.</span></span> <span data-ttu-id="a550f-107">Sorunu çözmek için:</span><span class="sxs-lookup"><span data-stu-id="a550f-107">To resolve the issue:</span></span>
 - <span data-ttu-id="a550f-108">**Windows Server 2003 IIS SMTP artık çalışmayacak - Windows’un daha yeni bir sürümü gereklidir.**</span><span class="sxs-lookup"><span data-stu-id="a550f-108">**Windows Server 2003 IIS SMTP will no longer work – a newer version of Windows is required.**</span></span>  
 - <span data-ttu-id="a550f-109">Modern bir şifrelemenin desteklenip desteklenmediğini veya bir güncelleştirme olup olmadığını öğrenmek için lütfen uygulama veya cihaz satıcınıza başvurun.</span><span class="sxs-lookup"><span data-stu-id="a550f-109">Please check with your application or device vendor to see if a modern cipher is supported or if there is an update.</span></span>
