---
title: SharePoint Online ile başlayın
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: 5e61491b626bfe75fd26a15ee54be82d9efa19a7
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/29/2019
ms.locfileid: "37766911"
---
# <a name="workflows-in-sharepoint"></a><span data-ttu-id="ae196-102">SharePoint'teki Iş Akışları</span><span class="sxs-lookup"><span data-stu-id="ae196-102">Workflows in SharePoint</span></span>

<span data-ttu-id="ae196-103">SharePoint iş akışları e-posta göndermiyorsa, kuruluşunuz Exchange Online gönderen sınırlarıyla karşılaşmış olabilir.</span><span class="sxs-lookup"><span data-stu-id="ae196-103">If SharePoint workflows are not sending emails, your organization may have encountered the Exchange Online sender limits.</span></span>

<span data-ttu-id="ae196-104">Aşağıdaki öğelerden birine sahipseniz ,'İş Akışı Askıya Alındı' hata iletisi oluşabilir:</span><span class="sxs-lookup"><span data-stu-id="ae196-104">The 'Workflow is Suspended' error message may occur if you have one of the following items:</span></span>

- <span data-ttu-id="ae196-105">SharePoint Online'da SharePoint 2010 veya SharePoint 2013 iş akışı platform türünü kullanan bir iş akışınız vardır.</span><span class="sxs-lookup"><span data-stu-id="ae196-105">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>

- <span data-ttu-id="ae196-106">İş akışı, aynı anda 200'den fazla kullanıcıya, günde 10.000'den fazla alıcıya veya dakikada 30'dan fazla iletigöndermek üzere özel bir e-posta iletisi gönderecek şekilde yapılandırılmıştır.</span><span class="sxs-lookup"><span data-stu-id="ae196-106">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>

<span data-ttu-id="ae196-107">İş akışını çalıştırdığınızda, e-posta iletisi gönderilmez ve hata iletisini fark edeyim, İç Durum Askıya Alınan veya alıcıya gönderilemiyor olarak ayarlanır görüntülenir.</span><span class="sxs-lookup"><span data-stu-id="ae196-107">When you run the workflow, the email message isn't sent, and you notice the error message, Internal Status is set to Suspended or Unable to send to a recipient is displayed.</span></span>

<span data-ttu-id="ae196-108">Daha fazla bilgi için lütfen aşağıdaki [makaleye](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running)bakın.</span><span class="sxs-lookup"><span data-stu-id="ae196-108">For more information, please refer to the following [article](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span></span>

