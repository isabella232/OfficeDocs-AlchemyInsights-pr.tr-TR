---
title: Sorun Giderme Office 365 Gelişmiş Tehdit Koruması
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1039
ms.assetid: ''
ms.openlocfilehash: 7391b3c126d55213881f6b71cb6b5fc72bc68d0f
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44512610"
---
# <a name="troubleshooting-office-365-advanced-threat-protection"></a><span data-ttu-id="af196-102">Sorun Giderme Office 365 Gelişmiş Tehdit Koruması</span><span class="sxs-lookup"><span data-stu-id="af196-102">Troubleshooting Office 365 Advanced Threat Protection</span></span>

- <span data-ttu-id="af196-103">İleti iletisindeki gecikmeleri fark ediyor musunuz?</span><span class="sxs-lookup"><span data-stu-id="af196-103">Do you notice delays in message delivery?</span></span> <span data-ttu-id="af196-104">ATP Güvenli Ekler ipolitikasında [Dinamik Teslim](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) seçeneğini kullanın.</span><span class="sxs-lookup"><span data-stu-id="af196-104">Use the [Dynamic Delivery](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) option in your ATP Safe Attachments policy.</span></span> <span data-ttu-id="af196-105">Bu, alıcıları kötü amaçlı dosyalardan korurken ileti gecikmelerini önlemeye yardımcı olur.</span><span class="sxs-lookup"><span data-stu-id="af196-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="af196-106">Microsoft'a yanlış pozitif veya yanlış negatifleri bildirmek istiyor musunuz?</span><span class="sxs-lookup"><span data-stu-id="af196-106">Do you want to report false positives or false negatives to Microsoft?</span></span> <span data-ttu-id="af196-107">Çözümleme için dosya göndermek için bu [bağlantıyı](https://www.microsoft.com/wdsi/filesubmission/) kullanın.</span><span class="sxs-lookup"><span data-stu-id="af196-107">Use this [link](https://www.microsoft.com/wdsi/filesubmission/) to submit files for analysis.</span></span>

- <span data-ttu-id="af196-108">Kuruluşunuzdaki alıcılar arasında gönderilen dahili e-postalar için Güvenli Bağlantılar korumasını etkinleştirebileceğinizi biliyor muydunuz?</span><span class="sxs-lookup"><span data-stu-id="af196-108">Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?</span></span> <span data-ttu-id="af196-109">Şu adımları izleyin:</span><span class="sxs-lookup"><span data-stu-id="af196-109">Follow these steps:</span></span>

  1. <span data-ttu-id="af196-110">Genel [https://protection.office.com](https://protection.office.com) bir yönetici veya güvenlik yöneticisi hesabıyla oturum açın ve oturum açın.</span><span class="sxs-lookup"><span data-stu-id="af196-110">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="af196-111">**Tehdit yönetimi**altında sol navigasyon bölmesinde, **İlke** \> **Güvenli Bağlantılar**seçin.</span><span class="sxs-lookup"><span data-stu-id="af196-111">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Links**.</span></span>

  3. <span data-ttu-id="af196-112">Tüm **kuruluş bölümüne uygulanan** İlkeler'de, ilkeyi seçin ve **Edit'i**tıklatın.</span><span class="sxs-lookup"><span data-stu-id="af196-112">In the **Policies that apply to the entire organization** section, select the policy and click **Edit**.</span></span>

  4. <span data-ttu-id="af196-113">**Ayarlar**altında, **kuruluş içinde gönderilen iletilere güvenli bağlantılar uygulayın'ı etkinleştirin.**</span><span class="sxs-lookup"><span data-stu-id="af196-113">Under **Settings**, enable **Apply safe links to messages sent within the organization**.</span></span>
