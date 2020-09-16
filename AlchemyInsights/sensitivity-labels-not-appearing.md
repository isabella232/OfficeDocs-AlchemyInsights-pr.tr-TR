---
title: Duyarlılık etiketleri görünmüyor
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 6a64e001be115c8e5553a0d8c97b8cb815922c69
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801204"
---
# <a name="sensitivity-labels-not-appearing"></a>Duyarlılık etiketleri görünmüyor

Duyarlılık etiketleri hassas içeriğinizi sınıflandırmanıza ve korunmanıza olanak tanır. Microsoft 365 Uyumluluk Merkezi, Microsoft 365 güvenlik merkezi veya Microsoft 365 güvenlik & Uyumluluk Merkezi 'nde sınıflandırma > duyarlılık etiketleri altında oluşturulabilir. Bu özellik hakkında daha fazla bilgi edinmek için [duyarlılık etiketlerine genel bakış](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels)konusuna bakın.

Duyarlılık etiketlerinizi yapılandırdıysanız ancak Microsoft 365 uygulamalarında görünmüyorsa, aşağıdakileri denetleyin:

- Duyarlılık etiketinin, istediğiniz kullanıcı ve gruplara [yayımlandığını](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) doğrulayın.

- Kullanıcının, duyarlılık etiketlerini destekleyen bir uygulamayı kullandığını doğrulayın- [belgenizdeki duyarlılık etiketlerine](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable)bakın.

- [Azure Information Protection etiketlerini geçiriyorsanız](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), [burada](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels)listelenen dikkat edilmesi gereken noktaları göz önünde bulundurun.

- Veri kaybı önleme (DLP) desteği: şimdilik yalnızca bekletme etiketleri DLP ilkelerinde bir koşul olarak kullanılabilir.  DLP ilkesindeki duyarlılık etiketleri desteği henüz kullanılamaz, ancak üzerinde çalışıyoruz.

- Duyarlılık etiketinde şifreleme etkinleştirildiğinde şunları yapabilirsiniz:
    - İzinleri şimdi ata
    - Kullanıcıların izin atamasına izin verme


Olası sorunlar hakkında daha fazla bilgi için [duyarlılık etiketleriyle Ilgili bilinen sorunlar](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc)konusuna bakın.