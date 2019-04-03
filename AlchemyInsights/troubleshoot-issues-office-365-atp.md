---
title: İle Office 365 Gelişmiş tehdit Koruması (ATP) sorunlarını giderme
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: dbdfe2ddcc4afd4477f66ffd060ddb7093af8fd6
ms.sourcegitcommit: 601aec31e6556286fe5e0fd62827a037cbb6fe17
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/02/2019
ms.locfileid: "31031128"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a><span data-ttu-id="093f7-102">Office 365 KM ile ilgili sorunları giderme</span><span class="sxs-lookup"><span data-stu-id="093f7-102">Troubleshoot issues with Office 365 ATP</span></span>

- <span data-ttu-id="093f7-103">**E-posta ileti teslimi ile bildirim gecikmeleri**?</span><span class="sxs-lookup"><span data-stu-id="093f7-103">**Notice delays with email message delivery**?</span></span> <span data-ttu-id="093f7-104">ATP güvenli ekler ilkelerinizi dinamik teslim seçeneğini kullanmayı deneyin.</span><span class="sxs-lookup"><span data-stu-id="093f7-104">Try using the Dynamic Delivery option for your ATP Safe Attachments policies.</span></span> <span data-ttu-id="093f7-105">Kötü amaçlı dosyaları alıcılar korurken bu e-posta iletisi teslim gecikmelerini önler.</span><span class="sxs-lookup"><span data-stu-id="093f7-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="093f7-106">**Yanlış pozitif durumlar rapor ya da yanlış negatifler istiyor musunuz**?</span><span class="sxs-lookup"><span data-stu-id="093f7-106">**Do you want to report false positives or false negatives**?</span></span> <span data-ttu-id="093f7-107">Dosyanızı analiz için göndermek için bu bağlantıyı kullanın:[https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span><span class="sxs-lookup"><span data-stu-id="093f7-107">Use this link to submit your file for analysis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span></span>
- <span data-ttu-id="093f7-108">**Kuruluşunuzdaki kişiler arasında gönderilen e-posta için güvenli bağlantılar ATP koruma etkinleştirmek biliyor muydunuz**?</span><span class="sxs-lookup"><span data-stu-id="093f7-108">**Did you know that you can enable ATP Safe Links protection for email sent between people in your organization**?</span></span> <span data-ttu-id="093f7-109">İzleyeceğiniz adımlar:</span><span class="sxs-lookup"><span data-stu-id="093f7-109">Follow these steps:</span></span>
    1. <span data-ttu-id="093f7-110">Git https://protection.office.comve oturum açın.</span><span class="sxs-lookup"><span data-stu-id="093f7-110">Go to https://protection.office.com, and sign in.</span></span>
    2. <span data-ttu-id="093f7-111">**Tehdit Yönetimi**Git > **ilke** > **Güvenli bağlantılar**.</span><span class="sxs-lookup"><span data-stu-id="093f7-111">Go to **Threat management** > **Policy** > **Safe Links**.</span></span>
    3. <span data-ttu-id="093f7-112">**Belirli alıcılar için geçerli ilkeleri**altında Düzenle (veya ekleyin) bir ilke.</span><span class="sxs-lookup"><span data-stu-id="093f7-112">Under **Policies that apply to specific recipients**, edit (or add) a policy.</span></span>
    4. <span data-ttu-id="093f7-113">**Kuruluş içinde gönderilen iletilere uygula güvenli bağlantıları**seçin.</span><span class="sxs-lookup"><span data-stu-id="093f7-113">Select **Apply safe links to messages sent within the organization**.</span></span>
    5. <span data-ttu-id="093f7-114">İlkeniz kaydedin ve yaklaşık 30 dakika boyunca yaptığınız değişiklikler, datacenter üzerinden kendi şekilde çalışmanıza olanak sağlar.</span><span class="sxs-lookup"><span data-stu-id="093f7-114">Save your policy, and allow about 30 minutes for your changes to work their way through your datacenter.</span></span>
- <span data-ttu-id="093f7-115">ATP ile ilgili daha fazla yardım almak için bkz: [Office 365 Gelişmiş tehdit koruması](https://docs.microsoft.com/office365/securitycompliance/office-365-atp).</span><span class="sxs-lookup"><span data-stu-id="093f7-115">To get more help with ATP, see [Office 365 Advanced Threat Protection](https://docs.microsoft.com/office365/securitycompliance/office-365-atp).</span></span>