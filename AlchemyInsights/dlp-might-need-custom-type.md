---
title: DLP, özel bir türde olabilir
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 72b16d437f97de27cbdc364f022c3e2059b31ef0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712204"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="c932a-102">DLP, özel bir türde olabilir</span><span class="sxs-lookup"><span data-stu-id="c932a-102">DLP might need a custom type</span></span>

<span data-ttu-id="c932a-103">**Önemli**: Bu benzeri görünmemiş zamanlarda, SharePoint Online ve OneDrive hizmetlerinin kullanılabilirlik düzeyinin her zaman yüksek olmasını sağlamaya yönelik adımlar atıyoruz. Daha fazla bilgi için lütfen [SharePoint Online Geçici Özellik Değişiklikleri](https://aka.ms/ODSPAdjustments) sayfasını ziyaret edin.</span><span class="sxs-lookup"><span data-stu-id="c932a-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="c932a-104">**DLP, özel bilgi türü gerektirebilir**</span><span class="sxs-lookup"><span data-stu-id="c932a-104">**DLP may require a custom information type**</span></span>

<span data-ttu-id="c932a-105">Veri kaybı önleme (DLP) ilkesiyle, kuruluşunuzdaki hassas verileri tanımlayabilir ve koruyabilir.</span><span class="sxs-lookup"><span data-stu-id="c932a-105">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="c932a-106">Bazı senaryolarda, kuruluşunuzun verilerini korumanız için kendi **özel** hassas bilgi türünüzün oluşturulması gerekebilir.</span><span class="sxs-lookup"><span data-stu-id="c932a-106">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="c932a-107">Örneğin, kuruluşunuzun kuruluşunuz için belirli biçimdeki çalışan kimliklerini veya diğer verileri belirleyip korumanız gerekebilir. Öyleyse, daha fazla bilgi için aşağıdaki makalelere bakın.</span><span class="sxs-lookup"><span data-stu-id="c932a-107">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="c932a-108">**Yerleşik duyarlı bir bilgi türünü özelleştirme**</span><span class="sxs-lookup"><span data-stu-id="c932a-108">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="c932a-109">Yerleşik duyarlı bir bilgi türü yalnızca birkaç şeyle ihtiyaçlarınızı karşılıyorsa, [yerleşik duyarlı bir bilgi türünü özelleştirebilirsiniz](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="c932a-109">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="c932a-110">Örneğin, anahtar sözcükleri ekleyebilir veya kaldırabilirsiniz ya da tarih veya adres gibi destekleyici bir kanıt ekleyebilir veya kaldırabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="c932a-110">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="c932a-111">**Özel hassas bilgi türü oluşturma**</span><span class="sxs-lookup"><span data-stu-id="c932a-111">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="c932a-112">Ancak farklı türde duyarlı bilgileri tümüyle bulmanız ve korumanız gerekiyorsa, güvenlik & Uyumluluk Merkezi Kullanıcı arabiriminde [özel bir hassas bilgi türü oluşturabilirsiniz](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) .</span><span class="sxs-lookup"><span data-stu-id="c932a-112">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="c932a-113">**Güvenlik & Uyumluluk Merkezi PowerShell 'de özel hassas bir bilgi türü oluşturma**</span><span class="sxs-lookup"><span data-stu-id="c932a-113">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="c932a-114">Son olarak, Kullanıcı arabirimi ihtiyaç duyacağınız tüm seçenekleri sağlamıyorsa, [güvenlik & Uyumluluk Merkezi PowerShell 'de özel bir hassas bilgi türü oluşturabilirsiniz](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="c932a-114">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="c932a-115">Bir XML dosyasıyla başlayarak, sağlanan her seçeneği kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="c932a-115">By starting with an XML file, you can use every option available.</span></span>
