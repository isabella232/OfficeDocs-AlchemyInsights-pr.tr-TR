---
title: Web üzerinde Outlook'ta S/MIME
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: bef87baafdbaf9346f99f1ff54aaa83bc9173c70f1412ea00afb717c15a8014c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54010744"
---
# <a name="encrypt-email-messages-in-outlook"></a>E-posta iletilerini Outlook

Microsoft 365 İleti Şifrelemesi, Azure Microsoft Azure Koruması'nın bir parçası olan Güvenlik Hakları Yönetimi (Azure RMS) üzerine kurulur. Aboneliğiniz Azure Hak Yönetimi'ne veya Azure Information **Protection'a** sahipse, Hak Yönetimi Hizmetini el ile etkinleştirmek veya etkinleştirmek için herhangi bir işlem yapmaya gerek yok.

Müşteri geri bildirimlerine bağlı olarak, artık kiracınız için varsayılan Exchange tür hassas bilgiler içeren giden e-postaları otomatik olarak şifrelemek için posta akışı kurallarını etkinleştirmemiz gerekmeyecek. Bunun yerine, kendiniz kendiniz yapmak için ayrıntılı yönergeler sağlıyoruz. Hassas bilgileri şifrelemek üzere aktarım kuralı oluşturma hakkında ek ayrıntılar için bu [makaleye bakın.](https://aka.ms/OmeEtr)

- Web'Outlook Posta Sunucusu kullanıyorsanız (eski adı **OWA):** E-posta iletisi oluşturmak için OWA'da **Koru'ya** tıklamanız gerekir. Bu, "İtema" iznini uygulanır. İzni **değiştir'e** tıklayın ve yalnızca **iletiyi** şifrelemek için Şifrele'yi seçin.

- Outlook **istemcisi** kullanıyorsanız: Outlook 2013 veya 2016'dan şifrelenmiş ileti göndermek için Mac için Outlook 2016, Seçenekler İzinleri'ne tıklayın ve ardından ihtiyacınız olan koruma  >  seçeneğini belirtin.

- Belirli **alıcılara veya dış** iş ortağı kuruluşlara gönderilen tüm e-postaları otomatik olarak şifrelemek için, Yönetim Merkezi'nde bir posta akışı aktarım Exchange gerekir. Bu destek makalesinde [ayrıntılı yönergeler sağlanmaktadır.](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities)

