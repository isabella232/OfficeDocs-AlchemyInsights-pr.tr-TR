---
title: Günlük e-posta sınırı aşıldı. İş akışı askıya alınır.
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 802aba696da61be5f0a6c12072842cbc3cd96499
ms.sourcegitcommit: 407f6c1e82f1a0be5cf53301fbf03cd25dcbf0ee
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/02/2019
ms.locfileid: "36059658"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="c3577-103">Günlük e-posta sınırı aştı.</span><span class="sxs-lookup"><span data-stu-id="c3577-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="c3577-104">İş akışı askıya alınır.</span><span class="sxs-lookup"><span data-stu-id="c3577-104">Workflow is suspended.</span></span>

<span data-ttu-id="c3577-105">Bu hata aşağıdaki senaryolarda alınan:</span><span class="sxs-lookup"><span data-stu-id="c3577-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="c3577-106">Bir iş akışı SharePoint 2010 SharePoint veya SharePoint 2013 iş akışı platform türü kullanan çevrimiçi olarak vardır.</span><span class="sxs-lookup"><span data-stu-id="c3577-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="c3577-107">İş akışı, bir saat, günde 10. 000'den fazla alıcı veya dakika başına 30'dan fazla ileti 200'den fazla kullanıcılara özel e-posta iletisi göndermek için yapılandırılır.</span><span class="sxs-lookup"><span data-stu-id="c3577-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="c3577-108">İş akışı çalıştırdığınızda, e-posta iletisi gönderilmez ve aşağıdaki davranışla karşılaşırsınız:</span><span class="sxs-lookup"><span data-stu-id="c3577-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="c3577-109">SharePoint 2013 platform türünü kullanarak iş akışı, **İş akışı durumu** sayfasına gidin.</span><span class="sxs-lookup"><span data-stu-id="c3577-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="c3577-110">İş akışı durumu sayfasında **İç durumu** **başlatıldı**olarak ayarlanır ve **alıcıya gönderilemiyor**bilgi balonu görüntüler.</span><span class="sxs-lookup"><span data-stu-id="c3577-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="c3577-111">Bu soruna geçici bir çözüm için [gönderen Exchange Online sınırları](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits)aşmadan e-posta iletileri göndermek için iş akışı yapılandırın.</span><span class="sxs-lookup"><span data-stu-id="c3577-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="c3577-112">Örneğin, iş akışında duraklama kullanmak, Office 365 grup, bir dağıtım grubu veya posta etkin güvenlik grubunun e-posta Gönder veya aynı anda 200'den daha az sayıda alıcıya göndermek.</span><span class="sxs-lookup"><span data-stu-id="c3577-112">For example, use a pause in the workflow, send the email to an Office 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="c3577-113">Daha fazla bilgi için aşağıdaki [makaleye](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)bakın.</span><span class="sxs-lookup"><span data-stu-id="c3577-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="c3577-114">İlgili konular</span><span class="sxs-lookup"><span data-stu-id="c3577-114">Related topics</span></span>
- [<span data-ttu-id="c3577-115">Akış oluşturma</span><span class="sxs-lookup"><span data-stu-id="c3577-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="c3577-116">SharePoint ve akış</span><span class="sxs-lookup"><span data-stu-id="c3577-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 