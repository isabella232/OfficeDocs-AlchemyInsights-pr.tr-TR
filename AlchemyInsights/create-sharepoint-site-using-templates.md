---
title: SharePoint çevrimiçi bir site oluşturmak
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: 9ab06cbd1648da31d8a04e61c237a2326b4bbe93
ms.sourcegitcommit: f856d46a325c517fc29d935c27f21b77c4219e66
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/24/2019
ms.locfileid: "35199293"
---
# <a name="create-sharepoint-sites-using-templates"></a>Şablonları kullanarak SharePoint sitesi oluşturmak

SharePoint site şablonları, belirli bir iş gereksinimini tasarlanmış önceden oluşturulmuş tanımlardır. Daha fazla bilgi için bkz: [farklı türde SharePoint siteleri oluşturmak için şablonları kullanma](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).

İşte bazı yaygın sorunlar/çözümleri kaydetme bir Site veya liste ile ilgili bir şablon olarak Sharepoint çevrimiçi. 

**Site/liste şablonu Kaydet'i eksik veya kullanılabilir değil**

Yöneticiler, şablon özellikleri etkinleştirmek için özel komut dosyasına izin gerekir. Ayrıntılı adımlar için bkz: örnekler ve dikkat edilmesi gereken noktalar 

- [İzin verme veya özel komut dosyası engelleme](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- Şablon komut olarak Kaydet site desteklenmez ve SharePoint Server Yayımlama altyapısını kullanan sitelerde sorunlara neden olabilir.

**Site şablonu oluşturulamıyor veya düzgün çalışmıyor**

Şablon [özelliği](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) eksik ve etkinleştirmeniz gerekmez. Özelliği geçerli site koleksiyonunda etkinleştirmek kullanılabilir değilse, site şablonu site oluşturmak için kullanamazsınız.

- Bu site şablonu oluşturulmasını engelleyebilir gibi herhangi bir liste veya kitaplık 5000 öğeleri [Liste görünümü sınırı eşiği](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) aşarsa denetleyin.

- Site çok fazla kaynak kullanıyor olabilir ve bu nedenle site şablonu 50 MB sınırı aşıyor.


- Arama sütunu kullanan bir listeden veri görüntüleme sorunları vardır. Daha fazla bilgi için bkz: [SharePoint çevrimiçi doğru arama listesinden verileri şablonu tarafından oluşturulan liste görüntülenmeyecek](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).

Yaygın sorunlar ve çözümleri hakkında daha ayrıntılı bilgi için lütfen [site şablonları oluşturma ve kullanma](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)denetleyin.



