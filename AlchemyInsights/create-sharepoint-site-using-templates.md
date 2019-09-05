---
title: SharePoint Online'da site oluşturma
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: 42430c8dadc17b87dc7741f3fa045ba7c25fab84
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36755328"
---
# <a name="create-sharepoint-sites-using-templates"></a>Şablonları kullanarak SharePoint siteleri oluşturma

SharePoint site şablonları, belirli bir iş gereksinimi etrafında tasarlanmış önceden oluşturulmuş tanımlardır. Daha fazla bilgi için bkz. [Farklı SharePoint siteleri oluşturmak için şablonları kullanma.](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4)

Sharepoint Online'da bir Siteyi veya Listeyi şablon olarak kaydetmeyle ilgili bazı sık karşılaşılan sorunlar/çözümler aşağıda verilmiştir. 

**Site/liste şablonu kaydet düğmesi kullanılamıyor veya eksik**

Yöneticilerin şablon özelliklerini etkinleştirmek için Özel Komut Dosyasına İzin Vermeleri gerekir. Ayrıntılı adımlar, örnekler ve hususlar için bkz. 

- [Özel komut dosyasına izin verme veya engelleme](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- Şablon komutu olarak kaydet sitesi desteklenmez ve SharePoint Server Yayımlama Altyapısını kullanan sitelerde sorunlara neden olabilir.

**Site şablonu oluşturulamıyor veya doğru çalışmıyor**

Şablon bir [özellik](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) eksik olabilir ve etkinleştirilmez. Özellik geçerli site koleksiyonunda etkinleştirmek için kullanılamıyorsa, site şablonunu bir site oluşturmak için kullanamazsınız.

- Herhangi bir liste veya kitaplık, bir site şablonunun oluşturulmasını engelleyebilir gibi 5000 öğe liste [görünümü sınır eşiği](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) aşAbilir olup olmadığını görmek için denetleyin.

- Site çok fazla kaynak kullanıyor olabilir ve bu nedenle site şablonu 50 MB sınırını aşıyor.


- Arama sütunu kullanan bir listeden veri görüntülemede sorunlar vardır. Daha fazla bilgi için bkz: [Şablon tarafından oluşturulan liste SharePoint Online'da doğru arama listesinden veri görüntülemiyor.](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data)

Sık karşılaşılan sorunlar ve çözümler hakkında daha ayrıntılı bilgi için lütfen [site şablonları oluştur ve bunları kullanın.](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)



