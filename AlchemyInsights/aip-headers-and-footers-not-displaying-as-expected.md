---
title: 'AIP: Üstbilgiler ve altbilgiler beklendiği gibi görüntülenmiyor'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4541"
ms.openlocfilehash: e3a0e5caccba87ddd8e4c786b5c8918494e709b6f4d5d60e7c31215a60b1d5d6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951801"
---
# <a name="aip-headers-and-footers-not-displaying-as-expected"></a>AIP: Üstbilgiler ve altbilgiler beklendiği gibi görüntülenmiyor

Görsel işaretlerin beklendiği gibi görüntülenmesiyle ilgili sorunlar yaşıyorsanız, aşağıdaki yönergeleri izleyin:

1. Görsel işaretler uygulandığında [incelemeyi gözden geçirmeyi sağlar.](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)
2. Daha Office için, İçerik işaretleme [ve Office 365 için ne zaman içerik işaretlemesi ve şifrelemesi uygulandığını gözden geçirebilirsiniz.](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps#when-office-apps-apply-content-marking-and-encryption)
3. Var olan üst bilgileri/alt bilgileri kaldırmak için, Diğer etiket çözümlerinden üst bilgileri [ve alt bilgileri kaldırma'ya bakın.](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-customizations#remove-headers-and-footers-from-other-labeling-solutions)

Sorun hala yaşıyorsanız, Azure Information Protection istemci günlüklerini toplayın ve dışarı aktarıldı günlükleri bu bilete iliştirin.

**Azure Information Protection günlüklerini dışarı aktarma**

1. Office'da bir belge açın veya e-posta Outlook.
2. **Koru/Duyarlılık Yardımı ve geri**  >  **bildirim'e tıklayın.**
3. Günlükleri Dışarı **Aktar 'a tıklayın.**
4. Günlükleri tercih konumunuzla kaydedin ve bunları bu hizmet isteğine iliştirin.

Ek bilgi için bkz:

- [Azure Information Protection'da görsel işaretlere uygun etiketi yapılandırma](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Azure Information Protection belgelerini gözden geçirme](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Azure Information Protection gereksinimleri](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Azure Information Protection hızlı başlangıç öğreticisi](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [Azure Information Protection istemcisini indirin](https://www.microsoft.com/download/details.aspx?id=53018)
