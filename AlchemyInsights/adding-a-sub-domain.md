---
title: Alt etki alanı ekleme
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
- "7"
- "13902"
ms.openlocfilehash: ea39984a54a15ae6167363eb5855943c8ab1120d
ms.sourcegitcommit: a097d1f8915a31ed8460b5b68dccc8d87e563cc0
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/22/2021
ms.locfileid: "59506767"
---
# <a name="adding-a-sub-domain"></a>Alt etki alanı ekleme

Alt etki alanları, üst etki alanıyla aynı veya farklı bir kiracıya eklenebilir. Her iki durumda da kayıt şirketinizin web sitesinde kendi DNS ayarlarınızı yönetmeniz gerekir. DNS ayarlarınızı NS kayıtlarında Microsoft'un yönetmesine izin verdiysanız veya etki alanını Microsoft'tan satın aldıysanız, önce bunu değiştirmeden alt etki alanları ekeyebilirsiniz.

Önce üst etki alanını ekleyin ve ardından alt etki alanını ekleyin. Alt etki alanı aynı kiracıda yer alan bir etki alanı varsa, başka doğrulama gerekmez. Alt etki alanını ayrı bir kiracıya ekliyorsanız, etki alanını ve seçilen hizmetler için ek DNS kayıtlarını eklemeden önce DNS txt kaydı sahipliği doğrulaması gerekir.

- Etki alanı veya alt etki alanı [](https://admin.microsoft.com/Adminportal#/Domains/Wizard)eklemek için, Etki Alanı Ekle sihirbazını izleyin veya Etki Alanı Ekle'yi ayarla'ya gidip etki alanını veya alt etki alanını el  >    >  **ile ekleyin.**

Gerekirse:

- Mevcut bir etki alanı için DNS ayarlarınızı kimin yönetileceğini değiştirmek için Etki Alanları'Ayarlar gidin, etki alanının yanındaki onay kutusunu seçin ve  >  [](https://admin.microsoft.com/Adminportal/Home#/Domains)ardından DNS'yi Yönet **öğesini seçin.** Sihirbazda Kendi **DNS kayıtlarınızı ekleyin'i seçin** ve sihirbazı tamamlayın.
- Microsoft tarafından satın alınan bir etki alanına alt etki alanları eklemek için, önce etki alanını başka bir kayıt şirketine aktarın ve ardından kendi DNS kayıtlarınızı yönetmek için yukarıdaki değişikliği seçin. Yönergeler için bkz. [Etki alanını Microsoft'tan başka bir ana bilgisayara aktarma.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host)
- Etki alanınız zaten kuruluşta diğer üyeler veya kişiler tarafından kullanmakta olduğu hatasını alırsanız, etki alanını kullanmadan önce bu yönetim dışı hesabın hesabını sizinmiş olun. Yönergeler için [bkz. Azure Active Directory'de](https://docs.microsoft.com/azure/active-directory/enterprise-users/domains-admin-takeover)yönetici olarak yönetimi olmayan bir dizini Azure Active Directory.
