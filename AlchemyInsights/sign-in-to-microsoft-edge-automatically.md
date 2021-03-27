---
title: Microsoft Edge'de otomatik olarak oturum açma
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
ms.openlocfilehash: 6021991c125f5cb2a33ce8db8fe7717b528bf49b
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398749"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Microsoft Edge'de otomatik olarak oturum açma

Microsoft Edge, kullanıcının cihazına göre otomatik olarak oturum açması için işletim sistemi varsayılan hesabını kullanır. 

Cihaz yapılandırmasının her türüyle bağımlı kullanıcı oturum açma işleminin senaryoları aşağıda açıklanmıştır:

- **Cihaz karma/AAD-J**: Bu seçenek Windows 10, düşük düzey Windows ve buna karşılık gelen sunucu sürümlerinde kullanılabilir. Kullanıcılar, Azure Active Directory (AD) hesaplarıyla otomatik olarak oturum açılır.
- **Cihaz etki alanına katılmış durumdadır:** Bu seçenek Windows 10, alt düzey Windows ve buna karşılık gelen sunucu sürümlerinde kullanılabilir. Varsayılan olarak, etki alanı hesabı olan kullanıcılar otomatik olarak oturum alanmaz; otomatik oturum açma özelliğini etkinleştirmek için **ConfigureOnPremisesAccountAutoSignIn ilkesi kullanın.** Azure AD hesapları olan kullanıcılar için otomatik oturum açma özelliğini etkinleştirmek için cihazlarına karma katılmayı göz önünde bulundurabilirsiniz.
- **OS'un** varsayılan hesabı bir Microsoft hesabıdır: Bu seçenek Windows 10 RS3 (sürüm 1709, derleme 10.0.16299) ve sonraki sürümlerde kullanılabilir. Senaryonun kurumsal cihazlarda gerçekleşmesi olası değildir. Bununla birlikte, işletim sistemi varsayılan hesabı bir Microsoft hesabı ise, Microsoft Edge otomatik olarak kullanıcının Microsoft hesabıyla oturum açmasını sağlar.
 
 
