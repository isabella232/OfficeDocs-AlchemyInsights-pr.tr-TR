---
title: Microsoft Edge 'de otomatik olarak oturum açma
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003848"
- "6898"
ms.openlocfilehash: 68a1119abd0a3f687b6448bb6e58c6485c239c0f
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/08/2020
ms.locfileid: "49678819"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Microsoft Edge 'de otomatik olarak oturum açma

Microsoft Edge, kullanıcının cihazının nasıl yapılandırıldığına bağlı olarak bir kullanıcı için işletim sisteminin varsayılan hesabını kullanır. 

Her cihaz yapılandırması türünün senaryoları ve bağımlı Kullanıcı oturum açma süreci aşağıda açıklanmıştır:

1. **Cihaz karma/AAD-J**: Bu seçenek Windows 10, alt düzey Windows ve ilgili sunucu sürümlerinde kullanılabilir. Kullanıcılar Azure Active Directory (AD) hesaplarıyla otomatik olarak imzalanır.
2. **Cihaz etki alanına bağlı**: Bu seçenek Windows 10, alt düzey Windows ve ilgili sunucu sürümlerinde kullanılabilir. Varsayılan olarak, etki alanı hesabı olan kullanıcılar otomatik olarak imzalanır; otomatik oturum açmayı etkinleştirmek için **ConfigureOnPremisesAccountAutoSignIn** ilkesini kullanın. Azure AD hesapları olan kullanıcılar için otomatik oturum açmayı etkinleştirmek üzere, onlara karma olarak katılma seçeneğini dikkate alın.
3. **İşletim sisteminin varsayılan hesabı bir Microsoft hesabıdır**: Bu seçenek WINDOWS 10 yalnızca RS3 (sürüm 1709, derleme 10.0.16299) ve sonraki sürümlerde kullanılabilir. Senaryo kurumsal cihazlarda gerçekleşmiyor olabilir. Ancak, işletim sisteminin varsayılan hesabı bir Microsoft hesabındanda, Microsoft Edge kullanıcının Microsoft hesabıyla otomatik olarak oturum açmasını sağlayacaktır.
 
 
