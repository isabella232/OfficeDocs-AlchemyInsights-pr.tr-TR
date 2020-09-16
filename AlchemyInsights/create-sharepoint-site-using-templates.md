---
title: SharePoint Online 'da site oluşturma
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: b554bfa4ccccbd68d0c3df27cf17397f860735c2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732264"
---
# <a name="create-sharepoint-sites-using-templates"></a>Şablonları kullanarak SharePoint siteleri oluşturma

Siteyi şablon olarak kaydetme özelliği modern Iletişimde veya ekip sitelerinde desteklenmez. Şablonları kullanma hakkında daha fazla bilgi için [, SharePoint sitesini şablon olarak kaydetme, indirme ve karşıya yükleme](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template)bölümüne bakın.

SharePoint Online 'da bir site veya listeyi şablon olarak kaydetme ile ilgili bazı yaygın sorun/çözümleri aşağıda bulabilirsiniz. 

**Site/liste şablonunu Kaydet düğmesi kullanılamıyor veya yok**

Yöneticilerin şablon özelliklerini etkinleştirmesi için özel komut dosyasına Izin vermesi gerekir. Ayrıntılı adımlar için, örnekler ve hususlar 

- [Özel Betik](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- Siteyi şablon olarak Kaydet komutu desteklenmediğinden SharePoint Server yayımlama altyapısını kullanan sitelerde sorunlara neden olabilir.

**Site şablonu oluşturulamıyor veya düzgün çalışmıyor**

Şablonda bir [özellik](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) eksik olabilir ve etkinleştirilmeyecektir. Özellik geçerli site koleksiyonunda etkinleştirme için kullanılamıyorsa site şablonunu kullanarak site oluşturmaya kullanamazsınız.

- Herhangi bir liste veya kitaplıkta 5000 öğelerinin [liste görünümü sınırı eşiğini](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) aşmadığını denetleyin, bu da bir site şablonunun oluşturulmasını engelleyebilir.

- Site çok fazla kaynak kullanıyor olabilir ve bu nedenle site şablonu 50 MB sınırını aşıyor.


- Arama sütunu kullanan bir listeden verileri görüntülerken sorun çıktı. Daha fazla bilgi için, [şablon tarafından oluşturulan liste, SharePoint Online 'daki doğru arama listesinden verileri görüntülemez](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).

Sık karşılaşılan sorunlar ve çözümleri hakkında daha ayrıntılı bilgi için lütfen [site şablonlarını oluşturma ve kullanma](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)seçeneğini işaretleyin.



