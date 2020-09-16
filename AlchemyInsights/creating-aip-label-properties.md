---
title: IP etiket Ilkeleri oluşturma
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "4539"
- "9002266"
ms.openlocfilehash: bef170d8e38dcc91094b95604aeb1968d5c57fca
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732195"
---
# <a name="creating-aip-label-policies"></a><span data-ttu-id="5b917-102">IP etiket Ilkeleri oluşturma</span><span class="sxs-lookup"><span data-stu-id="5b917-102">Creating AIP Label Policies</span></span>

<span data-ttu-id="5b917-103">Azure Information Protection (AıP) etiketleri, bir kuruluşun normal olarak en düşük düzeyde gizli verilerin en yüksek sınıflandırmasına göre normal bir şekilde oluşturduğu tam veri aralığıyla kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="5b917-103">Azure Information Protection(AIP) labels can be used with the full range of data that an organization typically creates and stores, from the lowest classification of personal data, to the highest classification of highly confidential data.</span></span> <span data-ttu-id="5b917-104">Azure Information Protection Ilkeleri,  [IP birleştirilmiş etiketleme istemcisi](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history)değil, Azure Information Protection (AIP) Classic istemcisine uygulanır.</span><span class="sxs-lookup"><span data-stu-id="5b917-104">Azure Information Protection Policies apply to the Azure Information Protection(AIP) classic client and not the  [AIP Unified Labeling client](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span></span> <span data-ttu-id="5b917-105">Bir IP ilkesinde birden çok öğeyi yapılandırabilirsiniz; örneğin:</span><span class="sxs-lookup"><span data-stu-id="5b917-105">You can configure multiple elements in an AIP policy, including options like:</span></span>

- <span data-ttu-id="5b917-106">Hangi etiketin yöneticilere veya Kullanıcı sınıflandırmalarına ve korumasına (isteğe bağlı) belgelerin ve e-postaların</span><span class="sxs-lookup"><span data-stu-id="5b917-106">Option for which label will let administrators or user classify and protection(optional) documents and emails</span></span>
- <span data-ttu-id="5b917-107">Kullanıcılar belgeleri kaydederken ve e-posta gönderirken sınıflandırmayı zorunlu kılma seçeneği</span><span class="sxs-lookup"><span data-stu-id="5b917-107">Option to enforce classification when users save documents and send email</span></span>
- <span data-ttu-id="5b917-108">E-posta iletisini ekler doğrultusunda otomatik olarak etiketleme seçeneği.</span><span class="sxs-lookup"><span data-stu-id="5b917-108">Option to automatically label an email message, based on its attachments.</span></span>
- <span data-ttu-id="5b917-109">Bilgi koruması çubuğunun Office uygulamalarında gösterilip gösterilmeyeceğini denetleme seçeneği</span><span class="sxs-lookup"><span data-stu-id="5b917-109">Option to control whether the Information Protection bar is displayed in Office applications</span></span>

<span data-ttu-id="5b917-110">Azure bilgi koruması ilkeleriyle ilgili ek seçenekler ve bilgiler için bkz: [Azure bilgi koruması Ilkesine genel bakış](https://docs.microsoft.com/azure/information-protection/overview-policy).</span><span class="sxs-lookup"><span data-stu-id="5b917-110">For additional options and information on Azure Information Protection policies, see: [Overview of the Azure Information Protection policy](https://docs.microsoft.com/azure/information-protection/overview-policy).</span></span>  

<span data-ttu-id="5b917-111">IP ilkeleriyle ilgili diğer yararlı kaynaklar için bkz:</span><span class="sxs-lookup"><span data-stu-id="5b917-111">For other helpful resources regarding AIP policies, see:</span></span>

- [<span data-ttu-id="5b917-112">Öğretici: Azure bilgi koruması ilke ayarlarını yapılandırma ve yeni etiket oluşturma</span><span class="sxs-lookup"><span data-stu-id="5b917-112">Tutorial: Configure Azure Information Protection policy settings and create a new label</span></span>](https://docs.microsoft.com/azure/information-protection/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="5b917-113">Azure bilgi koruması ilkesini yapılandırma</span><span class="sxs-lookup"><span data-stu-id="5b917-113">Configuring the Azure Information Protection policy</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy)  
- [<span data-ttu-id="5b917-114">Duyarlılık etiketleri ve ilkelerini oluşturma ve yapılandırma</span><span class="sxs-lookup"><span data-stu-id="5b917-114">Create and configure sensitivity labels and their policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/create-sensitivity-labels)  
- [<span data-ttu-id="5b917-115">Azure bilgi koruması 'nı kullanan ortak senaryolar için nasıl yapılır kılavuzları</span><span class="sxs-lookup"><span data-stu-id="5b917-115">How-to guides for common scenarios that use Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/how-to-guides)  
- [<span data-ttu-id="5b917-116">Azure bilgi koruması belgelerini gözden geçirme</span><span class="sxs-lookup"><span data-stu-id="5b917-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)  
- [<span data-ttu-id="5b917-117">Azure bilgi koruması gereksinimleri</span><span class="sxs-lookup"><span data-stu-id="5b917-117">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)  
- [<span data-ttu-id="5b917-118">Azure bilgi koruması için Hızlı Başlangıç Öğreticisi</span><span class="sxs-lookup"><span data-stu-id="5b917-118">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="5b917-119">Azure bilgi Koruması istemcisini indirin</span><span class="sxs-lookup"><span data-stu-id="5b917-119">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)