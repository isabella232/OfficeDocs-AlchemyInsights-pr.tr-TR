---
title: DNS kayıtlarını güncelleştirerek web sitenizi geçerli barındırma sağlayıcınızla koruma
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 7bd36c3954d12d3ee4ac624a2f827d8e5cd88082
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665780"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>DNS kayıtlarını güncelleştirerek web sitenizi geçerli barındırma sağlayıcınızla koruma

1. Microsoft 365 yönetici merkezinde, **Kurulum**Etki  >  [Alanları](https://portal.office.com/adminportal/home#/Domains) sayfasına gidin ve etki alanları listesinde web siteniz için kullandığınız etki alanını seçin.

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

2. **Kaydet**'i seçin.
