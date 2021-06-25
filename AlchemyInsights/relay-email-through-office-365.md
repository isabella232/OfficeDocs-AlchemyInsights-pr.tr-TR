---
title: Microsoft 365 üzerinden e-posta geçişi
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
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 3b07dd4ccc8570e77a9ce30df48f9ac987a1db71
ms.sourcegitcommit: 93292c46464ac94971d11adfb808d066ab8bc406
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/24/2021
ms.locfileid: "53118003"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a><span data-ttu-id="447cf-102">E-posta göndermek için bir çok işlevli cihazı veya uygulamayı ayarlama</span><span class="sxs-lookup"><span data-stu-id="447cf-102">Set up a multifunction device or application to send email</span></span>

<span data-ttu-id="447cf-103">Seçenekleriniz ve adımlar hakkında bilgi edinmek için bkz. [Microsoft 365 kullanarak e-posta göndermek için bir çok işlevli cihazı veya uygulamayı ayarlama](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span><span class="sxs-lookup"><span data-stu-id="447cf-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Microsoft 365](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span></span>
  
<span data-ttu-id="447cf-104">Yakın zamanda çalışmayı durduran bir cihazınız veya uygulamanız varsa en yaygın sorunlar:</span><span class="sxs-lookup"><span data-stu-id="447cf-104">If you have a device or application that recently stopped working, the most common issues are:</span></span>

- <span data-ttu-id="447cf-105">**SMTP Auth istemci gönderimi kullanılırken kimlik doğrulama ile ilgili hatalar** Yakın zamanda SMTP Kimlik Doğrulaması'nın çalışma yöntemiyle ilgili bazı değişiklikler yaptık.</span><span class="sxs-lookup"><span data-stu-id="447cf-105">**Authentication related errors while using SMTP Auth client submission** We recently made some changes related to how SMTP Authentication works.</span></span> <span data-ttu-id="447cf-106">Sorunları çözme hakkında daha fazla bilgi için, Microsoft 365 veya LOB kullanarak e-posta gönderen [yazıcılar,](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful)tarayıcılar ve LOB uygulamalarıyla ilgili sorunları düzeltme bölümünün kimlik doğrulama başarısız Office 365.</span><span class="sxs-lookup"><span data-stu-id="447cf-106">For more information about how to resolve issues, see the authentication unsuccessful section of [Fix issues with printers, scanners, and LOB applications that send email using Microsoft 365 or Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful).</span></span>
- <span data-ttu-id="447cf-107">**Güvenli bir veri bağlantısı yaparken yalnızca TLS 1.2 sürümünü kabul Office 365** Güvenli bağlantı (TLS) kullanıyorsanız, uygulama cihazınızın TLS 1.2'yi desteklediğine emin olun.</span><span class="sxs-lookup"><span data-stu-id="447cf-107">**We accept only the TLS 1.2 version while making a secure connection to Office 365** If you're using Secure connection (TLS), make sure your application device supports TLS 1.2.</span></span> <span data-ttu-id="447cf-108">Daha fazla bilgi için bkz. [TlS 1.2 için Office 365 ve Office 365 GCC.](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)</span><span class="sxs-lookup"><span data-stu-id="447cf-108">For more information, see [Preparing for TLS 1.2 in Office 365 and Office 365 GCC](/microsoft-365/compliance/prepare-tls-1.2-in-office-365).</span></span>
 
<span data-ttu-id="447cf-109">Diğer sorunlar ve çözümler için bkz. Microsoft 365 veya LOB kullanarak e-posta gönderen [yazıcılar, tarayıcılar ve LOB Office 365.](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off)</span><span class="sxs-lookup"><span data-stu-id="447cf-109">For other issues and solutions, see [Fix issues with printers, scanners, and LOB applications that send email using Microsoft 365 or Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off).</span></span>

<span data-ttu-id="447cf-110">Etkilenen cihazları görmek için [SMTP Kimlik Doğrulama İstemcileri raporuna](https://protection.office.com/mailflow/dashboard) gidin.</span><span class="sxs-lookup"><span data-stu-id="447cf-110">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span>

<span data-ttu-id="447cf-111">**Not:** Exchange Online toplu posta senaryolarına uyum sağlar.</span><span class="sxs-lookup"><span data-stu-id="447cf-111">**Note**: Exchange Online doesn't accommodate bulk-mailing scenarios.</span></span> <span data-ttu-id="447cf-112">Toplu ticari e-posta göndermek için (örneğin, müşteri bültenleri), bu hizmetlerde özelleştirilmiş üçüncü taraf sağlayıcıları kullansanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="447cf-112">To send bulk commercial email (for example, customer newsletters), you should use third-party providers that specialize in these services.</span></span>
