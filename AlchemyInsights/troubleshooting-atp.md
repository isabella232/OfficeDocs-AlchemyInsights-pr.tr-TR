---
title: Windows için Microsoft Defender sorun giderme Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1039
ms.assetid: ''
ms.openlocfilehash: 91d73853d3ea67d6c6954fffb32dd1428e3d9976
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52545288"
---
# <a name="troubleshooting-microsoft-defender-for-office-365"></a><span data-ttu-id="97ca2-102">Windows için Microsoft Defender sorun giderme Office 365</span><span class="sxs-lookup"><span data-stu-id="97ca2-102">Troubleshooting Microsoft Defender for Office 365</span></span>

- <span data-ttu-id="97ca2-103">**İleti teslimi sırasında gecikme olduğunu fark ediyor musunuz?**</span><span class="sxs-lookup"><span data-stu-id="97ca2-103">**Do you notice delays in message delivery?**</span></span> <span data-ttu-id="97ca2-104">Ekler için [Microsoft Defender'da](/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) Dinamik Teslim Office 365 Kasa kullanın.</span><span class="sxs-lookup"><span data-stu-id="97ca2-104">Use the [Dynamic Delivery](/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) option in your Microsoft Defender for Office 365 Safe Attachments policy.</span></span> <span data-ttu-id="97ca2-105">Bu, alıcıları kötü amaçlı dosyalardan korurken ileti gecikmelerini önlemeye yardımcı olur.</span><span class="sxs-lookup"><span data-stu-id="97ca2-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="97ca2-106">**Hatalı pozitif veya yanlış negatifleri Microsoft'a bildirmeyi istiyor musunuz?**</span><span class="sxs-lookup"><span data-stu-id="97ca2-106">**Do you want to report false positives or false negatives to Microsoft?**</span></span> <span data-ttu-id="97ca2-107">Gönderiler [Gezgini'ni kullanın.](https://protection.office.com/reportsubmission)</span><span class="sxs-lookup"><span data-stu-id="97ca2-107">Use [Submissions Explorer](https://protection.office.com/reportsubmission).</span></span>

<span data-ttu-id="97ca2-108">-\*\* Kuruluş içindeki alıcılar arasında gönderilen iç e-Kasa için Bağlantılar korumasını etkinleştirebilirsiniz?\*\* Şu adımları izleyin:</span><span class="sxs-lookup"><span data-stu-id="97ca2-108">-\*\* Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?\*\* Follow these steps:</span></span>

  1. <span data-ttu-id="97ca2-109">Genel yönetici [https://protection.office.com](https://protection.office.com) veya güvenlik yöneticisi hesabıyla gidin ve oturum açın.</span><span class="sxs-lookup"><span data-stu-id="97ca2-109">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="97ca2-110">Tehdit yönetimi altındaki sol gezinti bölmesinde **İlke ve** **Bağlantılar'ı** \> **Kasa seçin.**</span><span class="sxs-lookup"><span data-stu-id="97ca2-110">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Links**.</span></span>

  3. <span data-ttu-id="97ca2-111">Kuruluşun **tamamına uygulanacak ilkeler bölümünde,** ilkeyi seçin ve Düzenle'ye **tıklayın.**</span><span class="sxs-lookup"><span data-stu-id="97ca2-111">In the **Policies that apply to the entire organization** section, select the policy and click **Edit**.</span></span>

  4. <span data-ttu-id="97ca2-112">Daha **Ayarlar** altında, **Kuruluş içinde gönderilen iletilere güvenli bağlantılar uygula 'ya tıklayın.**</span><span class="sxs-lookup"><span data-stu-id="97ca2-112">Under **Settings**, enable **Apply safe links to messages sent within the organization**.</span></span>
