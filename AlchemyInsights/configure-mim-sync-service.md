---
title: MIM Eşitleme hizmetini yapılandırma
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8472"
- "9004688"
ms.openlocfilehash: 48e9a0e8c26088b690092bfaedfba641841739f6
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482894"
---
# <a name="configure-mim-sync-service"></a>MIM Eşitleme hizmetini yapılandırma

Microsoft Identity Manager (MIM) Eşitleme Hizmeti, MIM'nin bir bileşenidir. Birden çok şirket içi dizine ve veritabanına sahip kuruluşlar için bilgileri depolar ve tümleştiren merkezi bir şirket içi hizmettir. Sorun yakın zamanda MIM güncelleştirmesinde ele alındı ise veya aşağıdaki bölümde adı geçen diğer sorunlardan biri ise MIM Eşitleme ile ilgili sorununuzu çözebilirsiniz.

**Önerilen adımlar**

1. MIM Eşitleme'nin son güncelleştirmesini kullanırkenn emin olun ve bir güncelleştirmede sorunun çözülmüş olup olmadığını belirlemek için [MIM Sync](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) sürüm notlarına bakın.
2. Sorun Generic LDAP, Generic SQL, Lotus Domino veya Web Services bağlayıcısı ile ilgili ise, genel bağlayıcıların son güncelleştirmesini [kullanırkenn emin olun.](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history)
3. MIM Eşitleme çalıştırması hatayla durursa, olası nedenleri belirlemek [için çalıştırma](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) hata kodları tablosuna bakın.
4. **Uzantı-dll-özel** durumu ile çalıştırma durursa, Bağlayıcı Alanı  Nesnesi özellikler penceresini açmak için bu sözcüklere tıklayın ve Temel neden hakkında daha fazla bilgi görmek için [Uzantı-DLL-Özel](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx)Durum'da açıklandığı gibi Yığın **İzleme...'ye** tıklayın.
5. Parola Değişikliği Bildirim Hizmeti (PCNS) bileşeni, parola eşitlemesi sırasında olay günlüğünde **6025** hatasını bildiriyorsa, [PCNS raporlama hatası 6025](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx)ile ilgili sorun giderme kılavuzunu kontrol edin.
6. FIM Hizmet Yönetimi Aracısı ile tam eşitleme  yavaşsa, TempDB için otomatik büyüme ayarını kontrol edin. Sorun giderme yavaş veya asılı tam eşitlemede açıklandığı [gibi.](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx)
7. FIM Hizmet Yönetimi Aracısını kullanarak başarısız oluşturma-yoluyla web-hizmetleriyle durduruldu sunucusu hatasıyla karşılaşıyorsanız, nedenlere genel bakış için [Destek-Bilgi: başarısız oluşturma-web-hizmetleri](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) hakkında bilgi için bkz.

