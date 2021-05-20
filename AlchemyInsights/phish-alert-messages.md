---
title: 2491 'Kimlik Avı Kiracı veya kullanıcı geçersiz kılma nedeniyle teslim edildi' ilkesinden gelen e-posta iletilerini uyarı
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 2b373423cf3e63b76a62465dd62076c023580e94
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544598"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="a3908-102">'Kimlik Avı Kiracı veya kullanıcı geçersiz kılma nedeniyle teslim edildi' ilkesinden gelen e-posta iletilerini uyarı</span><span class="sxs-lookup"><span data-stu-id="a3908-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="a3908-103">Microsoft Defender'ın P1 ve P2 lisansları olan kiracılara "Kimlik Avı Kiracı veya kullanıcı geçersiz kılma nedeniyle teslim edildi" adlı varsayılan bir uyarı ilkesi Office 365 alınmış.</span><span class="sxs-lookup"><span data-stu-id="a3908-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Microsoft Defender for Office 365 P1 and P2 licenses.</span></span> <span data-ttu-id="a3908-104">Bu uyarıyı aldıysanız, şu adımları araştırabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="a3908-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="a3908-105">Uyarı iletisinde, **Uyarıyı Görüntüle'ye** **tıklar ve** Güvenlik ve Uyumluluk Merkezi'& gidin.</span><span class="sxs-lookup"><span data-stu-id="a3908-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="a3908-106">İleti listesini görüntüleme veya İletileri **Explorer'da görüntüleme seçeneğini** **görmek için uyarıyı seçin.**</span><span class="sxs-lookup"><span data-stu-id="a3908-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="a3908-107">Bu seçeneklerin her ikisi de sizi İleti Kimliğini içeren iletinin ayrıntılarına götürmektedir.</span><span class="sxs-lookup"><span data-stu-id="a3908-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="a3908-108">Tehdit Gezgini bağlantısı, uyarı ölçütlerine uyan iletileri otomatik olarak filtrelemektedir.</span><span class="sxs-lookup"><span data-stu-id="a3908-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="a3908-109">Threat Explorer'da tarih filtresini ayarlamanız gerekiyor olabilir.</span><span class="sxs-lookup"><span data-stu-id="a3908-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="a3908-110">Kimlik avı iletisi elle yapılandırılan geçersiz kılma nedeniyle teslim edildi:</span><span class="sxs-lookup"><span data-stu-id="a3908-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="a3908-111">Kullanıcı tarafından ayarlanmış izin verilen bir gönderen veya etki alanı.</span><span class="sxs-lookup"><span data-stu-id="a3908-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="a3908-112">İstenmeyen posta önleme ilkesinde yönetici tarafından ayarlanmış, izin verilen bir gönderen veya etki alanı.</span><span class="sxs-lookup"><span data-stu-id="a3908-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="a3908-113">Bağlantı filtresi ilkesinde izin verilen IP adresi.</span><span class="sxs-lookup"><span data-stu-id="a3908-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="a3908-114">İletilere izin verecek şekilde yapılandırılmış bir posta akışı kuralı (aktarım kuralı olarak da bilinir).</span><span class="sxs-lookup"><span data-stu-id="a3908-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="a3908-115">İletinin yanlışlıkla kimlik avı olarak işaretlenen bir ileti [](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) olduğunu inanıyorsanız, Microsoft'Outlook ileti örnekleri göndermek için Rapor İletisi eklentinizi kullanın.</span><span class="sxs-lookup"><span data-stu-id="a3908-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
