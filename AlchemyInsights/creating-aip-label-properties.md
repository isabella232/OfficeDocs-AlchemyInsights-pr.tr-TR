---
title: AIP Etiket İlkeleri Oluşturma
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "4539"
- "9002266"
ms.openlocfilehash: de7d76564cabb0a5dd1a836984df6b1a63b2b218
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44569515"
---
# <a name="creating-aip-label-policies"></a><span data-ttu-id="7adee-102">AIP Etiket İlkeleri Oluşturma</span><span class="sxs-lookup"><span data-stu-id="7adee-102">Creating AIP Label Policies</span></span>

<span data-ttu-id="7adee-103">Azure Bilgi Koruması (AIP) etiketleri, bir kuruluşun tipik olarak oluşturduğu ve kişisel verilerin en düşük sınıflandırmasından son derece gizli verilerin en yüksek sınıflandırmasına kadar depoladığının tüm veri yelpazesiyle kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="7adee-103">Azure Information Protection(AIP) labels can be used with the full range of data that an organization typically creates and stores, from the lowest classification of personal data, to the highest classification of highly confidential data.</span></span> <span data-ttu-id="7adee-104">Azure Bilgi Koruma İlkeleri, [AIP Birleşik Etiketleme istemcisi](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history)için değil, Azure Bilgi Koruması (AIP) klasik istemcisi için geçerlidir.</span><span class="sxs-lookup"><span data-stu-id="7adee-104">Azure Information Protection Policies apply to the Azure Information Protection(AIP) classic client and not the  [AIP Unified Labeling client](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span></span> <span data-ttu-id="7adee-105">AIP ilkesinde, şu gibi seçenekler de dahil olmak üzere birden çok öğeyi yapılandırabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="7adee-105">You can configure multiple elements in an AIP policy, including options like:</span></span>

- <span data-ttu-id="7adee-106">Hangi etiketin yöneticilerin veya kullanıcının belgeleri ve e-postaları sınıflandırmasına ve korumasına izin verme seçeneği</span><span class="sxs-lookup"><span data-stu-id="7adee-106">Option for which label will let administrators or user classify and protection(optional) documents and emails</span></span>
- <span data-ttu-id="7adee-107">Kullanıcılar belgeleri kaydederken ve e-posta gönderirken sınıflandırmayı zorlama seçeneği</span><span class="sxs-lookup"><span data-stu-id="7adee-107">Option to enforce classification when users save documents and send email</span></span>
- <span data-ttu-id="7adee-108">E-posta iletisini ekleri temel alınarak otomatik olarak etiketleme seçeneği.</span><span class="sxs-lookup"><span data-stu-id="7adee-108">Option to automatically label an email message, based on its attachments.</span></span>
- <span data-ttu-id="7adee-109">Bilgi Koruması çubuğunun Office uygulamalarında görüntülenip görüntülenmediğini denetleme seçeneği</span><span class="sxs-lookup"><span data-stu-id="7adee-109">Option to control whether the Information Protection bar is displayed in Office applications</span></span>

<span data-ttu-id="7adee-110">Azure Bilgi Koruması ilkeleri yle ilgili ek seçenekler ve bilgiler için bkz: [Azure Bilgi Koruması ilkesine genel bakış.](https://docs.microsoft.com/azure/information-protection/overview-policy)</span><span class="sxs-lookup"><span data-stu-id="7adee-110">For additional options and information on Azure Information Protection policies, see: [Overview of the Azure Information Protection policy](https://docs.microsoft.com/azure/information-protection/overview-policy).</span></span>  

<span data-ttu-id="7adee-111">AIP ilkeleriyle ilgili diğer yararlı kaynaklar için bkz:</span><span class="sxs-lookup"><span data-stu-id="7adee-111">For other helpful resources regarding AIP policies, see:</span></span>

- [<span data-ttu-id="7adee-112">Öğretici: Azure Bilgi Koruması ilkesi ayarlarını yapılandırın ve yeni bir etiket oluşturun</span><span class="sxs-lookup"><span data-stu-id="7adee-112">Tutorial: Configure Azure Information Protection policy settings and create a new label</span></span>](https://docs.microsoft.com/azure/information-protection/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="7adee-113">Azure Bilgi Koruması ilkesini yapılandırma</span><span class="sxs-lookup"><span data-stu-id="7adee-113">Configuring the Azure Information Protection policy</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy)  
- [<span data-ttu-id="7adee-114">Duyarlılık etiketleri ve ilkelerini oluşturma ve yapılandırma</span><span class="sxs-lookup"><span data-stu-id="7adee-114">Create and configure sensitivity labels and their policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/create-sensitivity-labels)  
- [<span data-ttu-id="7adee-115">Azure Bilgi Koruması kullanan yaygın senaryolar için nasıl kullanılır kılavuzları</span><span class="sxs-lookup"><span data-stu-id="7adee-115">How-to guides for common scenarios that use Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/how-to-guides)  
- [<span data-ttu-id="7adee-116">Azure Bilgi Koruması belgelerini gözden geçirin</span><span class="sxs-lookup"><span data-stu-id="7adee-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)  
- [<span data-ttu-id="7adee-117">Azure Bilgi Koruması Gereksinimleri</span><span class="sxs-lookup"><span data-stu-id="7adee-117">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)  
- [<span data-ttu-id="7adee-118">Azure Bilgi Koruması için hızlı başlangıç öğreticisi</span><span class="sxs-lookup"><span data-stu-id="7adee-118">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="7adee-119">Azure Bilgi Koruması istemcisi indirin</span><span class="sxs-lookup"><span data-stu-id="7adee-119">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)