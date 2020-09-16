---
title: Siteyi veya listeyi şablon olarak kaydetme
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 37ae727aa6dd6af94d0d833ce972aec413d90194
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727551"
---
# <a name="save-site-or-list-as-a-template"></a>Siteyi veya listeyi şablon olarak kaydetme

SharePoint site şablonları, belirli bir iş ihtiyacı etrafında tasarlanmış önceden oluşturulmuş tanımlardır. Daha fazla bilgi için bkz: [şablonları kullanarak farklı türlerde SharePoint siteleri oluşturma](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).

SharePoint Online 'da bir site veya listeyi şablon olarak kaydetme ile ilgili bazı yaygın sorun/çözümleri aşağıda bulabilirsiniz.

**Site/liste şablonunu Kaydet düğmesi kullanılamıyor veya yok**. 

- Yöneticilerin şablon özelliklerini etkinleştirmesi için özel komut dosyasına Izin vermesi gerekir. Ayrıntılı adımlar için, örnekler ve hususlar [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)


- Siteyi şablon olarak Kaydet komutu desteklenmediğinden SharePoint Server yayımlama altyapısını kullanan sitelerde sorunlara neden olabilir.


**Site şablonu oluşturulamıyor veya düzgün çalışmıyor**

- Şablonda bir [özellik](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) eksik olabilir ve etkinleştirilmeyecektir. Özellik geçerli site koleksiyonunda etkinleştirme için kullanılamıyorsa site şablonunu kullanarak site oluşturmaya kullanamazsınız.


- Herhangi bir liste veya kitaplıkta 5000 öğelerinin [liste görünümü sınırı eşiğini](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) aşmadığını denetleyin, bu da bir site şablonunun oluşturulmasını engelleyebilir.


- Site çok fazla kaynak kullanıyor olabilir ve bu nedenle site şablonu 50 megabayt (MB) sınırını aşıyor.


- Arama sütunu kullanan bir listeden verileri görüntülerken sorun çıktı. Daha fazla bilgi için, [şablon tarafından oluşturulan liste, SharePoint Online 'daki doğru arama listesinden verileri görüntülemez](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).


Sık karşılaşılan sorunlar ve çözümler hakkında daha ayrıntılı bilgi için, [site şablonları oluşturma ve kullanma](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)konusuna başvurun.

