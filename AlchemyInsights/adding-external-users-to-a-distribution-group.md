---
title: Dağıtım grubuna dış Kullanıcı ekleme
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 03cfd2c576cb03cbefd524a4ab6f04e2ef1eebec
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663533"
---
# <a name="add-external-users-to-a-distribution-group"></a>Dağıtım grubuna dış Kullanıcı ekleme

Dağıtım grubuna (DG) dış kişi ekleme iki adımlı bir işlemdir:
  
1. Dış Kullanıcı için posta kişisi oluşturma:
    
    1. Yönetim merkezinde, **Kullanıcılar**  >  [kişiler](https://admin.microsoft.com/adminportal/home#/Contact) sayfasına gidin. 
    
    2. **Kişi ekle**'yi seçin.
    
    3. Kişinizin bilgilerini yazın ve **Ekle**'yi seçin.
    
2. DG 'inize posta kişisi ekleme:
    
    1. Yönetim merkezinde, **gruplar**  >  [gruplar](https://admin.microsoft.com/adminportal/home#/groups) sayfasına gidin. 
    
    2. Dış kullanıcıyı eklemek istediğiniz DG 'yi bulun ve düzenleme iletişim kutusunu açmak için seçin.
    
    3. **Üyeler** sekmesinde, **Tümünü görüntüle ve üyeleri Yönet**'i seçin. 
    
    4. **Üye Ekle**'yi seçin.
    
    5. Önceki adımda oluşturduğunuz posta kişisini seçin ve ardından **Kaydet**'i seçin.
    
Bu adımları uyguladıktan sonra, dış kullanıcılarınız DG 'ye e-posta gönderemezse veya e-posta almadığınızda, DG yalnızca iç kullanıcılardan gelen e-postalara izin verecek şekilde işaretlenmiş olabilir. Bu yapılandırmayı denetleyebilir ve [buradaki](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online)yönergeleri takip edebilirsiniz.
  
 **Not:** Grubunuzun türü "dağıtım grubu" yerine "Microsoft 365 Grubu" olduğunda bu yönergeler uygulanmaz. Bu durumda, dış kullanıcıyı doğrudan gruba ekleyebilirsiniz. Microsoft 365 Groups konuklarına ilişkin ayrıntılı bilgi ve dış konuklar ekleme yönergeleri [Bu makalede](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx)bulunabilir.
  