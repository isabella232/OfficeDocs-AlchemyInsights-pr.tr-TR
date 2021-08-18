---
title: Giden geçiş havuzu
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/08/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "12315"
ms.openlocfilehash: 7e5bb1fda1dec0c0f72d1944d54b6f2747a6e909
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326097"
---
# <a name="outbound-relay-pool"></a>Giden geçiş havuzu

Microsoft, e-postanın geçiş ve iletme için yapılandırmasında bazı değişiklikler Microsoft 365. Bazı senaryolarda iletiler, özel bir geçiş havuzu kullanılarak Microsoft 365 bir geçiş havuzu kullanılarak iletilir veya bu havuza geçebilirsiniz. Geçiş havuzu kullanılarak gönderilen iletiler alıcının gereksiz posta klasörüne kadar olabilir. Daha fazla bilgi için [bkz. Giden teslim havuzları](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)

Geçiş havuzunun kullanımıyla ilgili bir senaryodan kaçınmak için, iletili/geçişli iletilerin aşağıdaki ölçütlerden birini karşılaması gerekir:

- Giden gönderen, kiracının kabul edilen etki alanıdır.
- İleti ilk kez geldiğinde Sender Policy Framework (SPF) Microsoft 365.
- P2 gönderen etki alanındaki DomainKeys Identified Mail (DKIM) iletisi, Gelen Microsoft 365.
 
Yukarıdaki ölçütlere uyan iletiler geçiş havuzundan aktarlanmaz.

Etki alanınıza yönelik MX kaydı üçüncü taraf veya şirket içi bir sunucuya işaret ediyorsa, SPF doğrulamanın gelen e-posta için doğru olduğundan ve geçiş havuzu üzerinden e-posta gönderilmesini önlemek için gelişmiş filtrelemeyi kullanın.

**Geçiş havuzunun etkilenmesi ile ilgili durumu nasıl anlarız?**

İletili veya geçişli e-postanız yukarıdaki ölçütlerden birini kullanıyorsa, iletiler geçiş havuzundan aktarıilir. Öte yandan, ileti bir geçiş havuzu üzerinden gönderilirse, giden sunucu IP'si 40.95.0.0/16 aralığındadır ve giden sunucu adı **rly** içerir.

