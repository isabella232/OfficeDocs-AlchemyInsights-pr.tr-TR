---
title: Intune iOS APNS sertifikasını ayarlama
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "3543"
ms.openlocfilehash: 66590b8a063e74e80bbe3e1e497c596d63a54ece
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51824059"
---
# <a name="intune-ios-set-up-apns-certificate"></a><span data-ttu-id="32cb2-102">Intune iOS APNS sertifikasını ayarlama</span><span class="sxs-lookup"><span data-stu-id="32cb2-102">Intune iOS set up APNS certificate</span></span>

<span data-ttu-id="32cb2-103">Aboneliğinizde Apple MDM Anında İletme sertifikası (Apple Anında İletilen Bildirim Hizmeti (APNS) sertifikası olarak da adlandırılır) yapılandırılmadı.</span><span class="sxs-lookup"><span data-stu-id="32cb2-103">An Apple MDM Push certificate (also known as an Apple Push Notification Service (APNS) certificate) has not been configured on your subscription.</span></span>

<span data-ttu-id="32cb2-104">Apple MDM Anında İletme sertifikası yapılandırılmadan iOS ve MacOS cihazlarına kaydolamaz ve bu cihazları yönetemezsiniz.</span><span class="sxs-lookup"><span data-stu-id="32cb2-104">Without an Apple MDM Push certificate configured, you'll be unable to enroll and manage iOS and MacOS devices.</span></span> <span data-ttu-id="32cb2-105">Sertifikayı Intune’a ekledikten sonra kullanıcılarınız iOS cihazlarını yönetmek için Şirket Portalı uygulamasını yükleyebilir.</span><span class="sxs-lookup"><span data-stu-id="32cb2-105">After you add the certificate to Intune, your users can install the Company Portal app to enroll their iOS devices.</span></span>

<span data-ttu-id="32cb2-106">Intune kiracılığınıza APNS sertifikası ekleme işleminin adım adım kılavuzu için aşağıdaki bağlantının içeriğini gözden geçirin:</span><span class="sxs-lookup"><span data-stu-id="32cb2-106">For a step-by-step guide to adding an APNS certificate to your Intune tenant, please review the content on the following link:</span></span>

- [<span data-ttu-id="32cb2-107">Apple MDM Anında İletme sertifikası alma</span><span class="sxs-lookup"><span data-stu-id="32cb2-107">Get an Apple MDM Push certificate</span></span>](https://docs.microsoft.com/mem/intune/enrollment/apple-mdm-push-certificate-get)

<span data-ttu-id="32cb2-108">Apple Anında İletilen Bildirim sertifikasıyla (APNs) ile sorun yaşıyorsanız şu blog gönderisine bakın: [Intune ve APNs sertifikası: SSS ve yaygın sorunlar](https://techcommunity.microsoft.com/t5/Intune-Customer-Success/Intune-and-the-APNs-certificate-FAQ-and-common-issues/ba-p/280121)</span><span class="sxs-lookup"><span data-stu-id="32cb2-108">If you are having issues with the Apple Push Notification certificate (APNs) refer to this blog post: [Intune and the APNs certificate: FAQ and common issues](https://techcommunity.microsoft.com/t5/Intune-Customer-Success/Intune-and-the-APNs-certificate-FAQ-and-common-issues/ba-p/280121)</span></span>
