---
title: Kullanıcılarınız kötü amaçlı e-posta mı aldı?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002907"
- "5594"
- "3100017"
- "2578"
ms.openlocfilehash: 2197e7f195d789193798b80cb092d8046eb6e0be
ms.sourcegitcommit: 3c708a4a349b60b59bc623c44fb78674c685f3c2
ms.translationtype: HT
ms.contentlocale: tr-TR
ms.lasthandoff: 02/18/2021
ms.locfileid: "50291812"
---
# <a name="did-your-users-receive-malicious-email"></a><span data-ttu-id="55c81-102">Kullanıcılarınız kötü amaçlı e-posta mı aldı?</span><span class="sxs-lookup"><span data-stu-id="55c81-102">Did your users receive malicious email?</span></span>

- <span data-ttu-id="55c81-103">Artık [Güvenlik ve Uyumluluk Merkezi’nde Yönetici Gönderimleri](https://sip.protection.office.com/reportsubmission)’ni kullanarak kötü amaçlı e-postayı Microsoft’a bildirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="55c81-103">You can now report the malicious email to Microsoft using the [Admin Submissions in Security & Compliance Center](https://sip.protection.office.com/reportsubmission).</span></span>

<span data-ttu-id="55c81-104">[Yönetici gönderimlerinde](https://sip.protection.office.com/reportsubmission) gönderdiğiniz iletiler taranır ve **ayrıntılar** açılır öğesinde aşağıdaki sonuçlar gösterilir:</span><span class="sxs-lookup"><span data-stu-id="55c81-104">Messages that are submitted in [admin submissions](https://sip.protection.office.com/reportsubmission) are scanned, and the following results shown in the **details** flyout:</span></span>

- <span data-ttu-id="55c81-105">Teslim sırasında gönderenin e-posta kimlik doğrulamasında hata olup olmadığı.</span><span class="sxs-lookup"><span data-stu-id="55c81-105">If there was a failure in the sender's email authentication at the time of delivery.</span></span>
- <span data-ttu-id="55c81-106">İletiyle ilgili kararı etkilemiş veya geçersiz kılmış olabilecek bir ilke eşleşmesi hakkında bilgi.</span><span class="sxs-lookup"><span data-stu-id="55c81-106">Information about any policy hits that could have affected or overridden the verdict of a message.</span></span>
- <span data-ttu-id="55c81-107">İletide yer alan URL’lerin veya dosyaların kötü amaçlı olup olmadığını görmek için geçerli etkisizleştirme sonuçları.</span><span class="sxs-lookup"><span data-stu-id="55c81-107">Current detonation results to see if the URLs or files contained in the message were malicious or not.</span></span>
- <span data-ttu-id="55c81-108">Derecelendirme yapanların geri bildirimi</span><span class="sxs-lookup"><span data-stu-id="55c81-108">Feedback from graders</span></span>

<span data-ttu-id="55c81-109">Geçersiz kılma bulunursa, yeniden tarama işlemi birkaç dakika içinde tamamlanır.</span><span class="sxs-lookup"><span data-stu-id="55c81-109">If an override was found, the rescan should complete in several minutes.</span></span> <span data-ttu-id="55c81-110">E-posta kimlik doğrulamasında sorun yoksa veya teslim bir geçersiz kılmadan etkilenmemişse, derecelendirme yapanların geri bildirimi bir gün kadar sürebilir.</span><span class="sxs-lookup"><span data-stu-id="55c81-110">If there wasn't a problem in email authentication or if the delivery wasn't affected by an override, then the feedback from graders could take up to a day.</span></span>

<span data-ttu-id="55c81-111">İleti, URL veya dosyayla ilgili son karara (engellenme - engellenmeme kararı) katılmıyorsanız, yeniden taranması için bir gün sonra iletiyi tekrar gönderin.</span><span class="sxs-lookup"><span data-stu-id="55c81-111">If you disagree with the final verdict on a message, URL or file (blocked vs. not blocked), submit the message again after a day for rescan.</span></span> <span data-ttu-id="55c81-112">İleti yeniden gönderildikten sonra kararın değiştirilme olasılığı yüksektir.</span><span class="sxs-lookup"><span data-stu-id="55c81-112">The chances are high that the verdict would change after submitting the message again.</span></span>

<span data-ttu-id="55c81-113">Bu arada, [bu makalede](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization) sağlanan yönergeleri izleyerek kötü amaçlı e-postayı kullanıcı gelen kutularından kaldırabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="55c81-113">Meanwhile, you can remove malicious email from user inboxes by following the instructions in [this article](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).</span></span>

- <span data-ttu-id="55c81-114">Office 365 için Microsoft Defender kullanan müşteriler:</span><span class="sxs-lookup"><span data-stu-id="55c81-114">Customers with Microsoft Defender for Office 365 can:</span></span>
    - <span data-ttu-id="55c81-115">[Şüpheli e-postayı bulmak ve silmek için Tehdit Gezgini’ni](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered) kullanabilir</span><span class="sxs-lookup"><span data-stu-id="55c81-115">use [Threat Explorer to Find and Delete Suspicious email](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)</span></span>
    - <span data-ttu-id="55c81-116">kötü amaçlı URL’ye [erişimi engellemek için Güvenli Bağlantıları kullanabilir](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links)</span><span class="sxs-lookup"><span data-stu-id="55c81-116">[use Safe Links to block access](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links) to a malicious URL</span></span>
    - <span data-ttu-id="55c81-117">kötü amaçlı URL’leri tıklayan ve bu URL’lere erişen kullanıcıları izleyebilir: [Kimlik avı URL’sini görüntüleme ve karar verilerine tıklama](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)</span><span class="sxs-lookup"><span data-stu-id="55c81-117">track users who clicked and accessed malicious URLs: [View phishing URL and click verdict data](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)</span></span>
    - <span data-ttu-id="55c81-118">el ile [Otomatik Araştırma başlatabilir](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)</span><span class="sxs-lookup"><span data-stu-id="55c81-118">manually [start an Automated Investigation](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)</span></span>

<span data-ttu-id="55c81-119">Ayrıca kötü amaçlı dosyalar ve URL’lerden korunmak için [Kötü amaçlı URL’ler ve dosyalardan koruma](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats) adresinde sağlanan yönergeleri de izleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="55c81-119">You can also protect against malicious files and URLs by following the instructions in [Protection from malicious URLs and files](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).</span></span>