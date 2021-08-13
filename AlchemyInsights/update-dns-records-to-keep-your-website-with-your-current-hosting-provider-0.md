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
ms.openlocfilehash: f868ce25d68f61da30d2db4de88aa83675c97857b3c1371cf2039e0b03895a64
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007702"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>DNS kayıtlarını güncelleştirerek web sitenizi geçerli barındırma sağlayıcınızla koruma

1. Etki Microsoft 365 yönetim merkezi Kurulumu sayfasında gidin ve etki alanları listesinde, web siteniz için  >  [](https://admin.microsoft.com/Adminportal#/Domains) kullanmakta olduğunu etki alanını seçin.

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
