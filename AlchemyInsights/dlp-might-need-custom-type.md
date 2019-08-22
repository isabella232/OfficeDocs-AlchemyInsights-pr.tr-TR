---
title: Özel bir tür DLP gerekebilir
ms.author: stephow
author: stephow-MSFT
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
ms.openlocfilehash: 612b6652b445914063ac825847f5698d3afc3a00
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36530371"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="8e805-102">Özel bir tür DLP gerekebilir</span><span class="sxs-lookup"><span data-stu-id="8e805-102">DLP might need a custom type</span></span>

<span data-ttu-id="8e805-103">Veri kaybını önleme (DLP) ilkesi ile tanımlamak ve kuruluşunuzdaki önemli verileri koru.</span><span class="sxs-lookup"><span data-stu-id="8e805-103">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="8e805-104">Bazı senaryolarda, kuruluunuzun verilerini korumak için kendi **Özel** önemli bilgiler türünüzü oluşturmanız gerekebilir.</span><span class="sxs-lookup"><span data-stu-id="8e805-104">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="8e805-105">Örneğin, kuruluşunuzun tanımlamak ve çalışan kimliklerini veya diğer bazı biçiminde, Krlş. için belirli veri koruma gerekebilir Öyleyse, daha fazla bilgi için aşağıdaki makalelere bakın.</span><span class="sxs-lookup"><span data-stu-id="8e805-105">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="8e805-106">**Yerleşik hassas bilgilerin türünü özelleştirin**</span><span class="sxs-lookup"><span data-stu-id="8e805-106">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="8e805-107">Yerleşik hassas bilgilerin türü birkaç tweaks ile gereksinimlerinizi karşılamıyorsa, bu [bir yerleşik hassas bilgi türünü](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type)özelleştirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="8e805-107">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="8e805-108">Örneğin, veya anahtar sözcükler, kaldırmak veya eklemek ekleyip bir tarih veya adres gibi destekleyici kanıt.</span><span class="sxs-lookup"><span data-stu-id="8e805-108">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="8e805-109">**Özel hassas bilgi türü oluştur**</span><span class="sxs-lookup"><span data-stu-id="8e805-109">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="8e805-110">Ancak tanımlamak ve hassas bilgiler farklı türde tamamen korumak gerekiyorsa, kullanıcı arabiriminde Uyumluluk Merkezi güvenlik &, [özel önemli bilgiler türü oluşturmak](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) olabilir.</span><span class="sxs-lookup"><span data-stu-id="8e805-110">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="8e805-111">**Güvenlik & Uyumluluk Merkezi PowerShell özel önemli bilgiler türü oluştur**</span><span class="sxs-lookup"><span data-stu-id="8e805-111">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="8e805-112">Gereksinim duyduğunuz tüm seçenekleri UI vermiyorsa, son olarak, [Güvenlik & Uyumluluk Merkezi PowerShell özel önemli bilgiler yazıyla](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell)oluşturabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="8e805-112">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="8e805-113">Bir XML dosyası ile başlayarak kullanılabilir her seçeneği kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="8e805-113">By starting with an XML file, you can use every option available.</span></span>
