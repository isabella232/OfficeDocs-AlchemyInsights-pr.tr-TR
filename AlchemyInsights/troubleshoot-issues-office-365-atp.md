---
title: Office 365 Gelişmiş Tehdit Koruması (ATP) ile ilgili sorun giderme sorunları
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: f1dc675c8a8217ea2824ad46e029bfa303303e6a
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511132"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a><span data-ttu-id="426f1-102">Office 365 ATP ile ilgili sorun giderme sorunları</span><span class="sxs-lookup"><span data-stu-id="426f1-102">Troubleshoot issues with Office 365 ATP</span></span>

- <span data-ttu-id="426f1-103">**E-posta iletisi tesliminde gecikmeleri fark**eder misiniz?</span><span class="sxs-lookup"><span data-stu-id="426f1-103">**Notice delays with email message delivery**?</span></span> <span data-ttu-id="426f1-104">ATP Güvenli Ekleri ilkeleriniz için Dinamik Teslim seçeneğini kullanmayı deneyin.</span><span class="sxs-lookup"><span data-stu-id="426f1-104">Try using the Dynamic Delivery option for your ATP Safe Attachments policies.</span></span> <span data-ttu-id="426f1-105">Bu, alıcıları kötü amaçlı dosyalardan korurken e-posta iletisi tesliminde gecikmeleri önler.</span><span class="sxs-lookup"><span data-stu-id="426f1-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="426f1-106">**Yanlış pozitif leri veya yanlış negatifleri bildirmek istiyor musunuz?**</span><span class="sxs-lookup"><span data-stu-id="426f1-106">**Do you want to report false positives or false negatives**?</span></span> <span data-ttu-id="426f1-107">Dosyanızı analiz için göndermek için bu bağlantıyı kullanın:[https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span><span class="sxs-lookup"><span data-stu-id="426f1-107">Use this link to submit your file for analysis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span></span>
- <span data-ttu-id="426f1-108">**Kuruluşunuzdaki kişiler arasında gönderilen e-postalar için ATP Güvenli Bağlantılar korumasını etkinleştirebileceğinizi biliyor muydunuz?**</span><span class="sxs-lookup"><span data-stu-id="426f1-108">**Did you know that you can enable ATP Safe Links protection for email sent between people in your organization**?</span></span> <span data-ttu-id="426f1-109">Şu adımları izleyin:</span><span class="sxs-lookup"><span data-stu-id="426f1-109">Follow these steps:</span></span>
    1. <span data-ttu-id="426f1-110">Git https://protection.office.com ve oturum aç.</span><span class="sxs-lookup"><span data-stu-id="426f1-110">Go to https://protection.office.com, and sign in.</span></span>
    2. <span data-ttu-id="426f1-111">Tehdit **yönetimi**  >  **Politikası**  >  **Güvenli Linkler**gidin.</span><span class="sxs-lookup"><span data-stu-id="426f1-111">Go to **Threat management** > **Policy** > **Safe Links**.</span></span>
    3. <span data-ttu-id="426f1-112">**Belirli alıcılar için geçerli olan İlkeler**altında, bir ilkeyi edin (veya ekleyin).</span><span class="sxs-lookup"><span data-stu-id="426f1-112">Under **Policies that apply to specific recipients**, edit (or add) a policy.</span></span>
    4. <span data-ttu-id="426f1-113">**Kuruluş içinde gönderilen iletilere güvenli bağlantılar uygula'yı**seçin.</span><span class="sxs-lookup"><span data-stu-id="426f1-113">Select **Apply safe links to messages sent within the organization**.</span></span>
    5. <span data-ttu-id="426f1-114">İlkinizi kaydedin ve değişikliklerinizin veri merkezinizde çalışması için yaklaşık 30 dakika bekleyin.</span><span class="sxs-lookup"><span data-stu-id="426f1-114">Save your policy, and allow about 30 minutes for your changes to work their way through your datacenter.</span></span>
- <span data-ttu-id="426f1-115">ATP ile ilgili daha fazla yardım almak için [Bkz. Office 365 Gelişmiş Tehdit Koruması.](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp)</span><span class="sxs-lookup"><span data-stu-id="426f1-115">To get more help with ATP, see [Office 365 Advanced Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span></span>