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
ms.openlocfilehash: 824824257fee4aaaab1f2dd32597b4cdc858d035fabd357af90cf054dd35c9c4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54061452"
---
# <a name="sensitivity-labels-not-appearing"></a>Duyarlılık etiketleri görünmüyor

Duyarlılık etiketleri hassas içeriğinizi sınıflandırmanıza ve korumaya yardımcı olmanızı sağlar. Bu etiketler Sınıflandırma ve Duyarlılık Microsoft 365 uyumluluk merkezi, Microsoft 365 merkezi veya Microsoft 365 Güvenlik & Uyumluluk Merkezi'> oluşturulabilir. Bu özellik hakkında daha fazla bilgi edinmek için [bkz. Duyarlılık etiketlerine genel bakış.](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels)

Duyarlılık etiketlerinizi yapılandırdınız ancak bu etiketler Microsoft 365 görünmüyorsa, şunları kontrol edin:

- Duyarlılık etiketinin istediğiniz [kullanıcılara ve](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) gruplara yayım olduğunu onaylayın.

- Kullanıcının duyarlılık etiketlerini destekleyen bir uygulama kullanıyor olduğunu onaylayın- [belgenize duyarlılık etiketlerini bakın](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).

- Azure Information [Protection etiketlerini ediyorsanız,](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)burada listelenen dikkate alınacak noktalara [dikkat edin.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels)

- Veri kaybı önleme (DLP) desteği: Şu anda, DLP ilkelerde koşul olarak yalnızca bekletme etiketleri kullanılabilir.  DLP ilkesinde duyarlılık etiketleri desteği henüz kullanılamıyor ancak bunun üzerinde çalışıyoruz.

- Bir duyarlılık etiketinde şifreleme etkinleştirildiğinde şunları tercih edin:
    - İzinleri şimdi ata
    - Kullanıcıların izin atamasına izin ver


Olası sorunlar hakkında daha fazla bilgi için [bkz. Duyarlılık etiketleriyle ilgili bilinen sorunlar](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).