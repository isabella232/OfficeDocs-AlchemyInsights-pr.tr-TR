---
title: Site bulma
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9143"
- "9005291"
ms.openlocfilehash: bdf94220de45d92f63e56501ea4e35389224d25c
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694554"
---
# <a name="do-site-discovery"></a>Site bulma

Organizasyonunız hala eski web uygulamalarını ve Internet Explorer modunu kullanmayı planlıyorsa (çoğu müşteri bunu kullanıyorsa), bazı ek site keşifleri yapsanız iyi olur.

**Microsoft Edge'in eski bir sürümünü zaten dağıttın**

Kurumsal Site Listenizi Microsoft Edge'in eski sürümüyle çalışacak şekilde zaten yapılandırdıysanız, site bulmanız neredeyse bitti. Tek ihtiyacınız olan nötr siteler eklemektir.

Nötr siteler genellikle çoklu oturum açma (SSO) sağlayan sitelerdir. Microsoft Edge'den nötr bir siteye gidersiniz, kimlik doğrulaması yapmak için Microsoft Edge'de kalmak istersiniz. Internet Explorer modunda nötr bir siteye gidersiniz, kimlik doğrulaması yapmak için Internet Explorer modunda kalmak istersiniz.

Herhangi bir SSO veya diğer nötr siteleri kullanın ve bunları Kurumsal Site Listenize ekleyin.

**Internet Explorer varsayılan tarayıcınızdır**

Şu anda yalnızca Internet Explorer kullanıyorsanız, hangi sitelerin modern web standartlarına yükseltil olduğunu ve hangilerinin hala Internet Explorer'ın gerekli olduğunu bilmiyor olabilirsiniz. Internet Explorer modunu yalnızca bu siteler için kullanasınız diye bu siteleri bulmak ve Kurumsal Site Listesi'ne eklemek istiyor olursunuz.

> [!NOTE]
> [Kurumsal Site Bulma,](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) Internet Explorer modu gerektiren siteler keşfeder. Windows 10, Windows 8.1 veya Windows 7'de Windows Internet Explorer 8 ile Internet Explorer 11 arasında çalışan bilgisayarlarda veri toplayabilirsiniz.

**Verileri çözümleme**

Site verilerini topladikten sonra, verileri çözümlemek için aşağıdaki dört adımlık süreci öneririz:
1. Verileri etki alanına ve ardından URL'ye göre sırala.
2. Internet Explorer modu için yapılandırılan bir uygulamanın sınırlarını tanımlayın. Uygulamayı tanımlayan tüm siteleri ve web denetimlerini eklemek istiyor, ancak fazladan siteler ve denetimler eklemek istemiyorsanız. Bazı siteler aynı şekilde basit *https://contoso.com/app1* olabilir, ancak diğerleri birden çok site ve sayfa tanımlamanız gerektirmektedir.
3. Yerel olarak çalışmay olmadığını doğrulamak için uygulamayı test edin. Birçok site modern bir tarayıcı algılayana kadar modern içerik sağlar ve yalnızca Internet Explorer'ı algılayana kadar eski içerik sağlar.
4. Uygulamayı test başarısız olursa Kurumsal Site Listeniz'e ekleyin.

> [!NOTE]
> En iyi uygulama olarak, uygulamayı oluşturan tüm siteleri grupla. Bu şekilde, bir uygulamayı yükseltken sitenin tamamını Internet Explorer modundan kaldırmak ve bu uygulama için modern bir tarayıcı kullanmaya başlamak daha kolaydır.

Site bulma işi bittiğinde ve verileri analiz ettiyken, kanal stratejinize bakmaya başlamaya hazır oluruz.

