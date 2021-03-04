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
ms.openlocfilehash: e2803a49aaf087ac55b1fd62056e2b0af3fcd919
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/03/2021
ms.locfileid: "50428310"
---
# <a name="monitor-intune-conditional-access"></a>Intune Koşullu Erişimini İzleme

Koşullu erişimle hedef alan kullanıcılar, kuruma erişim gereksinimlerini karşılamıyorsa bir bildirim e-postası alırlar. Bu sorunu çözmek için aşağıdaki çözümlerden birini veya birden fazlasını öneririz:

1. Cihazın kayıtlı olduğu varsayiliyorsa, kullanıcıya Şirket Portalı uygulamasına gidip cihazın Şirket Portalı'nda görüntülendiğinden emin olması önerin. Bunu yoksa, kullanıcının cihazı kaydetmesi gerekir.
1. Azure portalında **Intune Cihaz**  >  **uyumluluğu'ne gidin.** 
1. Kullanıcının cihazı uyumlu olarak işaretlenirken cihaz uyumluluk raporlarınızı görüntülemek için, monitör altında **Cihaz** **uyumluluğu'ne tıklayın.**
1. Azure portalında **Intune Cihaz**  >  **uyumluluğu'ne gidin.** **Yönet'in altında İlkeler'e** **tıklayın.** Uyumluluk ilkeleri listesinde, kullanıcı cihazınıza bir profilin atandığı doğrulayın. Profil atanmamışsa, Intune cihazın uyumluluk durumunu onaylamaz.
1. Kullanıcının koşullu erişim atamalarını düzenleyin.
1. Azure portalında **Intune** Koşullu erişim İlkelerine gidin, listeden bir ilke seçin ve Kullanıcılar  >    >  ve **gruplar'a tıklayın.**
1. Belirli bir ilkeyi birine hedeflemek için, bu ilkeyi Ekle **listesine ekleyin.** Bir kişinin ilkeden atlanmış olduğundan emin olmak için, bu kişiyi Dışla **listesine ekleyin.**

**Yararlı bağlantılar:**

- [Cihaz uyumluluğuna genel bakış](https://docs.microsoft.com/intune/device-compliance-get-started)
- [CA sorunlarını giderme](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [Sorun giderme ilkesi](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [Intune cihaz uyumluluğunu izleme](https://docs.microsoft.com/intune/compliance-policy-monitor)

> [!NOTE]
> Bu adımlar yalnızca Azure Active Directory özelliği Koşullu Erişim sorunlarını gidermek için yararlıdır. Ayrıca, Exchange ilkesiyle e-posta erişimini engelleyen bir cihazı karantinaya almak da mümkündür. Exchange cihaz yönetimi hakkında daha fazla bilgiyi burada [**bulunabilir.**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141))
