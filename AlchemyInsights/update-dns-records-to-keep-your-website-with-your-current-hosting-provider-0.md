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
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: a1ea0589def4945da64c73d68b2e4a3d64d6b83d
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36506427"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>DNS kayıtlarını güncelleştirerek web sitenizi geçerli barındırma sağlayıcınızla koruma

1. [Etki alanları](https://portal.office.com/adminportal/home#/Domains) sayfasında, Web siteniz için kullandığınız etki alanı, etki alanı listesinde seçin.

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
