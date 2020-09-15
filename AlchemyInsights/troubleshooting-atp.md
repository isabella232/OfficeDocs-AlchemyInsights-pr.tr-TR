---
title: Office 365 Gelişmiş tehdit koruması sorunlarını giderme
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
ms.openlocfilehash: 5a13653ba08d8c6b822354ff70f6d276d31cd816
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658934"
---
# <a name="troubleshooting-office-365-advanced-threat-protection"></a><span data-ttu-id="7b643-102">Office 365 Gelişmiş tehdit koruması sorunlarını giderme</span><span class="sxs-lookup"><span data-stu-id="7b643-102">Troubleshooting Office 365 Advanced Threat Protection</span></span>

- <span data-ttu-id="7b643-103">İleti tesliminde gecikmeler fark ediyor musunuz?</span><span class="sxs-lookup"><span data-stu-id="7b643-103">Do you notice delays in message delivery?</span></span> <span data-ttu-id="7b643-104">ATP güvenli ekler ilkemizin ilkesindeki [dinamik teslim](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) seçeneğini kullanın.</span><span class="sxs-lookup"><span data-stu-id="7b643-104">Use the [Dynamic Delivery](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) option in your ATP Safe Attachments policy.</span></span> <span data-ttu-id="7b643-105">Bu, alıcıları kötü niyetli dosyalardan korurken ileti gecikmelerinden korunmanıza yardımcı olur.</span><span class="sxs-lookup"><span data-stu-id="7b643-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="7b643-106">Yanlış pozitif durumları veya yanlış negatifleri Microsoft 'a bildirmek mı istiyorsunuz?</span><span class="sxs-lookup"><span data-stu-id="7b643-106">Do you want to report false positives or false negatives to Microsoft?</span></span> <span data-ttu-id="7b643-107">Dosyaları Analize göndermek için bu [bağlantıyı](https://www.microsoft.com/wdsi/filesubmission/) kullanın.</span><span class="sxs-lookup"><span data-stu-id="7b643-107">Use this [link](https://www.microsoft.com/wdsi/filesubmission/) to submit files for analysis.</span></span>

- <span data-ttu-id="7b643-108">Kuruluşunuzdaki alıcılar arasında gönderilen iç e-posta için güvenli bağlantılar korumasını etkinleştirebileceğiniz biliyor muydunuz?</span><span class="sxs-lookup"><span data-stu-id="7b643-108">Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?</span></span> <span data-ttu-id="7b643-109">Şu adımları izleyin:</span><span class="sxs-lookup"><span data-stu-id="7b643-109">Follow these steps:</span></span>

  1. <span data-ttu-id="7b643-110">[https://protection.office.com](https://protection.office.com)Genel yönetici veya güvenlik yöneticisi hesabıyla gidin ve oturum açın.</span><span class="sxs-lookup"><span data-stu-id="7b643-110">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="7b643-111">Gezinti bölmesinde **tehdit yönetimi**'nin altında **ilkeye** göre \> **güvenli bağlantılar**'ı seçin.</span><span class="sxs-lookup"><span data-stu-id="7b643-111">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Links**.</span></span>

  3. <span data-ttu-id="7b643-112">**Tüm kuruluş bölümü için geçerli olan ilkelerde** ilkeyi seçin ve **Düzenle**'ye tıklayın.</span><span class="sxs-lookup"><span data-stu-id="7b643-112">In the **Policies that apply to the entire organization** section, select the policy and click **Edit**.</span></span>

  4. <span data-ttu-id="7b643-113">**Ayarlar**'ın altında, **kuruluş içinde gönderilen Iletilere güvenli bağlantılar uygulayın**.</span><span class="sxs-lookup"><span data-stu-id="7b643-113">Under **Settings**, enable **Apply safe links to messages sent within the organization**.</span></span>
