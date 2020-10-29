---
title: Office 365 için Microsoft Defender sorunlarını giderme
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
ms.openlocfilehash: 2c9543660056ebc02b0bd297f619f20fa6820093
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801466"
---
# <a name="troubleshooting-microsoft-defender-for-office-365"></a><span data-ttu-id="3951e-102">Office 365 için Microsoft Defender sorunlarını giderme</span><span class="sxs-lookup"><span data-stu-id="3951e-102">Troubleshooting Microsoft Defender for Office 365</span></span>

- <span data-ttu-id="3951e-103">İleti tesliminde gecikmeler fark ediyor musunuz?</span><span class="sxs-lookup"><span data-stu-id="3951e-103">Do you notice delays in message delivery?</span></span> <span data-ttu-id="3951e-104">ATP güvenli ekler ilkemizin ilkesindeki [dinamik teslim](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) seçeneğini kullanın.</span><span class="sxs-lookup"><span data-stu-id="3951e-104">Use the [Dynamic Delivery](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) option in your ATP Safe Attachments policy.</span></span> <span data-ttu-id="3951e-105">Bu, alıcıları kötü niyetli dosyalardan korurken ileti gecikmelerinden korunmanıza yardımcı olur.</span><span class="sxs-lookup"><span data-stu-id="3951e-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="3951e-106">Yanlış pozitif durumları veya yanlış negatifleri Microsoft 'a bildirmek mı istiyorsunuz?</span><span class="sxs-lookup"><span data-stu-id="3951e-106">Do you want to report false positives or false negatives to Microsoft?</span></span> <span data-ttu-id="3951e-107">Dosyaları Analize göndermek için bu [bağlantıyı](https://www.microsoft.com/wdsi/filesubmission/) kullanın.</span><span class="sxs-lookup"><span data-stu-id="3951e-107">Use this [link](https://www.microsoft.com/wdsi/filesubmission/) to submit files for analysis.</span></span>

- <span data-ttu-id="3951e-108">Kuruluşunuzdaki alıcılar arasında gönderilen iç e-posta için güvenli bağlantılar korumasını etkinleştirebileceğiniz biliyor muydunuz?</span><span class="sxs-lookup"><span data-stu-id="3951e-108">Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?</span></span> <span data-ttu-id="3951e-109">Şu adımları izleyin:</span><span class="sxs-lookup"><span data-stu-id="3951e-109">Follow these steps:</span></span>

  1. <span data-ttu-id="3951e-110">[https://protection.office.com](https://protection.office.com)Genel yönetici veya güvenlik yöneticisi hesabıyla gidin ve oturum açın.</span><span class="sxs-lookup"><span data-stu-id="3951e-110">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="3951e-111">Gezinti bölmesinde **tehdit yönetimi** 'nin altında **ilkeye** göre \> **güvenli bağlantılar** 'ı seçin.</span><span class="sxs-lookup"><span data-stu-id="3951e-111">In the left navigation pane under **Threat management** , choose **Policy** \> **Safe Links** .</span></span>

  3. <span data-ttu-id="3951e-112">**Tüm kuruluş bölümü için geçerli olan ilkelerde** ilkeyi seçin ve **Düzenle** 'ye tıklayın.</span><span class="sxs-lookup"><span data-stu-id="3951e-112">In the **Policies that apply to the entire organization** section, select the policy and click **Edit** .</span></span>

  4. <span data-ttu-id="3951e-113">**Ayarlar** 'ın altında, **kuruluş içinde gönderilen Iletilere güvenli bağlantılar uygulayın** .</span><span class="sxs-lookup"><span data-stu-id="3951e-113">Under **Settings** , enable **Apply safe links to messages sent within the organization** .</span></span>
