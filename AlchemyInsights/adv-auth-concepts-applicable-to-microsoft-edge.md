---
title: Kullanıcılar için geçerli gelişmiş kimlik Microsoft Edge
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
ms.openlocfilehash: 8ddec37260ec4e3bcc390dcc8adb7397368de19555ee31be458be033d3886386
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934385"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>Kullanıcılar için geçerli gelişmiş kimlik Microsoft Edge

Aşağıdakiler, kimlik doğrulaması için geçerli olan gelişmiş kimlik Microsoft Edge:

**Proactive Authentication**

[ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) Microsoft Edge etkinleştirseniz, Microsoft Edge kimlik doğrulaması yapmak için önceden oturum kullanan kullanıcıların kimliğini doğrulamayı Microsoft hizmetleri. Düzenli aralıklarla, Proaktif Kimlik Doğrulaması'nda geçerli olan yapılandırmayı içeren güncelleştirilmiş bir bildirimi kontrol etmek için çevrimiçi bir hizmet kullanır.

Avantajlar: Proaktif Kimlik Doğrulaması, Yeni Sekme Sayfası gibi önemli hizmetlerde Office sağlar. Ayrıca, arama Bing olarak kullanılan Proaktif Kimlik Doğrulama, adres çubuğunun performansını artırır ve işletmenizin ihtiyaçlarına göre kişiselleştirilmiş arama sonuçları üretmeye yardımcı olur.

**Windows Hello NTLM Kimlik Doğrulaması için CredUI**

Bir web sitesi NTLM veya Görüşme mekanizması aracılığıyla kullanıcıda oturum açmaya çalıştığında çoklu oturum açma (SSO) yoksa, bu özellik kullanıcının işletim sistemi kimlik bilgilerini web sitesiyle paylaşmasına ve Windows Hello Cred UI kullanarak kimlik doğrulama zorluklarını karşılamasına olanak verir. Bu oturum açma akışı yalnızca Windows 10'de görüntülenir ve yalnızca NTLM sırasında SSO'ya veya Görüşme sırasında SSO'ya sahip olmayan kullanıcılara görünür.

**Kaydedilmiş parolaları kullanarak otomatik olarak oturum açma**

Parolaları web sitelerine Microsoft Edge, kimlik bilgilerini kaydettilen web sitelerinde otomatik olarak oturum açma özelliğini etkinleştirebilirsiniz. Kullanıcılar bu özelliği e-posta edge://settings/passwords ve parola yöneticisi ilkesinde [yapılandırabilirsiniz.](https://go.microsoft.com/fwlink/?linkid=2134622)
