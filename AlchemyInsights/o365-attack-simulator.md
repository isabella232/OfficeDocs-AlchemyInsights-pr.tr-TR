---
title: 2681 saldırı Simülat365 örü
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: dec96238c8438dcf9df176e3e3f20bd8a985b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47759239"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="08c8a-102">Microsoft 365 'de saldırı simülatörü</span><span class="sxs-lookup"><span data-stu-id="08c8a-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="08c8a-103">Saldırı simülatörü eksik mısınız?</span><span class="sxs-lookup"><span data-stu-id="08c8a-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="08c8a-104">Saldırı simülatörü için **Office 365 Gelişmiş tehdit koruması planı 2 (ATP plan 2)** veya **Office 365 Kurumsal E5**gereklidir.</span><span class="sxs-lookup"><span data-stu-id="08c8a-104">Attack Simulator requires **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="08c8a-105">Saldırı simülatörü Office 365 Gelişmiş tehdit koruması plan 1 (ATP planı 1), Office 365 Kurumsal E3 veya herhangi bir Microsoft 365 uygulaması **için kullanılabilir.**</span><span class="sxs-lookup"><span data-stu-id="08c8a-105">Attack Simulator is **not** included in Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="08c8a-106">Benzetilmiş saldırıları başlatmak için kullandığınız hesap, genel yönetici veya Güvenlik Yöneticisi izinleri ve çok faktörlü kimlik doğrulaması (MFA) gerektirir.</span><span class="sxs-lookup"><span data-stu-id="08c8a-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="08c8a-107">Saldırı simülatörü gereksinimleri hakkında daha fazla bilgi için [Bu konuya](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)bakın.</span><span class="sxs-lookup"><span data-stu-id="08c8a-107">For more information about Attack Simulator requirements, see [this topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>

- <span data-ttu-id="08c8a-108">**Kaba, parola** saldırısı benzetimleri ile ilgili bilinmesi gereken önemli noktalar:</span><span class="sxs-lookup"><span data-stu-id="08c8a-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="08c8a-109">Hedef hesaba MFA etkinleştirilmişse ve parola doğru tahmindiyse, hesap tehlikeye düşmesi halinde gösterilmez (ikinci kimlik doğrulama faktörü tamamlanmamış olacaktır).</span><span class="sxs-lookup"><span data-stu-id="08c8a-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="08c8a-110">Parola dosyası 10 MB 'den büyük olamaz.</span><span class="sxs-lookup"><span data-stu-id="08c8a-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="08c8a-111">Her satırda bir parola kullanın ve listedeki son parolanın sonrasına boş bir satır (satır başı) ekleyin.</span><span class="sxs-lookup"><span data-stu-id="08c8a-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="08c8a-112">**Spear sızdırma** ile ilgili bilinmesi gereken önemli noktalar:</span><span class="sxs-lookup"><span data-stu-id="08c8a-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="08c8a-113">Tasarıma göre, **kimlik avı oturum sunucusu URL 'si**için özel bir değer sağlayamıyoruz.</span><span class="sxs-lookup"><span data-stu-id="08c8a-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="08c8a-114">Alıcı, iletiyi kimlik avı olarak bildirmek için [rapor ileti eklentisini etkinleştir](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) seçeneğini kullanırsa, ileti için uyarı alamayabilirsiniz (Bu, benzetilmiş bir saldırı nedeniyle).</span><span class="sxs-lookup"><span data-stu-id="08c8a-114">If a recipient uses the [Enable the Report Message add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="08c8a-115">Raporlar: benzetim işlemi tamamlandıktan sonra, raporu görmek için **saldırı ayrıntıları** 'na tıklayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="08c8a-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="08c8a-116">Saldırı [365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)simülatörü ile ilgili ayrıntılı yönergeler ve yeni özellikler</span><span class="sxs-lookup"><span data-stu-id="08c8a-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>
