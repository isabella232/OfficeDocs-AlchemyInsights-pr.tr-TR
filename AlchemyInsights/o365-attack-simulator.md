---
title: Microsoft 365 2681 Saldırı Simülatörü
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 3dae4768ca62757ce7f92dfc527078c963d72742
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506758"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="50831-102">Microsoft 365'te Saldırı Simülatörü</span><span class="sxs-lookup"><span data-stu-id="50831-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="50831-103">Saldırı Simülatörü'nü kaçırıyor musunuz?</span><span class="sxs-lookup"><span data-stu-id="50831-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="50831-104">Saldırı Simülatörü **Office 365 Gelişmiş Tehdit Koruma Planı 2 (ATP Planı 2)** veya **Office 365 Enterprise E5**gerektirir.</span><span class="sxs-lookup"><span data-stu-id="50831-104">Attack Simulator requires **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="50831-105">Saldırı Simülasyon Aracı, Office 365 Gelişmiş Tehdit Koruma Planı 1 (ATP Plan 1), Office 365 Enterprise E3 veya iş abonelikleri için herhangi bir Microsoft 365 Sürümüne dahil **değildir.**</span><span class="sxs-lookup"><span data-stu-id="50831-105">Attack Simulator is **not** included in Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="50831-106">Benzetimli saldırılar başlatmak için kullandığınız hesap, genel yönetici veya güvenlik yöneticisi izinleri ve çok faktörlü kimlik doğrulama (MFA) gerektirir.</span><span class="sxs-lookup"><span data-stu-id="50831-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="50831-107">Saldırı Simülatörü gereksinimleri hakkında daha fazla bilgi için [bu konuya](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)bakın.</span><span class="sxs-lookup"><span data-stu-id="50831-107">For more information about Attack Simulator requirements, see [this topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>

- <span data-ttu-id="50831-108">**Brute Force Password** saldırı simülasyonları hakkında bilinmesi gereken önemli şeyler:</span><span class="sxs-lookup"><span data-stu-id="50831-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="50831-109">Hedef hesap MFA etkinleştirilmişse ve parola doğru tahmin edildiyse, hesap tehlikeye atılmış olarak gösterilmez (ikinci kimlik doğrulama faktörü eksik olur).</span><span class="sxs-lookup"><span data-stu-id="50831-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="50831-110">Parola dosyası 10 MB'dan büyük olamaz.</span><span class="sxs-lookup"><span data-stu-id="50831-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="50831-111">Satır başına bir parola kullanın ve listedeki son paroladan sonra boş bir satır (satır başı) ekleyin.</span><span class="sxs-lookup"><span data-stu-id="50831-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="50831-112">**Spear Phishing** hakkında bilinmesi gereken önemli şeyler simülasyonları ekleyin:</span><span class="sxs-lookup"><span data-stu-id="50831-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="50831-113">Tasarım gereği, **Kimlik Avı giriş sunucusu URL'si**için özel bir değer sağlayamaz.</span><span class="sxs-lookup"><span data-stu-id="50831-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="50831-114">Bir alıcı, [iletiyi](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) kimlik avı olarak bildirmek için Rapor İletisi eklentisini etkinleştir'i kullanırsa, ileti için uyarı almayabilirsiniz (bu simüle edilmiş bir saldırı olduğu için).</span><span class="sxs-lookup"><span data-stu-id="50831-114">If a recipient uses the [Enable the Report Message add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="50831-115">Raporlar: Benzetimli saldırı tamamlandıktan sonra, raporu görmek için **Saldırı Ayrıntıları'nı** tıklatabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="50831-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="50831-116">Attack Simulator'daki ayrıntılı talimatlar ve yeni özellikler için [Microsoft 365'teki Saldırı Simülatörü'ne](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)bakın.</span><span class="sxs-lookup"><span data-stu-id="50831-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>
