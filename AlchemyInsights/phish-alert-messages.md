---
title: 2491 ' Kiracı veya Kullanıcı geçersiz kıldığı için e-posta iletilerini '
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
ms.openlocfilehash: 5b5faa08542cb5878107f10afb34427f636562ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47728631"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="bd8b0-102">E-posta iletilerini, kiracı veya Kullanıcı geçersiz kıldığı için</span><span class="sxs-lookup"><span data-stu-id="bd8b0-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="bd8b0-103">Office 365 ATP P1 ve P2 lisansları ile "Kiracı veya Kullanıcı geçersiz kılma nedeniyle teslim edildi</span><span class="sxs-lookup"><span data-stu-id="bd8b0-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Office 365 ATP P1 and P2 licenses.</span></span> <span data-ttu-id="bd8b0-104">Bu uyarıyı aldıysanız, şu adımları araştırmalısınız:</span><span class="sxs-lookup"><span data-stu-id="bd8b0-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="bd8b0-105">Uyarı iletisinden, güvenlik & Uyumluluk Merkezi 'ndeki **Uyarılar** sayfasına gitmek Için **uyarıyı görüntüle** 'ye tıklayın.</span><span class="sxs-lookup"><span data-stu-id="bd8b0-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="bd8b0-106">**İleti listesini görüntüleme** veya **Explorer 'da iletileri görüntüleme**seçeneğini görmek için uyarıyı seçin.</span><span class="sxs-lookup"><span data-stu-id="bd8b0-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="bd8b0-107">Bu seçeneklerin her ikisi de ileti KIMLIĞINI içeren iletinin ayrıntılarına götürür.</span><span class="sxs-lookup"><span data-stu-id="bd8b0-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="bd8b0-108">Tehdit Gezgini bağlantısının uyarı ölçütleriyle eşleşen iletilere otomatik olarak filtrelendirilecektir.</span><span class="sxs-lookup"><span data-stu-id="bd8b0-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="bd8b0-109">Tehdit Gezginindeki Tarih filtresini ayarlamanız gerekebilir.</span><span class="sxs-lookup"><span data-stu-id="bd8b0-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="bd8b0-110">El ile yapılandırılmış bir geçersiz kılma nedeniyle kimlik avı iletisi teslim edildi:</span><span class="sxs-lookup"><span data-stu-id="bd8b0-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="bd8b0-111">Kullanıcının verdiği bir göndereni veya etki alanı.</span><span class="sxs-lookup"><span data-stu-id="bd8b0-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="bd8b0-112">Yönetici tarafından istenmeyen posta önleme ilkesinde ayarlanan bir kişi veya etki alanı.</span><span class="sxs-lookup"><span data-stu-id="bd8b0-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="bd8b0-113">Bağlantı filtresi ilkesinde izin verilen bir IP adresi.</span><span class="sxs-lookup"><span data-stu-id="bd8b0-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="bd8b0-114">Uygulamasında iletilere izin verecek şekilde yapılandırılmış bir posta akış kuralı (taşıma kuralı olarak da bilinir).</span><span class="sxs-lookup"><span data-stu-id="bd8b0-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="bd8b0-115">İletinin yanlış şekilde bir şekilde işaretlendiğini düşünüyorsanız, ileti örneklerini Microsoft 'a göndermek için Outlook [rapor iletisi eklentisini](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) kullanın.</span><span class="sxs-lookup"><span data-stu-id="bd8b0-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
