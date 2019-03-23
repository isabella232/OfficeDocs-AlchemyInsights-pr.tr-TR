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
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>DNS kayıtlarını güncelleştirerek web sitenizi geçerli barındırma sağlayıcınızla koruma

1. [Etki alanları](https://portal.office.com/adminportal/home#/Domains) sayfasındaki etki alanları listesinde, web siteniz için kullandığınız etki alanını seçin ve ardından yönetim bölmesindeki **DNS ayarları** 'nı seçin. 
    
2. **+ Yeni özel kayıt** 'ı seçin ve aşağıdakileri girin: 
    
  - **DNS türü** için şunu girin: **A (Adres)**
    
  - **Ana bilgisayar adı veya Diğer ad** olarak şunu yazın: **@**
    
  - **IP Adresi** olarak web sitenizin şu anda barındırıldığı statik IP adresini yazın (örneğin, 172.16.140.1). 
    
    Bu adres web sitesinin  *statik*  IP adresi olmalıdır,  *dinamik*  IP adresi olamaz. Genel web siteniz için bir statik IP adresi alıp alamayacağınızdan emin olmak için web sitenizin barındırıldığı siteyi kontrol edin. 
    
3. **Kaydet** 'i seçin. 
    
Buna ek olarak, müşterilerin web sitenizi bulmalarına yardım etmek için bir CNAME kaydı da oluşturabilirsiniz.
  
1. **+ Yeni özel kayıt** 'ı seçin ve aşağıdakileri girin: 
    
  - **DNS türü** için şunu girin: **CNAME (Diğer ad)**
    
  - **Ana bilgisayar adı veya Diğer ad** olarak şunu yazın: **www**
    
  - **İşaret edilen adres** olarak, web sitenizin tam etki alanı adını (FQDN) yazın (örneğin, contoso.com). 
    
2. **Kaydet** 'i seçin. 
    

