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
ms.openlocfilehash: 87fcb5c3cc9ccd525265097b66d9d9b3a85c5feb
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977290"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="f0e11-102">DLP özel bir tür gerekebilir</span><span class="sxs-lookup"><span data-stu-id="f0e11-102">DLP might need a custom type</span></span>

<span data-ttu-id="f0e11-103">**Önemli**: Bu eşi görülmemiş zamanlarda, SharePoint Online ve OneDrive hizmetlerinin yüksek oranda kullanılabilir kalmasını sağlamak için adımlar atıyoruz – Daha fazla bilgi için lütfen [SharePoint Online Geçici Özellik Ayarlamaları'nı](https://aka.ms/ODSPAdjustments) ziyaret edin.</span><span class="sxs-lookup"><span data-stu-id="f0e11-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="f0e11-104">**DLP özel bir bilgi türü gerektirebilir**</span><span class="sxs-lookup"><span data-stu-id="f0e11-104">**DLP may require a custom information type**</span></span>

<span data-ttu-id="f0e11-105">Veri kaybıönleme (DLP) ilkesiyle, kuruluşunuzdaki hassas verileri tanımlayabilir ve koruyabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="f0e11-105">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="f0e11-106">Bazı senaryolarda, kuruluşunuzun verilerini korumak için kendi **özel** duyarlı bilgi türünü oluşturmanız gerekebilir.</span><span class="sxs-lookup"><span data-stu-id="f0e11-106">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="f0e11-107">Örneğin, kuruluşunuzun çalışan kimliklerini veya orgunuza özgü bir biçimdeki diğer verileri tanımlaması ve koruması gerekebilir. Bu nedenle, daha fazla bilgi için aşağıdaki makalelere bakın.</span><span class="sxs-lookup"><span data-stu-id="f0e11-107">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="f0e11-108">**Yerleşik duyarlı bilgi türünü özelleştirme**</span><span class="sxs-lookup"><span data-stu-id="f0e11-108">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="f0e11-109">Yerleşik bir hassas bilgi türü yalnızca birkaç değişiklikle ihtiyaçlarınızı karşılayacaksa, [yerleşik hassas bilgi türünü özelleştirebilirsiniz.](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type)</span><span class="sxs-lookup"><span data-stu-id="f0e11-109">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="f0e11-110">Örneğin, anahtar kelimeler ekleyebilir veya kaldırabilir veya tarih veya adres gibi destekleyici kanıt ekleyebilir veya kaldırabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="f0e11-110">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="f0e11-111">**Özel duyarlı bilgi türü oluşturma**</span><span class="sxs-lookup"><span data-stu-id="f0e11-111">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="f0e11-112">Ancak, farklı bir hassas bilgi türünü tamamen tanımlamanız ve korumanız gerekiyorsa, Güvenlik & Uyumluluk Merkezi'nin kullanıcı bilgi sinde [özel bir bilgi türü oluşturabilirsiniz.](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type)</span><span class="sxs-lookup"><span data-stu-id="f0e11-112">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="f0e11-113">**Güvenlik & Uyumluluk Merkezi PowerShell'de özel duyarlı bilgi türü oluşturma**</span><span class="sxs-lookup"><span data-stu-id="f0e11-113">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="f0e11-114">Son olarak, Kullanıcı Bira gereksinimi duyduğunuz tüm seçenekleri sağlamazsa, [Güvenlik & Uyumluluk Merkezi PowerShell'de özel bir bilgi türü oluşturabilirsiniz.](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="f0e11-114">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="f0e11-115">Bir XML dosyasıyla başlayarak, kullanılabilir her seçeneği kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="f0e11-115">By starting with an XML file, you can use every option available.</span></span>
