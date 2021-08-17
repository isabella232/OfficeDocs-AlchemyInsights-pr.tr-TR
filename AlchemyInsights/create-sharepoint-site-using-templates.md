---
title: SharePoint Online'da site oluşturma
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
ms.openlocfilehash: eaf09aebad5568aab3a716ce28c8ce3357c9f43175e1b1458bfcd43fd95a71fa
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54057986"
---
# <a name="create-sharepoint-sites-using-templates"></a>Şablonları SharePoint site oluşturma

Siteyi şablon olarak kaydetme özelliği, modern İletişim veya Ekip Siteleri ile desteklanmaz. Şablonları kullanma hakkında daha fazla bilgi için bkz. SharePoint [sitesini şablon olarak kaydetme, indirme ve karşıya yükleme.](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template)

Burada, Bir Siteyi veya Listeyi SharePoint Online'da şablon olarak kaydetmeyle ilgili bazı yaygın sorunlar/çözümler bulabilirsiniz. 

**Site/liste şablonu kaydet düğmesi kullanılamıyor veya eksik**

Yöneticilerin şablon özelliklerini etkinleştirmek için Özel Betiklere İzin Vermeleri gerekir. Ayrıntılı adımlar, örnekler ve dikkate alınacak noktalar için bkz. 

- [Özel betiklere izin verme veya engelleme](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- Siteyi şablon olarak kaydet komutu desteklenmiyor ve SharePoint Server Yayımlama Altyapısı kullanan sitelerde sorunlara neden olabilir.

**Site şablonu oluşturulamıyor veya düzgün çalışmıyor**

Şablonda bir özellik [eksik olabilir](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) ve etkinleştirmez. Özellik geçerli site koleksiyonunda etkinleştirilene kadar kullanılamıyorsa, site şablonunu kullanarak site oluşturamazsınız.

- Liste veya kitaplıklardan herhangi biri [](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) 5000 öğelik Liste Görünümü Sınırı Eşiği'nin aşıp geçmemektedir, çünkü bu, site şablonu oluşturulmasını engelleyebilir.

- Site çok fazla kaynak kullanıyor ve dolayısıyla site şablonu 50 MB sınırını aşıyor olabilir.


- Arama sütunu kullanan bir listeden verileri görüntülerken sorun vardır. Daha fazla bilgi için bkz. Şablon tarafından oluşturulan liste [SharePoint Online'da doğru arama listesinden verileri görüntüley çalışmıyor.](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data)

Sık karşılaşılan sorunlar ve çözümler hakkında daha ayrıntılı bilgi için, lütfen Site şablonları [oluşturma ve kullanma kutusunu kontrol edin.](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)



