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
ms.openlocfilehash: 9c9bc2d04fb8efaa5e75194b4ca09316d24e018e
ms.sourcegitcommit: 07b47d7f3ca191363e6bc84140e8e01524d6f08e
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/24/2019
ms.locfileid: "37682336"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="381f8-102">Hata kodu 5.7.23 için e-posta teslim sorunlarını düzeltme</span><span class="sxs-lookup"><span data-stu-id="381f8-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="381f8-103">Web'de herkese açık bir SPF veya DNS kayıt denetleyicisi olarak etki alanınız için SPF DNS kaydını doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="381f8-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="381f8-104">Giden iletinin Office 365 tarafından spam olarak tanımlanmadığını ve [Yüksek Riskli Teslim Havuzu'ndan](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages)yönlendirildiğini doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="381f8-104">Verify that the outbound message wasn't identified as spam by Office 365 and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="381f8-105">Yüksek Riskli Teslim Havuzundaki iletiler SPF denetimlerini geçmez ve bu nedenle hedef e-posta kuruluşu tarafından kabul edilmez.</span><span class="sxs-lookup"><span data-stu-id="381f8-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="381f8-106">Sorun devam ederse, e-posta göndermeye çalıştığınız posta ana bilgisayar yöneticisiyle iletişime geçmeniz gerekebilir.</span><span class="sxs-lookup"><span data-stu-id="381f8-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="381f8-107">Geri dönen iletide bulunan ayrıntılı dış hataya dikkat edin.</span><span class="sxs-lookup"><span data-stu-id="381f8-107">Make note of the detailed external error available in the bounce message.</span></span>  <span data-ttu-id="381f8-108">Office 365 desteği daha fazla yardımcı olamayabilir.</span><span class="sxs-lookup"><span data-stu-id="381f8-108">Office 365 support may not be able to assist further.</span></span>