---
title: Varsayılan Yammer etki alanını değiştirme
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002662"
- "5162"
ms.openlocfilehash: 099feb5c58a2b1068a2ec501ff966c6ac73d804d
ms.sourcegitcommit: 87aa36e3ff4835efb120a320c5169bfa77199ec4
ms.translationtype: HT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/01/2020
ms.locfileid: "43991331"
---
# <a name="changing-the-defaultprimary-yammer-domain"></a>Varsayılan/birincil Yammer etki alanını değiştirme

Yammer URL’si, Yammer ağınızın geçerli birincil etki alanı adını içerir. Bu etki alanı adı Office 365’te veya Azure AD’de ayarlanan birincil etki alanı adıyla eşleşmeyebilir. Kiracıya eklenen özel etki alanı sayısına ve Yammer’ın desteklenen bir yapılandırmada (1 Kiracı: 1 Ağ veya 1:1) olup olmadığına göre davranışta farklılıklar vardır. [Yammer etki alanları ve Office 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/manage-yammer-domains) ile ilgili belgeler mevcuttur.

Yanlış bir etki alanı görmenizin en yaygın nedeni, birden çok Yammer ağının bulunmasıdır ve bunların birleştirilmesi gerekir.  Ağ geçiş aracını kullanarak [tek bir ağ halinde birleştirme](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) ilk önemli adımdır. Birincil etki alanınızı ayarlamayı denemeden önce bu adımı tamamlayın.

**Özel etki alanı yok**

Yeni kiracılarda, Yammer için kiracıdan alınan varsayılan etki alanı (örn. fabrikam.onmicrosoft.com) kullanılır. Birincil etki alanı, yammer.com/fabrikam.onmicrosoft.com olarak ayarlanır.

**Tek özel etki alanı**

Yammer otomatik olarak kiracıdan alınan özel etki alanını (örn. fabrikam.com) Yammer’da birincil etki alanı olarak seçer. Etki alanı, yammer.com/fabrikam.com olarak ayarlanır. Bu değişiklik etki alanı eşitleme hizmeti ile yapılır ve geçerli olması 24 saati bulabilir.

**Birden çok özel etki alanı**

Yammer varsayılan kiracı etki alanından farklı bir birincil etki alanına sahip olabilir. Birden çok özel etki alanı olduğundan, Yammer kullanılabilir olanlar arasından doğru etki alanını tahmin etmeyi denemez. Birincil etki alanı adının tercih ettiğiniz birincil etki alanı olarak değiştirilmesini isteyen bir destek olayı açmanız gerekir.

**Ek sorun giderme bilgileri**

Bazı durumlarda, etki alanları kiracılar arasında taşınmış olabilir ve etki alanı eşitleme hizmeti başarıyla çalıştırılamayabilir. Yanlış bir birincil etki alanının yanı sıra oturum açma sorunu veya başka sorunlar yaşayabilirsiniz. Bu sorunu çözmek için, etki alanlarının Microsoft Desteği’nden yardım alınarak doğru ağa taşınması gerekebilir. Bu durum doğrudan yardım gerektirir ve özellikle çok uzun bir etki alanı adı listesi varsa çözülmesi biraz zaman alabilir. Bu tür sorunların çözümüyle ilgili yardım almak için bir destek olayı açın.

Bir destek temsilcisiyle çalışırken, destek temsilcisi denetimizde olan bir kiracıdaki etki alanlarının doğrulanıp doğrulanmadığını kontrol eder. Destek temsilcisi, kiracınıza eklenmiş ancak DNS tarafından doğrulanmamış etki alanlarınız hakkında ek doğrulama soruları sorabilir. İşlemi hızlandırmak için lütfen etki alanlarının DNS tarafından doğrulandığından emin olun.
