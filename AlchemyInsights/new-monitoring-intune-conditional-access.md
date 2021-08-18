---
title: Intune Koşullu Erişimini İzleme
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004636"
- "8386"
ms.openlocfilehash: 2c3a382671ac95ecbaec1b374bd8c474cf9690a2
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58327577"
---
# <a name="monitor-intune-conditional-access"></a>Intune Koşullu Erişimini İzleme

Koşullu erişimle hedef alan kullanıcılar, kuruma erişim gereksinimlerini karşılamıyorsa bir bildirim e-postası alırlar. Bu sorunu çözmek için aşağıdaki çözümlerden birini veya birden fazlasını öneririz:

1. Cihazın kayıtlı olduğu varsay görünüyorsa, kullanıcıya Şirket Portalı uygulamasına gidip cihazın kayıtta görüntülendiğinden emin Şirket Portalı. Bunu yoksa, kullanıcının cihazı kaydetmesi gerekir.
1. Azure portalında **Intune Cihaz**  >  **uyumluluğu'ne gidin.** 
1. Kullanıcının cihazı uyumlu olarak işaretleniyor olduğunu doğrulamak üzere cihaz uyumluluk raporlarınızı görüntülemek için, Monitör altında, **Cihaz** uyumluluğu **'ne tıklayın.**
1. Azure portalında **Intune Cihaz**  >  **uyumluluğu'ne gidin.** **Yönet'in altında İlkeler'e** **tıklayın.** Uyumluluk ilkeleri listesinde, kullanıcı cihazınıza bir profil atanmalıdır. Profil atanmamışsa, Intune cihazın uyumluluk durumunu onaylayabilir.
1. Kullanıcının koşullu erişim atamalarını düzenleyin.
1. Azure portalında **Intune Koşullu erişim İlkeleri'ne** gidin, listeden bir ilke seçin ve Kullanıcılar ve  >    >   **gruplar'a tıklayın.**
1. Belirli bir ilkeyi bir kişinin hedefi olarak hedeflemek için, o ilkeyi Ekle **listesine ekleyin.** Bir kişinin ilkeye dahil dışı bırakıla olduğundan emin olmak için, o kişiyi Dışla **listesine ekleyin.**

**Yararlı bağlantılar:**

- [Cihaz uyumluluğuna genel bakış](https://docs.microsoft.com/intune/device-compliance-get-started)
- [CA sorunlarını giderme](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [Sorun giderme ilkesi](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [Intune cihaz uyumluluğunu izleme](https://docs.microsoft.com/intune/compliance-policy-monitor)

**Not:** Bu adımlar yalnızca Koşullu Erişim özelliğinin Azure Active Directory yardımcı olur. Ayrıca, o cihazın e-posta erişimini engelleyen bir cihazı karantinaya Exchange mümkündür. Cihaz yönetimi Exchange fazla bilgiyi burada [**bulunabilir.**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141))
