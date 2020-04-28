---
title: Dağıtım Grubuna harici kullanıcı ekleme
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 7dbc69bced9ca800d3f95081b77dda5e49662579
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/27/2020
ms.locfileid: "43910952"
---
# <a name="add-external-users-to-a-distribution-group"></a>Dağıtım Grubuna harici kullanıcı ekleme

Dağıtım Grubuna (DG) harici bir bağlantı eklemek iki adımlı bir işlemdir:
  
1. Harici kullanıcı için Bir Posta İlgili Kişisi Oluşturun:
    
    1. Yönetici merkezinde, **Kullanıcılar** > [Kişileri](https://admin.microsoft.com/adminportal/home#/Contact) sayfasına gidin. 
    
    2. **Kişi ekle'yi**seçin.
    
    3. İlgili kişinizin bilgilerini yazın ve **Ekle'yi**seçin.
    
2. Posta İlgili Kişisini DG'nize ekleyin:
    
    1. Yönetici merkezinde Gruplar **sayfasına** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) gidin. 
    
    2. Dış kullanıcıeklemek istediğiniz DG'yi bulun ve edit iletişim kutusunu açmak için seçin.
    
    3. **Üyeler** sekmesinde, **Tümünü Görüntüle'yi ve üyeleri yönet'i**seçin. 
    
    4. **Üye Ekle'yi**seçin.
    
    5. Önceki adımda oluşturduğunuz Posta İlgili Kişisini seçin ve ardından **Kaydet'i**seçin.
    
Bu adımları izleyerek dış kullanıcılarınız DG'ye e-posta gönderemezse veya ondan e-posta alamıyorsa, DG yalnızca dahili kullanıcılardan gelen e-postalara izin verecek şekilde işaretlenmiş olabilir. Bu yapılandırmayı kontrol edebilir ve [burada](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online)yönergeleri izleyerek düzeltebilirsiniz.
  
 **Not:** Grubunuzun türü "Dağıtım grubu" yerine "Microsoft 365 grubu" ise bu talimatlar geçerli değildir. Bu durumda, dış kullanıcıyı doğrudan Outlook'tan gruba ekleyebilirsiniz. Microsoft 365 Grupları konukları hakkında ayrıntılı bilgi nin yanı sıra harici misafir ekleme [talimatlarına da bu makalede](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx)yer bulabilirsiniz.
  