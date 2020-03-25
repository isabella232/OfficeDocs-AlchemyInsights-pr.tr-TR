---
title: SharePoint Online Azaltma
ms.author: pebaum
author: pebaum
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 59104ef96c95de4e4bc7744825245bdafba97d7c
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931246"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="b5ef3-102">SharePoint Online Azaltma</span><span class="sxs-lookup"><span data-stu-id="b5ef3-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="b5ef3-103">**Önemli**: Birçok SharePoint Online ve OneDrive müşterisi, arka planda çalışan hizmete karşı iş açısından kritik uygulamalar çalıştırıyor.</span><span class="sxs-lookup"><span data-stu-id="b5ef3-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="b5ef3-104">Bunlar arasında içerik geçişi, Veri Kaybıönleme (DLP) ve yedekleme çözümleri yer alır.</span><span class="sxs-lookup"><span data-stu-id="b5ef3-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="b5ef3-105">Bu eşi görülmemiş zamanlarda, SharePoint Online ve OneDrive hizmetlerinin uzak çalışma senaryolarında hizmete her zamankinden daha fazla bağımlı olan kullanıcılarınız için son derece kullanılabilir ve güvenilir kalmasını sağlamak için adımlar atıyoruz.</span><span class="sxs-lookup"><span data-stu-id="b5ef3-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="b5ef3-106">Bu hedefi desteklemek için, hafta içi gündüz saatlerinde arka plan uygulamalarına (geçiş, DLP ve yedekleme çözümleri) daha sıkı azaltma limitleri uyguladık.</span><span class="sxs-lookup"><span data-stu-id="b5ef3-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="b5ef3-107">Bu uygulamaların bu zamanlarda çok sınırlı bir iş artışı elde edeceğini bekleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="b5ef3-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="b5ef3-108">Ancak, bölge için akşam ve hafta sonu saatlerinde, hizmet arka plan uygulamalarından gelen isteklerin önemli ölçüde daha yüksek hacimli işlemek için hazır olacaktır.</span><span class="sxs-lookup"><span data-stu-id="b5ef3-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="b5ef3-109">**503 sunucu meşgul hata**</span><span class="sxs-lookup"><span data-stu-id="b5ef3-109">**503 server is busy error**</span></span>

<span data-ttu-id="b5ef3-110">Kullanıcılar SharePoint veya OneDrive sitelerine gezinmeye çalışırken bir 503 sunucu meşgul hata alabilir.</span><span class="sxs-lookup"><span data-stu-id="b5ef3-110">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="b5ef3-111">Bu hata, SharePoint hizmeti içinde daraltma neden olabilir.</span><span class="sxs-lookup"><span data-stu-id="b5ef3-111">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="b5ef3-112">SharePoint Online, SharePoint Online hizmetinin en iyi performansını ve güvenilirliğini korumak için azaltma yı kullanır.</span><span class="sxs-lookup"><span data-stu-id="b5ef3-112">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="b5ef3-113">Azaltma, kaynakların aşırı kullanımını önlemek için kullanıcı eylemlerinin veya eşzamanlı çağrıların (komut dosyası veya koda göre) sayısını sınırlar.</span><span class="sxs-lookup"><span data-stu-id="b5ef3-113">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> 

<span data-ttu-id="b5ef3-114">Azaltma hakkında daha fazla bilgi için [SharePoint Online'da daraltılmaktan veya engellenmesinden kaçının.](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)</span><span class="sxs-lookup"><span data-stu-id="b5ef3-114">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="b5ef3-115">Bu hatanın azaltmayla ilgisi olmadığını düşünüyorsanız, [İleti merkezi'ne](https://portal.office.com/adminportal/home#/MessageCenter)yönlendirerek kiracınızda etkin bir bakım olup olmadığını kontrol edebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="b5ef3-115">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="b5ef3-116">Son olarak, oluşabilecek danışma/olayları kontrol etmek için [Hizmet Durumu](https://portal.office.com/adminportal/home#/servicehealth) sayfasını ziyaret ettiğinizden emin olun.</span><span class="sxs-lookup"><span data-stu-id="b5ef3-116">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

