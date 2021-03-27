---
title: Microsoft Edge için uygun gelişmiş kimlik doğrulama kavramları
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003931"
- "6986"
- "8329"
- "9004625"
ms.openlocfilehash: d469973c4f8605b00d32f6f625eb5fdd17e8f390
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398605"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>Microsoft Edge için uygun gelişmiş kimlik doğrulama kavramları

Aşağıda, Microsoft Edge için geçerli olan gelişmiş kimlik doğrulama kavramları ve bilgileri ve bilgileri yermektedir:

**Proaktif Kimlik Doğrulama**

[ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) ilkeyi etkinleştirseniz, Microsoft Edge Microsoft hizmetleri aracılığıyla oturum açık kullanıcıların önceden kimlik doğrulamasını yapmaya çalışır. Düzenli aralıklarla, Proaktif Kimlik Doğrulaması'nın geçerli olduğu yapılandırmayı içeren güncelleştirilmiş bir bildirim olup denetlemesi için çevrimiçi bir hizmet kullanır.

Avantajlar: Proaktif Kimlik Doğrulama, Office Yeni Sekme Sayfası gibi önemli hizmetlerde kimlik doğrulamayı sağlar. Ayrıca, Bing arama motoru olarak kullanılıyorsa, Proaktif Kimlik Doğrulama adres çubuğunun performansını artırır ve işletmenizin ihtiyaçlarına göre kişiselleştirilmiş arama sonuçları üretmeye yardımcı olur.

**NTLM Kimlik Doğrulaması için Windows Hello CredUI**

Bir web sitesi NTLM veya Görüşme mekanizması aracılığıyla kullanıcıda oturum açmaya çalıştığında çoklu oturum açma (SSO) kullanılamıyorsa, bu özellik kullanıcının işletim sistemi kimlik bilgilerini web sitesiyle paylaşmasına ve Windows Hello Cred UI kullanarak kimlik doğrulama zorluklarını karşılamasına olanak sağlar. Bu oturum açma akışı yalnızca Windows 10'da ve yalnızca NTLM veya Görüşme sırasında SSO almayan kullanıcılar için görüntülenir.

**Kaydedilen parolaları kullanarak otomatik olarak oturum açma**

Microsoft Edge'de parolaları kaydeden kullanıcılar, kimlik bilgilerini kaydettilen web sitelerinde otomatik olarak oturum açma özelliğini etkinleştirebilirsiniz. Kullanıcılar bu özelliği aynı edge://settings/passwords veya devre dışı bırakır ve parola yöneticisi ilkelerde [yapılandırabilirsiniz.](https://go.microsoft.com/fwlink/?linkid=2134622)
