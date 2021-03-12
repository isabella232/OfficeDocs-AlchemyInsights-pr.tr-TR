---
title: Koşullu Erişimi İzleme
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003769"
- "6702"
ms.openlocfilehash: c3bf5dd9066685af2df7ba50f0eb3ba6e891c2a9
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708694"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Exchange için Koşullu Erişimi İzleme

Koşullu erişimle hedef alan kullanıcılar, kuruma erişim gereksinimlerini karşılamıyorsa bir bildirim e-postası alırlar. Bu sorunu çözmek için aşağıdaki çözümlerden birini veya birden fazlasını öneririz:

- Cihazın kayıtlı olduğu varsayiliyorsa, kullanıcıya Şirket Portalı uygulamasına gidip cihazın Şirket Portalı'nda görüntülendiğinden emin olması önerin. Bunu yoksa, kullanıcının cihazı kaydetmesi gerekir.
- Azure portalında Intune'a > uyumluluğuna gidin. İzleme'nin altında Cihaz uyumluluğu'ne tıklayın. Kullanıcının cihazı uyumlu olarak işaretlenir doğrulamak için cihaz uyumluluk raporlarınızı görüntüleme.
- Azure portalında Intune'a > uyumluluğuna gidin. Yönet'in altında İlkeler'e tıklayın. Uyumluluk ilkeleri listesinde, kullanıcı cihazınıza bir profilin atandığı doğrulayın. Profil atanmamışsa, Intune cihazın uyumluluk durumunu onaylamaz.
- Kullanıcının koşullu erişim atamalarını düzenleyin.

1. Azure portalında **Intune Koşullu erişim**  >  **İlkeleri'ne**  >  **gidin.**
2. Listeden bir ilke seçin.
3. Kullanıcılar ve gruplar'a tıklayın.
4. Belirli bir ilkeyi birine hedeflemek için, bu ilkeyi Ekle listesine ekleyin. Bir kişinin ilkeden atlanmış olduğundan emin olmak için, bu kişiyi Dışla listesine ekleyin.

Yararlı bağlantılar:

[Cihaz uyumluluğuna genel bakış](https://docs.microsoft.com/intune/device-compliance-get-started)

[CA sorunlarını giderme](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Sorun giderme ilkesi](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[Intune cihaz uyumluluğunu izleme](https://docs.microsoft.com/intune/compliance-policy-monitor)

Not: Bu adımlar yalnızca Azure Active Directory özelliği Koşullu Erişim sorunlarını gidermek için yararlıdır. Ayrıca, Exchange ilkesiyle e-posta erişimini engelleyen bir cihazı karantinaya almak da mümkündür. Exchange cihaz yönetimi hakkında daha fazla bilgiyi [burada]( https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) bulunabilir.
