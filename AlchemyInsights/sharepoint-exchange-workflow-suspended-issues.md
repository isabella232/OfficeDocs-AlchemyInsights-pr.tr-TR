---
title: SharePoint Online ile çalışmaya başlama
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: bba89489cb75555e1f508224de223bee04e1d665
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700727"
---
# <a name="workflows-in-sharepoint"></a><span data-ttu-id="d8a80-102">SharePoint 'teki iş akışları</span><span class="sxs-lookup"><span data-stu-id="d8a80-102">Workflows in SharePoint</span></span>

<span data-ttu-id="d8a80-103">SharePoint iş akışları e-posta göndermiyor ise, kuruluşunuz Exchange Online gönderen limitleriyle karşılaşmış olabilir.</span><span class="sxs-lookup"><span data-stu-id="d8a80-103">If SharePoint workflows are not sending emails, your organization may have encountered the Exchange Online sender limits.</span></span>

<span data-ttu-id="d8a80-104">Aşağıdaki öğelerden birine sahipseniz ' Iş akışı askıya alındı ' hata iletisi görüntülenebilir:</span><span class="sxs-lookup"><span data-stu-id="d8a80-104">The 'Workflow is Suspended' error message may occur if you have one of the following items:</span></span>

- <span data-ttu-id="d8a80-105">SharePoint Online 'da SharePoint 2010 veya SharePoint 2013 Workflow Platform türünü kullanan bir iş akışınız var.</span><span class="sxs-lookup"><span data-stu-id="d8a80-105">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>

- <span data-ttu-id="d8a80-106">İş akışı, tek seferde 10.000 ' ten 200 fazla kullanıcıya veya dakikada 30 iletiden uzun bir e-posta iletisi gönderecek şekilde yapılandırılmıştır.</span><span class="sxs-lookup"><span data-stu-id="d8a80-106">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>

<span data-ttu-id="d8a80-107">İş akışını çalıştırdığınızda, e-posta iletisi gönderilmez ve hata iletisiyle karşılaşırsanız, dahili durumun askıya alınmış veya alıcıya gönderilemediği gösterilir.</span><span class="sxs-lookup"><span data-stu-id="d8a80-107">When you run the workflow, the email message isn't sent, and you notice the error message, Internal Status is set to Suspended or Unable to send to a recipient is displayed.</span></span>

<span data-ttu-id="d8a80-108">Daha fazla bilgi için lütfen aşağıdaki [makaleye](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running)bakın.</span><span class="sxs-lookup"><span data-stu-id="d8a80-108">For more information, please refer to the following [article](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span></span>

