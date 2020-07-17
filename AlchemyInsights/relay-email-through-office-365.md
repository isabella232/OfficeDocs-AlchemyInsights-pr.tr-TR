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
ms.openlocfilehash: 074a9106553bf3a2a5e563f9ebaca9dfc38111cb
ms.sourcegitcommit: 9872280f71429d2344b0b441e218fba5b3bd3cf7
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/02/2020
ms.locfileid: "45023479"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a><span data-ttu-id="967df-102">E-posta göndermek için bir çok işlevli cihazı veya uygulamayı ayarlama</span><span class="sxs-lookup"><span data-stu-id="967df-102">Set up a multifunction device or application to send email</span></span>

<span data-ttu-id="967df-103">Seçenekleriniz ve adımlar hakkında bilgi edinmek için bkz. [Microsoft 365 kullanarak e-posta göndermek için bir çok işlevli cihazı veya uygulamayı ayarlama](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span><span class="sxs-lookup"><span data-stu-id="967df-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span></span>
  
<span data-ttu-id="967df-104">**Not:** Yakın zamanda çalışmayı durduran bir cihaz veya uygulamanız varsa, lütfen kısa süre önce planlandığı gibi [3DES şifrelemesini devre dışı bırakmaya](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption) başladığımızı aklınızda bulundurun.</span><span class="sxs-lookup"><span data-stu-id="967df-104">**Note:** If you have a device or application that recently stopped working, please note we have recently begun [disabling the 3DES cipher](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption) as planned.</span></span> <span data-ttu-id="967df-105">Etkilenen cihazları görmek için [SMTP Kimlik Doğrulama İstemcileri raporuna](https://protection.office.com/mailflow/dashboard) gidin.</span><span class="sxs-lookup"><span data-stu-id="967df-105">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span> <span data-ttu-id="967df-106">Yaygın hatalar şunlara benzer olabilir: Kimlik doğrulama başarısızlığı/hatası, TLS başarısızlığı/hatası, Şifreleme algoritması hatası, Algoritma uyuşmazlığı veya Bağlantı kesildi.</span><span class="sxs-lookup"><span data-stu-id="967df-106">Common errors could be similar to: Authentication failure/error, TLS failure/error, Cipher algorithm error, Algorithm mismatch, or Connection dropped.</span></span> <span data-ttu-id="967df-107">Sorunu çözmek için:</span><span class="sxs-lookup"><span data-stu-id="967df-107">To resolve the issue:</span></span>

 - <span data-ttu-id="967df-108">**Windows Server 2003 IIS SMTP artık çalışmayacak - Windows’un daha yeni bir sürümü gereklidir.**</span><span class="sxs-lookup"><span data-stu-id="967df-108">**Windows Server 2003 IIS SMTP will no longer work – a newer version of Windows is required.**</span></span>  
 - <span data-ttu-id="967df-109">Modern bir şifrelemenin desteklenip desteklenmediğini veya bir güncelleştirme olup olmadığını öğrenmek için lütfen uygulama veya cihaz satıcınıza başvurun.</span><span class="sxs-lookup"><span data-stu-id="967df-109">Please check with your application or device vendor to see if a modern cipher is supported or if there is an update.</span></span>
