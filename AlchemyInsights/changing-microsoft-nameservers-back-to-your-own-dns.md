---
title: Microsoft ad sunucularından kendi DNS kayıtlarınızı yönetmeye geri dönme
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13988"
- "14"
ms.openlocfilehash: a228bcda1220011ab994de7aa70f19ea092e2142
ms.sourcegitcommit: e9e282be4997b0ee95f1ff4491e0943f8fc52444
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/22/2021
ms.locfileid: "59506976"
---
# <a name="changing-from-microsoft-nameservers-back-to-managing-your-own-dns-records"></a>Microsoft ad sunucularından kendi DNS kayıtlarınızı yönetmeye geri dönme

NS kayıtlarınızı daha önce Microsoft'a (ns1.bdm.microsoftonline.com) işaret olacak şekilde değiştirdiniz, ancak şimdi KENDI DNS kayıtlarınızı yönetmeye karar vermişsinizdir:

Etki alanı kayıt şirketinizin web sitesinde, ad sunucusu yerine kayıt şirketinize veya önceki ayarına geri gidin. DNS konusunu iyi bilmiyorsanız, etki alanı kayıt şirketinin desteğine başvurun. Ad sunucusu değişikliklerinin yayılması 48 saat kadar sürebilir. 

1. Microsoft 365 portalında Etki **Alanları'Ayarlar** gidin, etki alanının yanındaki onay kutusunu seçin ve  >  [](https://admin.microsoft.com/Adminportal/Home#/Domains)DNS'yi Yönet **öğesini seçin.** 

2. Sihirbazda Kendi **DNS kayıtlarınızı ekleyin'i seçin** ve sihirbazı tamamlayın. Bu, DNS'nizin nasıl yönetileceğini değiştirir ve seçili hizmetlerinizi desteklemek için gereken özel DNS kayıtlarını eklemenize olanak sağlar.

Alternatif olarak, ad sunucusu kayıtlarınızı Microsoft olarak değiştirdiysiniz ve bir web siteniz varsa, ad sunucularını geri değiştirmek yerine web sitesi için DNS kayıtları eklersiniz. Daha fazla bilgi için [bkz. DNS kayıtlarını güncelleştirin ve web sitenizi geçerli barındırma sağlayıcınızla birlikte kullanın.](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)


