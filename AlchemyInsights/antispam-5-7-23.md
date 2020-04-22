---
title: Antispam - 5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: 307b738c40c620d057e68eff7d218c8c9b5eb665
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43676517"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="31e57-102">Hata kodu 5.7.23 için e-posta teslim sorunlarını düzeltme</span><span class="sxs-lookup"><span data-stu-id="31e57-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="31e57-103">Web'de herkese açık bir SPF veya DNS kayıt denetleyicisi olarak etki alanınız için SPF DNS kaydını doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="31e57-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="31e57-104">Giden iletinin Microsoft tarafından spam olarak tanımlanmadığını ve [Yüksek Riskli Teslim Havuzu'na](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages)yönlendirildiğini doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="31e57-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="31e57-105">Yüksek Riskli Teslim Havuzundaki iletiler SPF denetimlerini geçmez ve bu nedenle hedef e-posta kuruluşu tarafından kabul edilmez.</span><span class="sxs-lookup"><span data-stu-id="31e57-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="31e57-106">Sorun devam ederse, e-posta göndermeye çalıştığınız posta ana bilgisayar yöneticisiyle iletişime geçmeniz gerekebilir.</span><span class="sxs-lookup"><span data-stu-id="31e57-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="31e57-107">Geri dönen iletide bulunan ayrıntılı dış hataya dikkat edin.</span><span class="sxs-lookup"><span data-stu-id="31e57-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="31e57-108">Microsoft desteği daha fazla yardımcı olamayabilir.</span><span class="sxs-lookup"><span data-stu-id="31e57-108">Microsoft support may not be able to assist further.</span></span>
