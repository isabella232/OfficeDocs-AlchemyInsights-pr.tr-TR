---
title: DLP özel bir tür gerekebilir
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: ''
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 890bba57bc36c034c507e6124cd6593ef4d92af8
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932678"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="2dafc-102">DLP özel bir tür gerekebilir</span><span class="sxs-lookup"><span data-stu-id="2dafc-102">DLP might need a custom type</span></span>

<span data-ttu-id="2dafc-103">**Önemli**: Birçok SharePoint Online ve OneDrive müşterisi, arka planda çalışan hizmete karşı iş açısından kritik uygulamalar çalıştırıyor.</span><span class="sxs-lookup"><span data-stu-id="2dafc-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="2dafc-104">Bunlar arasında içerik geçişi, Veri Kaybıönleme (DLP) ve yedekleme çözümleri yer alır.</span><span class="sxs-lookup"><span data-stu-id="2dafc-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="2dafc-105">Bu eşi görülmemiş zamanlarda, SharePoint Online ve OneDrive hizmetlerinin uzak çalışma senaryolarında hizmete her zamankinden daha fazla bağımlı olan kullanıcılarınız için son derece kullanılabilir ve güvenilir kalmasını sağlamak için adımlar atıyoruz.</span><span class="sxs-lookup"><span data-stu-id="2dafc-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="2dafc-106">Bu hedefi desteklemek için, hafta içi gündüz saatlerinde arka plan uygulamalarına (geçiş, DLP ve yedekleme çözümleri) daha sıkı azaltma limitleri uyguladık.</span><span class="sxs-lookup"><span data-stu-id="2dafc-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="2dafc-107">Bu uygulamaların bu zamanlarda çok sınırlı bir iş artışı elde edeceğini bekleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="2dafc-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="2dafc-108">Ancak, bölge için akşam ve hafta sonu saatlerinde, hizmet arka plan uygulamalarından gelen isteklerin önemli ölçüde daha yüksek hacimli işlemek için hazır olacaktır.</span><span class="sxs-lookup"><span data-stu-id="2dafc-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="2dafc-109">**DLP özel bir bilgi türü gerektirebilir**</span><span class="sxs-lookup"><span data-stu-id="2dafc-109">**DLP may require a custom information type**</span></span>

<span data-ttu-id="2dafc-110">Veri kaybıönleme (DLP) ilkesiyle, kuruluşunuzdaki hassas verileri tanımlayabilir ve koruyabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="2dafc-110">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="2dafc-111">Bazı senaryolarda, kuruluşunuzun verilerini korumak için kendi **özel** duyarlı bilgi türünü oluşturmanız gerekebilir.</span><span class="sxs-lookup"><span data-stu-id="2dafc-111">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="2dafc-112">Örneğin, kuruluşunuzun çalışan kimliklerini veya orgunuza özgü bir biçimdeki diğer verileri tanımlaması ve koruması gerekebilir. Bu nedenle, daha fazla bilgi için aşağıdaki makalelere bakın.</span><span class="sxs-lookup"><span data-stu-id="2dafc-112">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="2dafc-113">**Yerleşik duyarlı bilgi türünü özelleştirme**</span><span class="sxs-lookup"><span data-stu-id="2dafc-113">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="2dafc-114">Yerleşik bir hassas bilgi türü yalnızca birkaç değişiklikle ihtiyaçlarınızı karşılayacaksa, [yerleşik hassas bilgi türünü özelleştirebilirsiniz.](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type)</span><span class="sxs-lookup"><span data-stu-id="2dafc-114">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="2dafc-115">Örneğin, anahtar kelimeler ekleyebilir veya kaldırabilir veya tarih veya adres gibi destekleyici kanıt ekleyebilir veya kaldırabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="2dafc-115">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="2dafc-116">**Özel duyarlı bilgi türü oluşturma**</span><span class="sxs-lookup"><span data-stu-id="2dafc-116">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="2dafc-117">Ancak, farklı bir hassas bilgi türünü tamamen tanımlamanız ve korumanız gerekiyorsa, Güvenlik & Uyumluluk Merkezi'nin kullanıcı bilgi sinde [özel bir bilgi türü oluşturabilirsiniz.](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type)</span><span class="sxs-lookup"><span data-stu-id="2dafc-117">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="2dafc-118">**Güvenlik & Uyumluluk Merkezi PowerShell'de özel duyarlı bilgi türü oluşturma**</span><span class="sxs-lookup"><span data-stu-id="2dafc-118">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="2dafc-119">Son olarak, Kullanıcı Bira gereksinimi duyduğunuz tüm seçenekleri sağlamazsa, [Güvenlik & Uyumluluk Merkezi PowerShell'de özel bir bilgi türü oluşturabilirsiniz.](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="2dafc-119">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="2dafc-120">Bir XML dosyasıyla başlayarak, kullanılabilir her seçeneği kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="2dafc-120">By starting with an XML file, you can use every option available.</span></span>
