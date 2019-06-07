---
title: Office 365 Gelişmiş tehdit koruması sorunlarını giderme
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1039
ms.assetid: ''
ms.openlocfilehash: b4358fb55a1145833510c6063b520d822f2d1eaf
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765515"
---
# <a name="troubleshooting-office-365-advanced-threat-protection"></a><span data-ttu-id="399f1-102">Office 365 Gelişmiş tehdit koruması sorunlarını giderme</span><span class="sxs-lookup"><span data-stu-id="399f1-102">Troubleshooting Office 365 Advanced Threat Protection</span></span>

- <span data-ttu-id="399f1-103">İleti teslimi gecikme fark?</span><span class="sxs-lookup"><span data-stu-id="399f1-103">Do you notice delays in message delivery?</span></span> <span data-ttu-id="399f1-104">ATP güvenli ekler ilkenizde [Dinamik teslim](https://docs.microsoft.com/office365/securitycompliance/dynamic-delivery-and-previewing) seçeneğini kullanın.</span><span class="sxs-lookup"><span data-stu-id="399f1-104">Use the [Dynamic Delivery](https://docs.microsoft.com/office365/securitycompliance/dynamic-delivery-and-previewing) option in your ATP Safe Attachments policy.</span></span> <span data-ttu-id="399f1-105">Bu kötü amaçlı dosyaları alıcılar korurken ileti gecikmeleri önlemek yardımcı olur.</span><span class="sxs-lookup"><span data-stu-id="399f1-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="399f1-106">Yanlış pozitif veya yanlış negatif Microsoft'a bildirmek istiyor musunuz?</span><span class="sxs-lookup"><span data-stu-id="399f1-106">Do you want to report false positives or false negatives to Microsoft?</span></span> <span data-ttu-id="399f1-107">Çözümleme için dosyaları göndermek için bu [bağlantıyı](https://www.microsoft.com/wdsi/filesubmission/) kullanın.</span><span class="sxs-lookup"><span data-stu-id="399f1-107">Use this [link](https://www.microsoft.com/wdsi/filesubmission/) to submit files for analysis.</span></span>

- <span data-ttu-id="399f1-108">Kuruluşunuz içindeki alıcılar arasında gönderilen iç e-posta için güvenli bağlantılar korumasını etkinleştirebilirsiniz biliyor muydunuz?</span><span class="sxs-lookup"><span data-stu-id="399f1-108">Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?</span></span> <span data-ttu-id="399f1-109">İzleyeceğiniz adımlar:</span><span class="sxs-lookup"><span data-stu-id="399f1-109">Follow these steps:</span></span>

  1. <span data-ttu-id="399f1-110">Git [https://protection.office.com](https://protection.office.com) ve genel yönetici veya güvenlik yöneticisi hesabı ile oturum açın.</span><span class="sxs-lookup"><span data-stu-id="399f1-110">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="399f1-111">**İlke** **tehdit Yönetimi**altında sol gezinti bölmesinde seçin \> **Güvenli bağlantılar**.</span><span class="sxs-lookup"><span data-stu-id="399f1-111">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Links**.</span></span>

  3. <span data-ttu-id="399f1-112">**Kuruluşun tamamı için geçerli ilkeleri** bölümünde, ilkeyi seçin ve **Düzenle**' yi tıklatın.</span><span class="sxs-lookup"><span data-stu-id="399f1-112">In the **Policies that apply to the entire organization** section, select the policy and click **Edit**.</span></span>

  4. <span data-ttu-id="399f1-113">**Ayarlar**altında **kuruluş içinde gönderilen iletilere uygula güvenli bağlantıları**etkinleştirin.</span><span class="sxs-lookup"><span data-stu-id="399f1-113">Under **Settings**, enable **Apply safe links to messages sent within the organization**.</span></span>
