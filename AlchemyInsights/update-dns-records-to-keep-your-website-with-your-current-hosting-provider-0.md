---
title: DNS kayıtlarını güncelleştirerek web sitenizi geçerli barındırma sağlayıcınızla koruma
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 89bce2aa5931c0c20706efabd42d2351be43938b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827560"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="c5526-102">DNS kayıtlarını güncelleştirerek web sitenizi geçerli barındırma sağlayıcınızla koruma</span><span class="sxs-lookup"><span data-stu-id="c5526-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="c5526-103">Microsoft 365 yönetim merkezinde Kurulum Etki Alanları sayfasına gidin ve etki alanları listesinde web siteniz için kullanmakta olduğunu  >  [](https://admin.microsoft.com/Adminportal#/Domains) etki alanını seçin.</span><span class="sxs-lookup"><span data-stu-id="c5526-103">In the Microsoft 365 admin center, go to the **Setup** > [Domains](https://admin.microsoft.com/Adminportal#/Domains) page, and in the list of domains, select the domain you're using for your website.</span></span>

2. <span data-ttu-id="c5526-104">**+ Yeni özel kayıt** 'ı seçin ve aşağıdakileri girin:</span><span class="sxs-lookup"><span data-stu-id="c5526-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="c5526-105">**DNS türü** için şunu girin: **A (Adres)**</span><span class="sxs-lookup"><span data-stu-id="c5526-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="c5526-106">**Ana bilgisayar adı veya Diğer ad** olarak şunu yazın: **@**</span><span class="sxs-lookup"><span data-stu-id="c5526-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="c5526-107">**IP Adresi** olarak web sitenizin şu anda barındırıldığı statik IP adresini yazın (örneğin, 172.16.140.1).</span><span class="sxs-lookup"><span data-stu-id="c5526-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="c5526-p101">Bu adres web sitesinin  *statik*  IP adresi olmalıdır,  *dinamik*  IP adresi olamaz. Genel web siteniz için bir statik IP adresi alıp alamayacağınızdan emin olmak için web sitenizin barındırıldığı siteyi kontrol edin.</span><span class="sxs-lookup"><span data-stu-id="c5526-p101">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address. Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="c5526-110">**Kaydet** 'i seçin.</span><span class="sxs-lookup"><span data-stu-id="c5526-110">Select **Save**.</span></span>

<span data-ttu-id="c5526-111">Buna ek olarak, müşterilerin web sitenizi bulmalarına yardım etmek için bir CNAME kaydı da oluşturabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="c5526-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="c5526-112">**+ Yeni özel kayıt** 'ı seçin ve aşağıdakileri girin:</span><span class="sxs-lookup"><span data-stu-id="c5526-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="c5526-113">**DNS türü** için şunu girin: **CNAME (Diğer ad)**</span><span class="sxs-lookup"><span data-stu-id="c5526-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="c5526-114">**Ana bilgisayar adı veya Diğer ad** olarak şunu yazın: **www**</span><span class="sxs-lookup"><span data-stu-id="c5526-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="c5526-115">**İşaret edilen adres** olarak, web sitenizin tam etki alanı adını (FQDN) yazın (örneğin, contoso.com).</span><span class="sxs-lookup"><span data-stu-id="c5526-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="c5526-116">**Kaydet** 'i seçin.</span><span class="sxs-lookup"><span data-stu-id="c5526-116">Select **Save**.</span></span>
