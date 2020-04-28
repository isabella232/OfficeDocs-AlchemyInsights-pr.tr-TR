---
title: Günlük e-posta sınırı aşıldı. İş akışı askıya alındı.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 5a510f1137c7c49cd1de3d3fd2a470759e37ba1e
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/27/2020
ms.locfileid: "43908724"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="db391-103">Günlük e-posta Sınırı Aşıldı.</span><span class="sxs-lookup"><span data-stu-id="db391-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="db391-104">İş akışı askıya alındı.</span><span class="sxs-lookup"><span data-stu-id="db391-104">Workflow is suspended.</span></span>

<span data-ttu-id="db391-105">Bu hata aşağıdaki senaryolarda alınabilir:</span><span class="sxs-lookup"><span data-stu-id="db391-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="db391-106">SharePoint Online'da SharePoint 2010 veya SharePoint 2013 iş akışı platform türünü kullanan bir iş akışınız vardır.</span><span class="sxs-lookup"><span data-stu-id="db391-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="db391-107">İş akışı, aynı anda 200'den fazla kullanıcıya, günde 10.000'den fazla alıcıya veya dakikada 30'dan fazla iletigöndermek üzere özel bir e-posta iletisi gönderecek şekilde yapılandırılmıştır.</span><span class="sxs-lookup"><span data-stu-id="db391-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="db391-108">İş akışını çalıştırdığınızda, e-posta iletisi gönderilmez ve aşağıdaki davranışı fark e-postayla fark e-posta yla karşılarınız:</span><span class="sxs-lookup"><span data-stu-id="db391-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="db391-109">SharePoint 2013 platform türünü kullanan bir iş akışı için **İş Akışı Durumu** sayfasına göz atarsınız.</span><span class="sxs-lookup"><span data-stu-id="db391-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="db391-110">İş Akışı Durumu sayfasında, **İç Durum** **Başlatıldı**olarak ayarlanır ve bilgi balonu **alıcıya gönderilemeyince**görüntülenir.</span><span class="sxs-lookup"><span data-stu-id="db391-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="db391-111">Bu sorunu çözmek için iş akışınızı Exchange Online gönderen [sınırlarını](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits)aşmadan e-posta iletileri gönderecek şekilde yapılandırın.</span><span class="sxs-lookup"><span data-stu-id="db391-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="db391-112">Örneğin, iş akışında bir duraklama kullanın, e-postayı bir Microsoft 365 grubuna, bir dağıtım grubuna veya posta etkin güvenlik grubuna gönderin veya iletiyi aynı anda 200'den az alıcıya gönderin.</span><span class="sxs-lookup"><span data-stu-id="db391-112">For example, use a pause in the workflow, send the email to an Microsoft 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="db391-113">Daha fazla bilgi için aşağıdaki [makaleye](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)bakın.</span><span class="sxs-lookup"><span data-stu-id="db391-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="db391-114">İlgili konular</span><span class="sxs-lookup"><span data-stu-id="db391-114">Related topics</span></span>
- [<span data-ttu-id="db391-115">Akış Oluştur</span><span class="sxs-lookup"><span data-stu-id="db391-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="db391-116">SharePoint ve Akış</span><span class="sxs-lookup"><span data-stu-id="db391-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 