---
title: 2491 'Kiracı veya kullanıcı geçersiz kılma nedeniyle teslim edilen Kimlik Avı' ilkesinden uyarı e-posta iletileri
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 2e4efd504304da757687e697ff23374aeea31851
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758954"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="5a18b-102">'Kiracı veya kullanıcı geçersiz kılma nedeniyle teslim edilen Kimlik Avı' ilkesinden gelen e-posta iletilerini uyar</span><span class="sxs-lookup"><span data-stu-id="5a18b-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="5a18b-103">Office 365 ATP P1 ve P2 lisanslarına sahip kiracılara "Kiracı veya kullanıcı geçersiz kılma nedeniyle Kimlik Avı Teslim" adlı varsayılan uyarı ilkesi kullanıma sunuldu.</span><span class="sxs-lookup"><span data-stu-id="5a18b-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Office 365 ATP P1 and P2 licenses.</span></span> <span data-ttu-id="5a18b-104">Bu uyarıyı aldıysanız, araştırılabilmek için adımlar şunlardır:</span><span class="sxs-lookup"><span data-stu-id="5a18b-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="5a18b-105">Uyarı iletisinden, Güvenlik & Uyumluluk Merkezi'ndeki **Uyarılar** sayfasına gitmek için **Uyarıyı** Görüntüle'yi tıklatın.</span><span class="sxs-lookup"><span data-stu-id="5a18b-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="5a18b-106">**İleti listesini** görüntüleme veya **Explorer'da iletileri görüntüleme**seçeneğini görmek için uyarıyı seçin.</span><span class="sxs-lookup"><span data-stu-id="5a18b-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="5a18b-107">Bu seçeneklerin her ikisi de sizi İleti Kimliği'ni içeren iletinin ayrıntılarına götürür.</span><span class="sxs-lookup"><span data-stu-id="5a18b-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="5a18b-108">Tehdit Gezgini bağlantısının uyarı ölçütlerine uyan iletilere otomatik olarak filtre uygulayacağını unutmayın.</span><span class="sxs-lookup"><span data-stu-id="5a18b-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="5a18b-109">Tehdit Gezgini'ndeki tarih filtresini ayarlamanız gerekebilir.</span><span class="sxs-lookup"><span data-stu-id="5a18b-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="5a18b-110">Kimlik avı iletisi, el ile yapılandırılan geçersiz kılma nedeniyle teslim edildi:</span><span class="sxs-lookup"><span data-stu-id="5a18b-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="5a18b-111">Kullanıcı tarafından ayarlanan izin verilen bir gönderen veya etki alanı.</span><span class="sxs-lookup"><span data-stu-id="5a18b-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="5a18b-112">İstenmeyen bir politikada yönetici tarafından ayarlanan izin verilen bir gönderen veya etki alanı.</span><span class="sxs-lookup"><span data-stu-id="5a18b-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="5a18b-113">Bağlantı filtresi ilkesinde izin verilen bir IP adresi.</span><span class="sxs-lookup"><span data-stu-id="5a18b-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="5a18b-114">İletilerin girmesine izin verecek şekilde yapılandırılan bir posta akışı kuralı (aktarım kuralı olarak da bilinir).</span><span class="sxs-lookup"><span data-stu-id="5a18b-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="5a18b-115">İletinin kimlik avı olarak yanlış olarak işaretlendiğini düşünüyorsanız, Microsoft'a ileti örnekleri göndermek için Outlook [Rapor İletisi eklentisini](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) kullanın.</span><span class="sxs-lookup"><span data-stu-id="5a18b-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
