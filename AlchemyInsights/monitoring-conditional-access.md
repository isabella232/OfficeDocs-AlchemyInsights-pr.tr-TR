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
ms.openlocfilehash: 80e8cc72db8ae32445d48e5c8a411d5ccd538626653260b3dbd28a247561e888
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53975121"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Denetimler için Koşullu Erişimi Exchange

Koşullu erişimle hedef alan kullanıcılar, kuruma erişim gereksinimlerini karşılamıyorsa bir bildirim e-postası alır. Bu sorunu çözmek için aşağıdaki çözümlerden birini veya birden fazlasını öneririz:

- Cihazın kayıtlı olduğu varsay görünüyorsa, kullanıcıya Şirket Portalı uygulamasına gidip cihazın kayıtta görüntülendiğinden emin Şirket Portalı. Yoksa, kullanıcının cihazı kaydetmesi gerekir.
- Azure portalında Intune'a gidin ve > uyumluluğu sağlayın. İzleme altında Cihaz uyumluluğu'ne tıklayın. Kullanıcının cihazı uyumlu olarak işaretlenirken emin olmak için cihaz uyumluluk raporlarınızı görüntüleme.
- Azure portalında Intune'a gidin ve > uyumluluğu sağlayın. Yönet'in altında İlkeler'e tıklayın. Uyumluluk ilkeleri listesinde, kullanıcı cihazınıza bir profil atan olduğunu doğrulayın. Profil atanmamışsa, Intune cihazın uyumluluk durumunu onaylayabilir.
- Kullanıcının koşullu erişim atamalarını düzenleyin.

1. Azure portalında **Intune Koşullu erişim İlkeleri'ne**  >    >  **gidin.**
2. Listeden bir ilke seçin.
3. Kullanıcılar ve gruplar'a tıklayın.
4. Belirli bir ilkeyi bir birine hedeflemek için, o ilkeyi Ekle listesine ekleyin. Bir kişinin ilkeye dahil dışı bırakıla olduğundan emin olmak için, o kişiyi Dışla listesine ekleyin.

Yararlı bağlantılar:

[Cihaz uyumluluğuna genel bakış](https://docs.microsoft.com/intune/device-compliance-get-started)

[CA sorunlarını giderme](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Sorun giderme ilkesi](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[Intune cihaz uyumluluğunu izleme](https://docs.microsoft.com/intune/compliance-policy-monitor)

Not: Bu adımlar yalnızca Koşullu Erişim özelliğinin Azure Active Directory yardımcı olur. Ayrıca, e-posta erişimini engelleyen bir cihazı karantinaya almak için de Exchange mümkündür. Cihaz yönetimi Exchange daha fazla bilgiyi [here]( https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) bulunabilir.
