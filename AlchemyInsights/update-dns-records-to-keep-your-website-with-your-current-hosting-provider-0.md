---
title: DNS kayıtlarını güncelleştirerek web sitenizi geçerli barındırma sağlayıcınızla koruma
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: f2cdb319e56b82c09b7a9856c81a45e69dee6759
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/22/2019
ms.locfileid: "30761006"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="5e763-102">DNS kayıtlarını güncelleştirerek web sitenizi geçerli barındırma sağlayıcınızla koruma</span><span class="sxs-lookup"><span data-stu-id="5e763-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="5e763-103">[Etki alanları](https://portal.office.com/adminportal/home#/Domains) sayfasındaki etki alanları listesinde, web siteniz için kullandığınız etki alanını seçin ve ardından yönetim bölmesindeki **DNS ayarları** 'nı seçin.</span><span class="sxs-lookup"><span data-stu-id="5e763-103">On the [Domains](https://portal.office.com/adminportal/home#/Domains) page, in the list of domains, select the domain you're using for your website, and then select **DNS settings** in the management pane.</span></span> 
    
2. <span data-ttu-id="5e763-104">**+ Yeni özel kayıt** 'ı seçin ve aşağıdakileri girin:</span><span class="sxs-lookup"><span data-stu-id="5e763-104">Select **+ New custom record** and enter the following:</span></span> 
    
  - <span data-ttu-id="5e763-105">**DNS türü** için şunu girin: **A (Adres)**</span><span class="sxs-lookup"><span data-stu-id="5e763-105">For **DNS type** enter: **A (Address)**</span></span>
    
  - <span data-ttu-id="5e763-106">**Ana bilgisayar adı veya Diğer ad** olarak şunu yazın: **@**</span><span class="sxs-lookup"><span data-stu-id="5e763-106">For **Host name or Alias**, type the following: **@**</span></span>
    
  - <span data-ttu-id="5e763-107">**IP Adresi** olarak web sitenizin şu anda barındırıldığı statik IP adresini yazın (örneğin, 172.16.140.1).</span><span class="sxs-lookup"><span data-stu-id="5e763-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span> 
    
    <span data-ttu-id="5e763-p101">Bu adres web sitesinin  *statik*  IP adresi olmalıdır,  *dinamik*  IP adresi olamaz. Genel web siteniz için bir statik IP adresi alıp alamayacağınızdan emin olmak için web sitenizin barındırıldığı siteyi kontrol edin.</span><span class="sxs-lookup"><span data-stu-id="5e763-p101">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address. Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span> 
    
3. <span data-ttu-id="5e763-110">**Kaydet** 'i seçin.</span><span class="sxs-lookup"><span data-stu-id="5e763-110">Select **Save**.</span></span> 
    
<span data-ttu-id="5e763-111">Buna ek olarak, müşterilerin web sitenizi bulmalarına yardım etmek için bir CNAME kaydı da oluşturabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="5e763-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="5e763-112">**+ Yeni özel kayıt** 'ı seçin ve aşağıdakileri girin:</span><span class="sxs-lookup"><span data-stu-id="5e763-112">Select **+ New custom record** and enter the following:</span></span> 
    
  - <span data-ttu-id="5e763-113">**DNS türü** için şunu girin: **CNAME (Diğer ad)**</span><span class="sxs-lookup"><span data-stu-id="5e763-113">For **DNS type** enter: **CNAME (Alias)**</span></span>
    
  - <span data-ttu-id="5e763-114">**Ana bilgisayar adı veya Diğer ad** olarak şunu yazın: **www**</span><span class="sxs-lookup"><span data-stu-id="5e763-114">For **Host name or Alias**, type the following: **www**</span></span>
    
  - <span data-ttu-id="5e763-115">**İşaret edilen adres** olarak, web sitenizin tam etki alanı adını (FQDN) yazın (örneğin, contoso.com).</span><span class="sxs-lookup"><span data-stu-id="5e763-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span> 
    
2. <span data-ttu-id="5e763-116">**Kaydet** 'i seçin.</span><span class="sxs-lookup"><span data-stu-id="5e763-116">Select **Save**.</span></span> 
    

