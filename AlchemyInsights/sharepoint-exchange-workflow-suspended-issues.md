---
title: SharePoint Online uygulamasını kullanmaya başlama
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: afb1ef115d364ee3e2cf09ea850adb57ad1d44e6
ms.sourcegitcommit: 136b8209c52c2a05d0f2fdaab93b2cd92253fa2c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34770582"
---
# <a name="workflows-in-sharepoint"></a><span data-ttu-id="0f27d-102">SharePoint iş akışları</span><span class="sxs-lookup"><span data-stu-id="0f27d-102">Workflows in SharePoint</span></span>

<span data-ttu-id="0f27d-103">SharePoint iş akışları e-postalar göndermek değil, kuruluşunuzda Exchange Online gönderen sınırları karşılaşmış olabilir.</span><span class="sxs-lookup"><span data-stu-id="0f27d-103">If SharePoint workflows are not sending emails, your organization may have encountered the Exchange Online sender limits.</span></span>

<span data-ttu-id="0f27d-104">Aşağıdaki öğelerden birini kullanıyorsanız, 'İş akışı askıya' hata iletisi ortaya çıkabilir:</span><span class="sxs-lookup"><span data-stu-id="0f27d-104">'Workflow is Suspended' error message may occur if you have one of the following items:</span></span>

- <span data-ttu-id="0f27d-105">Bir iş akışı SharePoint 2010 SharePoint veya SharePoint 2013 iş akışı platform türü kullanan çevrimiçi olarak vardır.</span><span class="sxs-lookup"><span data-stu-id="0f27d-105">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>

- <span data-ttu-id="0f27d-106">İş akışı, bir saat, günde 10. 000'den fazla alıcı veya dakika başına 30'dan fazla ileti 200'den fazla kullanıcılara özel e-posta iletisi göndermek için yapılandırılır.</span><span class="sxs-lookup"><span data-stu-id="0f27d-106">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>

<span data-ttu-id="0f27d-107">İş akışını çalıştırmak, e-posta iletisi gönderilmez ve hata iletisini görürsünüz, iç durumu ayarlanır Beklemede veya Unable bir alıcıya göndermek için görüntülenir.</span><span class="sxs-lookup"><span data-stu-id="0f27d-107">When you run the workflow, the email message isn't sent, and you notice the error message, Internal Status is set to Suspended or Unable to send to a recipient is displayed.</span></span>

<span data-ttu-id="0f27d-108">Daha fazla bilgi için lütfen aşağıdaki [makaleye](https://support.office.com/article/-daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or-unable-to-send-to-a-recipient-error-in-a-sharepoint-online-workflow-89d02169-5fa6-4259-affc-73edb6ca9fb6?ui=en-US&amp;rs=en-US&amp;ad=US)bakın.</span><span class="sxs-lookup"><span data-stu-id="0f27d-108">For more information, please refer to the following [article](https://support.office.com/article/-daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or-unable-to-send-to-a-recipient-error-in-a-sharepoint-online-workflow-89d02169-5fa6-4259-affc-73edb6ca9fb6?ui=en-US&amp;rs=en-US&amp;ad=US).</span></span>

