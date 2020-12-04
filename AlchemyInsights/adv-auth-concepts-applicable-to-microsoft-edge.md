---
title: Microsoft Edge için geçerli olan gelişmiş kimlik doğrulama kavramları
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
ms.openlocfilehash: 241d594fac6664dd1e85fd60e30a6344c432555e
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573780"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>Microsoft Edge için geçerli olan gelişmiş kimlik doğrulama kavramları

Microsoft Edge için geçerli olan gelişmiş kimlik doğrulama kavramları aşağıda verilmiştir:

**Önleyici kimlik doğrulama**

[Proactiveauthenabled](https://go.microsoft.com/fwlink/?linkid=2134621) ilkesini etkinleştirdiğinizde, Microsoft Edge, oturumu açık kullanıcılarla Microsoft hizmetlerini kullanarak kimlik doğrulama yapmayı dener. Düzenli aralıklarla, önleyici kimlik doğrulamayı yöneten yapılandırmayı içeren güncelleştirilmiş bir bildirimi denetlemek için bir çevrimiçi hizmet kullanacaktır.

Yararlar: önleyici kimlik doğrulaması, Office yeni sekme sayfası gibi temel hizmetlerin kimlik doğrulamasını sağlar. Ayrıca, Bing arama altyapısı olarak kullanılırsa, önleyici kimlik doğrulaması, adres çubuğunun performansını artırır ve işinizin ihtiyaçlarına göre kişiselleştirilmiş arama sonuçlarının oluşturulmasına yardımcı olur.

**NTLM kimlik doğrulaması için Windows Hello Creduı**

Web sitesi NTLM veya anlaşma mekanizması aracılığıyla Kullanıcı oturum açmaya çalıştığında çoklu oturum açma (SSO) kullanılamıyorsa, bu özellik kullanıcının işletim sistemi kimlik bilgilerini Web sitesiyle paylaşmasına ve Windows Hello Credentials Kullanıcı arabirimini kullanarak kimlik doğrulama sınamasını sağlamasına olanak tanır. Bu oturum açma akışı yalnızca Windows 10 ' da, yalnızca NTLM veya anlaşma sırasında SSO kullanmayan kullanıcılar için görünür.

**Otomatik olarak oturum açmak için kaydedilmiş parolaları kullanma**

Microsoft Edge 'de parolaları kaydeden kullanıcılar, kimlik bilgilerini kaydetdikleri web sitelerinde otomatik oturum açmayı etkinleştirebilirler. Kullanıcılar edge://settings/passwords 'da bu özelliği açıp kapatabilir ve bunu [Parola Yöneticisi](https://go.microsoft.com/fwlink/?linkid=2134622) ilkelerinde yapılandırabilirsiniz.
