---
title: Microsoft 365'te 2681 Attack Ayrıca
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
ms.openlocfilehash: e7d71fdb77b4a047c1998e9aba75cdd469a936a8
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52545746"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="2434c-102">Saldırı Saldırı Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="2434c-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="2434c-103">Saldırı Uçak'larını mı kaybettiniz?</span><span class="sxs-lookup"><span data-stu-id="2434c-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="2434c-104">Attack Defender, **Plan 2 veya Office 365** **E5** için Microsoft Defender Office 365 Kurumsal gerektirir.</span><span class="sxs-lookup"><span data-stu-id="2434c-104">Attack Simulator requires **Microsoft Defender for Office 365 Plan 2** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="2434c-105">Attack **Evet,** Plan 1, Office 365 Kurumsal E3 veya herhangi bir Office 365 için Microsoft Defender'a İş için Microsoft 365 Uygulamaları değildir.</span><span class="sxs-lookup"><span data-stu-id="2434c-105">Attack Simulator is **not** included in Microsoft Defender for Office 365 Plan 1, Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="2434c-106">Benzetimi yapılan saldırılar başlatmak için kullanabileceğiniz hesap, genel yönetici veya güvenlik yöneticisi izinlerini ve Çok Faktörlü Kimlik Doğrulaması (MFA) gerektirir.</span><span class="sxs-lookup"><span data-stu-id="2434c-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="2434c-107">SaldırıYanı gereksinimleri hakkında daha fazla bilgi için [bu konuya bakın.](/microsoft-365/security/office-365-security/attack-simulator)</span><span class="sxs-lookup"><span data-stu-id="2434c-107">For more information about Attack Simulator requirements, see [this topic](/microsoft-365/security/office-365-security/attack-simulator).</span></span>

- <span data-ttu-id="2434c-108">Force Force Password saldırı **benzetimleri hakkında önemli** şeyler:</span><span class="sxs-lookup"><span data-stu-id="2434c-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="2434c-109">Hedef hesap MFA'nın etkin olduğu ve parolanın doğru tahmin edilmiş olması, hesabın güvenliği ihlal edilmiş olarak göstermez (ikinci kimlik doğrulama faktörü eksik olur).</span><span class="sxs-lookup"><span data-stu-id="2434c-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="2434c-110">Parola dosyası 10 MB'den büyük olabilir.</span><span class="sxs-lookup"><span data-stu-id="2434c-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="2434c-111">Her satıra bir parola kullanın ve listede son paroladan sonra boş bir satır (satır başı) ekleyin.</span><span class="sxs-lookup"><span data-stu-id="2434c-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="2434c-112">Phishing ekleme **benzetimleri hakkında bilmek gereken** önemli şeyler:</span><span class="sxs-lookup"><span data-stu-id="2434c-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="2434c-113">Tasarım olarak, Kimlik avı oturum açma sunucusu **URL'si için özel bir değer sağ yoktur.**</span><span class="sxs-lookup"><span data-stu-id="2434c-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="2434c-114">Alıcı iletiyi [](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) kimlik avı olarak raporu yapmak için Rapor İletiyi Etkinleştir eklentilerini kullanırsa, iletiyle ilgili uyarı alamayabilirsiniz (çünkü bu sanal bir saldırıdır).</span><span class="sxs-lookup"><span data-stu-id="2434c-114">If a recipient uses the [Enable the Report Message add-in](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="2434c-115">Raporlar: Benzetimi yapılan saldırı tamamlandıktan sonra, Saldırı Ayrıntıları'nın **üzerine** tıklar ve raporu görebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="2434c-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="2434c-116">Attack Ayrıca'daki ayrıntılı yönergeler ve yeni özellikler için Saldırı [Saldırı'ya Microsoft 365.](/microsoft-365/security/office-365-security/attack-simulator)</span><span class="sxs-lookup"><span data-stu-id="2434c-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](/microsoft-365/security/office-365-security/attack-simulator).</span></span>
