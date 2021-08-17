---
title: Otomatik olarak oturum Microsoft Edge açma
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
- "8333"
- "9004625"
ms.openlocfilehash: 4e069a1c75caabf3bef7387140edd5650cf966856b888b5c6b5618a603986d6d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54050714"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Otomatik olarak oturum Microsoft Edge açma

Microsoft Edge, kullanıcının aygıtının nasıl yapılandırıldığuna göre otomatik olarak kullanıcıda oturum açması için işletim sistemi varsayılan hesabını kullanır. 

Cihaz yapılandırmasının her türüyle bağımlı kullanıcı oturum açma işleminin senaryoları aşağıda açıklanmıştır:

- **Cihaz karma/AAD-J'tir:** Bu seçenek Windows 10, alt Windows ve buna karşılık gelen sunucu sürümlerinde kullanılabilir. Kullanıcılar kendi hesap hesaplarıyla (AD) Azure Active Directory otomatik olarak oturum açılır.
- **Cihaz etki alanına katılmış durumdadır**: Bu seçenek Windows 10, alt düzey Windows ve buna karşılık gelen sunucu sürümlerinde kullanılabilir. Varsayılan olarak, etki alanı hesabı olan kullanıcılar otomatik olarak oturum alanmaz; onlar için otomatik oturum açma özelliğini etkinleştirmek için **ConfigureOnPremisesAccountAutoSignIn İlkesini** kullanın. Azure AD hesapları olan kullanıcılarda otomatik oturum açma özelliğini etkinleştirmek için cihazlarına karma birleştirmeyi göz önünde bulundurabilirsiniz.
- **Işletim sistemi** varsayılan hesabı bir Microsoft hesabıdır: Bu seçenek Windows 10 RS3 (sürüm 1709, derleme 10.0.16299) ve sonraki sürümlerinde kullanılabilir. Senaryonun kurumsal cihazlarda gerçekleşmesi olası değildir. Öte yandan, işletim sistemi varsayılan hesabı bir Microsoft hesabı ise, Microsoft Edge otomatik olarak kullanıcının Microsoft hesabıyla oturum açmasını sağlar.
 
 
