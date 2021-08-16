---
title: Site bulma yapma
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
ms.openlocfilehash: 4653fdef7e9226f05809d56e9a445cd1da35b0578c088bea72252a281d4527d2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54030778"
---
# <a name="do-site-discovery"></a>Site bulma yapma

Kuruluşta hala eski web uygulamaları ve Internet Explorer modunu kullanmayı planlıyorsa (çoğu müşteri bunu kullanıyorsa), bazı ek site keşifleri yapsanız iyi olur.

**Uygulamanın eski bir sürümünü zaten dağıtmış Microsoft Edge**

Enterprise Site Listenizi Microsoft Edge'in eski sürümü için çalışacak şekilde yapılandırdıysanız, site bulma işi neredeyse bitti. Nötr siteleri eklemeniz gerekmektedir.

Tarafsız siteler genellikle çoklu oturum açma (SSO) sağlayan sitelerdir. Birden fazla siteden nötr bir Microsoft Edge gidersanız, kimlik doğrulaması yapmak için Microsoft Edge kalmak gerekir. Internet Explorer modunda nötr bir siteye gidersanız, kimlik doğrulaması için Internet Explorer modunda kalmak istediğiniz olur.

Tüm SSO veya diğer nötr siteleri tanımlamak ve bunları kendi Site Listenize Enterprise eklemek.

**Internet Explorer varsayılan tarayıcınızdır**

Şu anda yalnızca Internet Explorer kullanıyorsanız, hangi sitelerin modern web standartlarına yükseltme olduğunu ve hangisinin hala Internet Explorer gerektirir olduğunu bilmiyor olabilir. Internet Explorer modunu yalnızca bu siteler için kullanasınız Enterprise bu siteleri bulmak ve bu sitelere eklemek istiyor olursunuz.

> [!NOTE]
> [Enterprise Bulma,](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) Internet Explorer modu gerekten siteleri keşfeder. Windows 10, Windows 8.1 veya Windows 7 üzerinde Internet Explorer 8 ile Internet Explorer 11 Windows 10 çalıştıran bilgisayarlarda Windows toplayabilirsiniz. Windows

**Verileri çözümleme**

Site verilerini topdikten sonra, verileri çözümlemek için aşağıdaki dört adımlık işlemi öneririz:
1. Verileri etki alanına ve ardından URL'ye göre sırala.
2. Internet Explorer modu için yapılandırmak üzere uygulamanın sınırlarını tanımlayın. Uygulamayı tanımlayan tüm siteleri ve web denetimlerini eklemek istiyor, ancak fazladan siteler ve denetimler eklemek istemiyorsanız. Bazı siteler sizin birden çok site ve *https://contoso.com/app1* sayfa tanımlamanız gerektirsin diye basit olabilir.
3. Yerel olarak çalışma çalıştığını doğrulamak için uygulamayı test edin. Birçok site, modern bir tarayıcı algılayana kadar modern içerik sağlar ve yalnızca Internet Explorer'ı algılayana kadar eski içeriği sağlar.
4. Uygulamayı test Enterprise Site Listeniz'e ekleyin.

> [!NOTE]
> En iyi uygulama olarak, bir uygulamayı oluşturan sitelerin hepsini gruplayın. Bu şekilde, uygulamayı yükselttirken sitenin tamamını Internet Explorer modundan kaldırmak ve bu uygulama için modern bir tarayıcı kullanmaya başlamak daha kolay olur.

Site bulma ile ilgili çalışmanız bittiğinde ve verileri çözümle hazır olduktan sonra, kanal stratejinizi incelemeye başlamaya hazır oluruz.

