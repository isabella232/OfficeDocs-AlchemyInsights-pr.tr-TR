---
title: Antispam-5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: ecbce4f0077dc9acab63575c19d40c0675a406ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717345"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="82e4c-102">Hata kodu 5.7.23 için e-posta teslim sorunlarını düzeltme</span><span class="sxs-lookup"><span data-stu-id="82e4c-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="82e4c-103">Web üzerinde genel kullanıma sunulan bir SPF veya DNS kayıt denetleyicisinde etki alanınızın SPF DNS kaydını doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="82e4c-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="82e4c-104">Giden iletinin Microsoft tarafından istenmeyen posta olarak tanımlandığını ve [yüksek riskli teslim havuzu](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages)aracılığıyla yönlendirildiğini doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="82e4c-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="82e4c-105">Yüksek riskli teslim havuzundaki mesajlar SPF denetimlerini geçirmez ve bu nedenle hedef e-posta organizasyonu tarafından kabul edilmez.</span><span class="sxs-lookup"><span data-stu-id="82e4c-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="82e4c-106">Sorun devam ederse, e-posta göndermeye çalıştığınız posta ana bilgisayarının yöneticisine başvurmanız gerekebilir.</span><span class="sxs-lookup"><span data-stu-id="82e4c-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="82e4c-107">Sıçrama iletisindeki ayrıntılı dış hata hatasını not alın.</span><span class="sxs-lookup"><span data-stu-id="82e4c-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="82e4c-108">Microsoft desteği daha fazla yardımcı olabilir.</span><span class="sxs-lookup"><span data-stu-id="82e4c-108">Microsoft support may not be able to assist further.</span></span>
