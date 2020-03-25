---
title: DLP İlke İpuçları çalışmıyor
ms.author: deniseb
author: denisebmsft
manager: laurawims
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c03d30be-474a-4a34-b3c0-240eb2a2c466
ms.custom:
- "1428"
- "3200001"
ms.openlocfilehash: 51b4472fa721443192eb542cac45965df67634df
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932606"
---
# <a name="dlp-policy-tip-issues"></a><span data-ttu-id="7f6ca-102">DLP İlke İpucu sorunları</span><span class="sxs-lookup"><span data-stu-id="7f6ca-102">DLP Policy Tip issues</span></span>

<span data-ttu-id="7f6ca-103">**Önemli**: Birçok SharePoint Online ve OneDrive müşterisi, arka planda çalışan hizmete karşı iş açısından kritik uygulamalar çalıştırıyor.</span><span class="sxs-lookup"><span data-stu-id="7f6ca-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="7f6ca-104">Bunlar arasında içerik geçişi, Veri Kaybıönleme (DLP) ve yedekleme çözümleri yer alır.</span><span class="sxs-lookup"><span data-stu-id="7f6ca-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="7f6ca-105">Bu eşi görülmemiş zamanlarda, SharePoint Online ve OneDrive hizmetlerinin uzak çalışma senaryolarında hizmete her zamankinden daha fazla bağımlı olan kullanıcılarınız için son derece kullanılabilir ve güvenilir kalmasını sağlamak için adımlar atıyoruz.</span><span class="sxs-lookup"><span data-stu-id="7f6ca-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="7f6ca-106">Bu hedefi desteklemek için, hafta içi gündüz saatlerinde arka plan uygulamalarına (geçiş, DLP ve yedekleme çözümleri) daha sıkı azaltma limitleri uyguladık.</span><span class="sxs-lookup"><span data-stu-id="7f6ca-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="7f6ca-107">Bu uygulamaların bu zamanlarda çok sınırlı bir iş artışı elde edeceğini bekleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="7f6ca-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="7f6ca-108">Ancak, bölge için akşam ve hafta sonu saatlerinde, hizmet arka plan uygulamalarından gelen isteklerin önemli ölçüde daha yüksek hacimli işlemek için hazır olacaktır.</span><span class="sxs-lookup"><span data-stu-id="7f6ca-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="7f6ca-109">**DLP ilke ipuçları**</span><span class="sxs-lookup"><span data-stu-id="7f6ca-109">**DLP policy tips**</span></span>

<span data-ttu-id="7f6ca-110">**DLP ilkeleri**kullanırken, kullanıcılar **ilke ipuçları**ile bir ilke ihlali haberdar edilebilir.</span><span class="sxs-lookup"><span data-stu-id="7f6ca-110">When using **DLP policies**, users can be notified of a policy violation with **policy tips**.</span></span> <span data-ttu-id="7f6ca-111">Yöneticiler, DLP ilkelerini sınarken veya ilke tam uygulama modundayken görüntülenecek ilke ipuçlarını yapılandırabilir.</span><span class="sxs-lookup"><span data-stu-id="7f6ca-111">Admins can configure policy tips to display while testing their DLP policy or when the policy is in full enforcement mode.</span></span>
  
<span data-ttu-id="7f6ca-112">Güvenlik ve Uyumluluk merkezindeki DLP ilkeniz hakkındaki ilke ipuçlarını tam uygulama modunda yapılandırmak için aşağıdakileri yapın:</span><span class="sxs-lookup"><span data-stu-id="7f6ca-112">To configure policy tips on your DLP policy in the Security and Compliance center in full enforcement mode, do the following:</span></span>
  
- <span data-ttu-id="7f6ca-113">[Buradaki](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)adımları kullanarak DLP kuralında ilke ipuçlarının **etkinleştirildiğinden** emin olun.</span><span class="sxs-lookup"><span data-stu-id="7f6ca-113">Ensure policy tips have been **enabled** on the DLP rule using the steps [here](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span></span>

- <span data-ttu-id="7f6ca-114">İçeriğinizin bu [makalede](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)özetlenen kuralı tetiklemek için **gerekenle** **eşleştiğinden** emin olun.</span><span class="sxs-lookup"><span data-stu-id="7f6ca-114">Ensure your **content matches** what is **required** to trigger the rule outlined in this article [here](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="7f6ca-115">İlke ipuçları hem OWA hem de Outlook'ta görüntülenir.</span><span class="sxs-lookup"><span data-stu-id="7f6ca-115">Policy tips display in both OWA and Outlook.</span></span> <span data-ttu-id="7f6ca-116">Ancak, **Outlook 2013 veya daha sonra**kullanırken, ilke ipuçları yalnızca belirli koşullar altında görüntülenir.</span><span class="sxs-lookup"><span data-stu-id="7f6ca-116">However, when using **Outlook 2013 or later**, policy tips are only displayed under certain conditions.</span></span> <span data-ttu-id="7f6ca-117">Bu koşullar burada listelenmiştir: [İlke İpuçlarını görüntülemek için Outlook 2013 veya sonraki](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions) koşullar</span><span class="sxs-lookup"><span data-stu-id="7f6ca-117">These conditions are listed here: [Supported conditions for Outlook 2013 or later for displaying Policy Tips](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)</span></span>

<span data-ttu-id="7f6ca-118">DLP ilke ipuçları hakkında daha fazla bilgi için bkz: [DLP İlkeleri için ilke ipuçlarını göster](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)</span><span class="sxs-lookup"><span data-stu-id="7f6ca-118">For additional information on DLP policy tips, see: [Show policy tips for DLP Policies](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)</span></span>
  