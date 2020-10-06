---
title: Koşullu erişimi izleme
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
ms.openlocfilehash: 0687875a3714067e774872d02630564858d71d1b
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366448"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Exchange için koşullu erişimi izleme

Koşullu erişimle hedeflenen kullanıcılar kuruluşunuzun erişim gereksinimlerini karşılamıyorsa bildirim e-postası alır. Sorunu çözmek için, aşağıdaki çözümlerden bir veya daha fazlasını öneririz:

- Cihazın kayıtlı olduğu kabul ediyorsanız, kullanıcının Şirket Portalı uygulamasına gitmesini ve şirket portalında göründüğünü doğrulamasını tavsiye edin. Yoksa, Kullanıcı cihazı kaydetmelidir.
- Azure portalında cihaz uyumluluğu > Intune 'a gidin. Monitör altında cihaz uyumluluğu 'nı tıklatın. Cihazın uyumluluk raporunuzu görüntülemek için, kullanıcının cihazının uyumlu olduğunu doğrulayın.
- Azure portalında cihaz uyumluluğu > Intune 'a gidin. Yönet altında, Ilkeler 'e tıklayın. Uyumluluk ilkeleri listesinde, kullanıcının cihazına bir profilin atandığını doğrulayın. Atanmış profil yoksa, Intune cihazın uyumluluk durumunu doğrulayamayacaktır.
- Kullanıcının koşullu erişim atamasını düzenleyin.

1. Azure portalında **Intune**  >  **koşullu erişim**  >  **ilkelerine**gidin.
2. Listeden bir ilke seçin.
3. Kullanıcılar ve gruplar 'ı tıklatın.
4. Belirli bir ilkeyi bir başkasından hedeflemek için bunları ekleme listesine ekleyin. Bir kişinin ilkeden atlandığından emin olmak için bunları dışlama listesine ekleyin.

Faydalı bağlantılar:

[Cihaz uyumuna genel bakış](https://docs.microsoft.com/intune/device-compliance-get-started)

[Sorun giderme CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Sorun giderme ilkesi](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

[Intune cihaz uyumluluğunu izleme](https://docs.microsoft.com/intune/compliance-policy-monitor)

Not: Bu adımlar yalnızca Azure Active Directory özelliğinin koşullu erişimi sorunlarını gidermede yardımcı olur. Exchange ilkesiyle e-posta erişimini engelleyen bir cihaz karantinaya alınabilir. Exchange cihazı yönetimi hakkında daha fazla bilgiyi [burada](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>)bulabilirsiniz.
