---
title: "'Override' kimlik avı teslim Kiracı veya kullanıcı ilkesi 2491 uyarı e-posta iletileri"
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 456b186ecea59422c791c79d4df056ad8446bc70
ms.sourcegitcommit: 7c90dcc570d32ebd968e3e4e816a7b482890b3a4
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36391596"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="4ca2e-102">'Override' kimlik avı teslim Kiracı veya kullanıcı ilkesi gelen uyarı e-posta iletileri</span><span class="sxs-lookup"><span data-stu-id="4ca2e-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="4ca2e-103">"Kiracı veya kullanıcı geçersiz kılma nedeniyle kimlik avı teslim edildi" adlı varsayılan bir uyarı ilke Office 365 KM P1 ve P2 lisansların kiracılar için alındı.</span><span class="sxs-lookup"><span data-stu-id="4ca2e-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Office 365 ATP P1 and P2 licenses.</span></span> <span data-ttu-id="4ca2e-104">Bu uyarı aldıysanız, araştırmak için adımlar şunlardır:</span><span class="sxs-lookup"><span data-stu-id="4ca2e-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="4ca2e-105">Uyarı iletisinden Uyumluluk Merkezi güvenlik & **Uyarıları** sayfasına gitmek için **Uyarı görüntüle** ' yi tıklatın.</span><span class="sxs-lookup"><span data-stu-id="4ca2e-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="4ca2e-106">Uyarı **ileti listesini görüntüle** veya **Explorer iletileri görüntüleme**seçeneği görmek için seçin.</span><span class="sxs-lookup"><span data-stu-id="4ca2e-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="4ca2e-107">Bu seçeneklerin her ikisi için ileti kimliği içeren ileti ayrıntılarını ele</span><span class="sxs-lookup"><span data-stu-id="4ca2e-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="4ca2e-108">Tehdit Explorer bağlantıyı otomatik olarak uyarı ölçütüne uyan iletileri süzer unutmayın.</span><span class="sxs-lookup"><span data-stu-id="4ca2e-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="4ca2e-109">Tarih Filtresi alanında tehdit Explorer ayarlamanız gerekebilir.</span><span class="sxs-lookup"><span data-stu-id="4ca2e-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="4ca2e-110">Kimlik avı iletisi nedeniyle el ile yapılandırılmış bir geçersiz kılma teslim edildi:</span><span class="sxs-lookup"><span data-stu-id="4ca2e-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="4ca2e-111">İzin verilen gönderen veya etki alanı kullanıcı tarafından ayarlanan.</span><span class="sxs-lookup"><span data-stu-id="4ca2e-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="4ca2e-112">İzin verilen gönderenin veya istenmeyen posta önleme İlkesi'nde yönetici tarafından ayarlanan etki alanı.</span><span class="sxs-lookup"><span data-stu-id="4ca2e-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="4ca2e-113">Bağlantı filtresi ilkesine izin verilen IP adresi.</span><span class="sxs-lookup"><span data-stu-id="4ca2e-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="4ca2e-114">İletilere izin vermek için yapılandırılmış bir posta akışı kuralı (aktarım kuralı olarak da bilinir).</span><span class="sxs-lookup"><span data-stu-id="4ca2e-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="4ca2e-115">İleti yanlış kimlik avı işaretlendi düşünüyorsanız, Outlook [raporu iletisi eklentisi](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) ileti örnekleri Microsoft'a göndermek için kullanın.</span><span class="sxs-lookup"><span data-stu-id="4ca2e-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
