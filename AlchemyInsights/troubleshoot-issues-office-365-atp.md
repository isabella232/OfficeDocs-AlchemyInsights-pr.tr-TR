---
title: Office için Microsoft Defender 365 (ATP) sorunlarını giderme
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: cf54d5b3b854587202ff1b575889b9602228dd06
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801427"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a><span data-ttu-id="c006d-102">Office 365 ATP ile ilgili sorunları giderme</span><span class="sxs-lookup"><span data-stu-id="c006d-102">Troubleshoot issues with Office 365 ATP</span></span>

- <span data-ttu-id="c006d-103">**E-posta iletisi tesliminde gecikmeler fark** edilsin mi?</span><span class="sxs-lookup"><span data-stu-id="c006d-103">**Notice delays with email message delivery** ?</span></span> <span data-ttu-id="c006d-104">ATP güvenli ekler ilkeleriniz için dinamik teslim seçeneğini kullanmayı deneyin.</span><span class="sxs-lookup"><span data-stu-id="c006d-104">Try using the Dynamic Delivery option for your ATP Safe Attachments policies.</span></span> <span data-ttu-id="c006d-105">Bu, alıcıları kötü niyetli dosyalardan korurken e-posta iletisi gönderme gecikmelerini engellemez.</span><span class="sxs-lookup"><span data-stu-id="c006d-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="c006d-106">**Yanlış pozitif durumları veya yanlış negatifleri raporlamak** mi istiyorsunuz?</span><span class="sxs-lookup"><span data-stu-id="c006d-106">**Do you want to report false positives or false negatives** ?</span></span> <span data-ttu-id="c006d-107">Dosyanızı çözümleme için göndermek üzere bu bağlantıyı kullanın: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span><span class="sxs-lookup"><span data-stu-id="c006d-107">Use this link to submit your file for analysis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span></span>
- <span data-ttu-id="c006d-108">**Kuruluşunuzdaki kişilerin gönderdiği e-posta IÇIN ATP güvenli bağlantılar korumasını etkinleştirebildiğinizi biliyor muydunuz** ?</span><span class="sxs-lookup"><span data-stu-id="c006d-108">**Did you know that you can enable ATP Safe Links protection for email sent between people in your organization** ?</span></span> <span data-ttu-id="c006d-109">Şu adımları izleyin:</span><span class="sxs-lookup"><span data-stu-id="c006d-109">Follow these steps:</span></span>
    1. <span data-ttu-id="c006d-110">Gidin https://protection.office.com ve oturum açın.</span><span class="sxs-lookup"><span data-stu-id="c006d-110">Go to https://protection.office.com, and sign in.</span></span>
    2. <span data-ttu-id="c006d-111">**Tehdit yönetimi**  >  **ilkesi**  >  **güvenli bağlantılarına** gidin.</span><span class="sxs-lookup"><span data-stu-id="c006d-111">Go to **Threat management** > **Policy** > **Safe Links** .</span></span>
    3. <span data-ttu-id="c006d-112">**Belirli alıcılara uygulanan ilkeler** altında, bir ilkeyi düzenleyin (veya ekleyin).</span><span class="sxs-lookup"><span data-stu-id="c006d-112">Under **Policies that apply to specific recipients** , edit (or add) a policy.</span></span>
    4. <span data-ttu-id="c006d-113">**Kuruluş içinde gönderilen iletilere güvenli bağlantılar Uygula** seçeneğini belirleyin.</span><span class="sxs-lookup"><span data-stu-id="c006d-113">Select **Apply safe links to messages sent within the organization** .</span></span>
    5. <span data-ttu-id="c006d-114">İlkenizi kaydedin ve değişikliklerinizin veri merkezinize göre çalışmasını sağlamak için 30 dakikalık bir izin verin.</span><span class="sxs-lookup"><span data-stu-id="c006d-114">Save your policy, and allow about 30 minutes for your changes to work their way through your datacenter.</span></span>
- <span data-ttu-id="c006d-115">ATP ile ilgili daha fazla yardım almak için [Office 365 Için Microsoft Defender](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp)'a bakın.</span><span class="sxs-lookup"><span data-stu-id="c006d-115">To get more help with ATP, see [Microsoft Defender for Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span></span>