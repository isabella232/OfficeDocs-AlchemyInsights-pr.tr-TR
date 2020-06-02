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
ms.openlocfilehash: 8122b409a731a5fcc46c718aff1eeda07e26890b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506463"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="dd3d9-102">Hata kodu 5.7.23 için e-posta teslim sorunlarını düzeltme</span><span class="sxs-lookup"><span data-stu-id="dd3d9-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="dd3d9-103">Web'de herkese açık bir SPF veya DNS kayıt denetleyicisi olarak etki alanınız için SPF DNS kaydını doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="dd3d9-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="dd3d9-104">Giden iletinin Microsoft tarafından spam olarak tanımlanmadığını ve [Yüksek Riskli Teslim Havuzu'na](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages)yönlendirildiğini doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="dd3d9-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="dd3d9-105">Yüksek Riskli Teslim Havuzundaki iletiler SPF denetimlerini geçmez ve bu nedenle hedef e-posta kuruluşu tarafından kabul edilmez.</span><span class="sxs-lookup"><span data-stu-id="dd3d9-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="dd3d9-106">Sorun devam ederse, e-posta göndermeye çalıştığınız posta ana bilgisayar yöneticisiyle iletişime geçmeniz gerekebilir.</span><span class="sxs-lookup"><span data-stu-id="dd3d9-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="dd3d9-107">Geri dönen iletide bulunan ayrıntılı dış hataya dikkat edin.</span><span class="sxs-lookup"><span data-stu-id="dd3d9-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="dd3d9-108">Microsoft desteği daha fazla yardımcı olamayabilir.</span><span class="sxs-lookup"><span data-stu-id="dd3d9-108">Microsoft support may not be able to assist further.</span></span>
