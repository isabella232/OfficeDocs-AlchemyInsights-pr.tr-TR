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
ms.openlocfilehash: d2f83b3afc4abf72a3e18bffe5ac9d6c940cc216916925338c18f0fb8a39948a
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/11/2021
ms.locfileid: "57883151"
---
# <a name="outbound-relay-pool"></a>Giden geçiş havuzu

Microsoft, e-postanın geçiş ve iletme için yapılandırmasında bazı değişiklikler Microsoft 365. Bazı senaryolarda iletiler özel bir geçiş havuzu kullanılarak Microsoft 365 bir geçiş havuzu kullanılarak iletilir veya bu havuza geçebilirsiniz. Geçiş havuzu kullanılarak gönderilen iletiler alıcının gereksiz posta klasörüne kadar olabilir. Daha fazla bilgi için [bkz. Giden teslim havuzları](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)

Geçiş havuzunun kullanımıyla ilgili bir senaryodan kaçınmak için, iletili/geçişli iletilerin aşağıdaki ölçütlerden birini karşılaması gerekir:

- Giden gönderen, kiracının kabul edilen etki alanıdır.
- İleti ilk kez geldiğinde Sender Policy Framework (SPF) Microsoft 365.
- P2 gönderen etki alanındaki DomainKeys Identified Mail (DKIM) iletisi, Gelen Microsoft 365.
 
Yukarıdaki ölçütlere uyan iletiler geçiş havuzundan aktarlanmaz.

Etki alanınıza yönelik MX kaydı üçüncü taraf veya şirket içi bir sunucuya işaret ediyorsa, SPF doğrulamanın gelen e-posta için doğru olduğundan ve geçiş havuzu üzerinden e-posta gönderilmesini önlemek için gelişmiş filtrelemeyi kullanın.

**Geçiş havuzunun etkilenmesi ile ilgili durumu nasıl anlarız?**

İletili veya geçişli e-postanız yukarıdaki ölçütlerden birini kullanıyorsa, iletiler geçiş havuzundan aktarıilir. Öte yandan, ileti bir geçiş havuzu üzerinden gönderilirse, giden sunucu IP'si 40.95.0.0/16 aralığındadır ve giden sunucu adı, adlarında **rly** içerir.

