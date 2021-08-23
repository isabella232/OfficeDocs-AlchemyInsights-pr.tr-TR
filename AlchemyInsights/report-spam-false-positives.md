---
title: Hatalı pozitif bir istenmeyen postayı Microsoft'a bildirmeniz mi iyi olur?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "975"
- "666"
- "3100019"
ms.openlocfilehash: d3897f24ce9a967b08a3fd15a2fdedbb3fe2a22d
ms.sourcegitcommit: f05d4caa0e657ee74d6b6e9abc88488f17d740fe
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/19/2021
ms.locfileid: "58396635"
---
# <a name="do-you-have-legitimate-messages-being-marked-as-spam"></a>Normal iletileriniz istenmeyen e-posta olarak işaretleniyor mu?

Geçerli bir e-posta gereksiz klasörüne veya Karantina'ya geldiğinde can sıkıcı bir durumdur. Hatalı pozitif sonuçlar için en yaygın nedenleri göz önünde bulundurarak:

**Kiracı geçersiz kılar (en yaygın olan)** Bunu düzeltmek için tamamen sizin denetiminizin içinde.

Etki etkileyen ilkelerin ve kuralların Microsoft 365 Defender için İletiyi İleti'de gönderin; yenidencan ayrıntıları dakika içinde kullanılabilir.
İlkeleri veya kuralları uygun şekilde gözden geçirme veya değiştirme. 

**Son Kullanıcı geçersiz kılmaları (yaygın)** Bunu düzeltmek için tamamen sizin denetiminizin içinde. 

Etki etkileyen ilkelerin ve kuralların Microsoft 365 Defender için İletiyi İleti'de gönderin; yenidencan ayrıntıları dakika içinde kullanılabilir. 

Bir ileti, kullanıcının Engellenen Gönderenler listesinde yer alan bir adresten gönderildiği için engellendiyse, üst bilgiler arasında İstenmeyen Posta Filtreleme Kararını "SFV:BLK" yer alır.

**Gönderenlerin e-posta kimlik doğrulaması** Bunu düzeltmek için kısmen sizin denetiminiz içinde.

Gönderenin e-posta kimlik doğrulamasında teslim sırasındaki hataları çözümlemek için iletiyi gönderin; sonuçları bir gün içinde kullanılabilir. 

Gönderme altyapısı size aitse, hedef e-posta sistemlerinin etki alanınız üzerinden gönderilen iletilere güvene sahip olduğundan emin olmak için onu SPF, DKIM ve DMARC ile nasıl hizalayacağız? gözden geçirebilirsiniz. Alternatif olarak, gönderenlere başvurarak DNS yapılandırmalarını haber velerini gönderebilirsiniz.

**Microsoft filtreleme kararlarını** Bunu düzeltmek için kısmen sizin denetiminiz içinde.

İletiyi gönderin ve iletiyi güvenli olarak rapor gönderin; yenidencan sonuçları bir gün içinde kullanılabilir. Belirli durumlarda filtreleme kararlarını kabul etmezken Kiracı İzin Ver/Engelle Listesini kullanın. Ancak, Microsoft filtreleme kararlarını kalıcı olarak atlamamalı. 

Daha fazla bilgi için bkz.:

- Son kullanıcılarınızı Microsoft'a ileti göndermelerini etkinleştirin. Microsoft, e-posta koruma teknolojilerinin daha etkili olması için bu gönderileri kullanır ve gönderi raporlarında sizin için ilkeleri güncelleştirmenin göstergesi olarak görünür. 

- İletileri çözümleme için göndermeyle ilgili kısa bir video izlemek için [bkz. Çözümleme için ileti gönderme.](https://go.microsoft.com/fwlink/?linkid=2166435)

- [Şüpheli istenmeyen posta, kimlik avı, URL'ler ve dosyaları Microsoft'a göndermek için Yönetici Gönderimi'ni kullanma](https://docs.microsoft.com/microsoft-365/security/office-365-security/admin-submission)

- [Kiracı İzin Ver/Engelleme Listesini Yönetme](https://docs.microsoft.com/microsoft-365/security/office-365-security/tenant-allow-block-list)

- [İletide istenmeyen posta önleme ileti Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spam-message-headers)

- [EOP'de giden istenmeyen posta koruması](https://docs.microsoft.com/microsoft-365/security/office-365-security/outbound-spam-controls)