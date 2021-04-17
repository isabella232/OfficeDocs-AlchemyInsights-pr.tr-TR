---
title: Antispam - 5.7.23
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: e494e8017f24d65a94d1a7490be4d67c46a2120b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821431"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="0e094-102">Hata kodu 5.7.23 için e-posta teslim sorunlarını düzeltme</span><span class="sxs-lookup"><span data-stu-id="0e094-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="0e094-103">Web'de genel kullanıma açık bir SPF veya DNS kayıt denetleyicisinde etki alanınız için SPF DNS kaydını doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="0e094-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="0e094-104">Giden iletinin Microsoft tarafından istenmeyen posta olarak tanım olmadığını ve Yüksek Riskli Teslim Havuzu aracılığıyla [yönlendirildi doğrulayın.](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages)</span><span class="sxs-lookup"><span data-stu-id="0e094-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="0e094-105">Yüksek Riskli Teslim Havuzu'daki iletiler SPF denetimlerinden geçirilecek ve bu nedenle hedef e-posta kuruluşu tarafından kabul edilmayacak.</span><span class="sxs-lookup"><span data-stu-id="0e094-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="0e094-106">Sorun devam ederse, e-posta göndermeye çalıştığınız posta ana bilgisayarının yöneticisine başvurabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="0e094-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="0e094-107">Geri dönen iletide kullanılabilen ayrıntılı dış hatayı not alabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="0e094-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="0e094-108">Microsoft desteği daha fazla yardımcı olabilir.</span><span class="sxs-lookup"><span data-stu-id="0e094-108">Microsoft support may not be able to assist further.</span></span>
