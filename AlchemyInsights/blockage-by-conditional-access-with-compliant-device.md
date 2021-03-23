---
title: Uyumlu bir cihazla Koşullu Erişim tarafından engellendim
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9835"
- "9003257"
ms.openlocfilehash: 240bd25f4d62505202c8cd7ceabe4c1cd3d5c0b5
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037080"
---
# <a name="im-getting-blocked-by-conditional-access-with-compliant-device"></a>Uyumlu cihazla Koşullu Erişim tarafından engellendim

**Kesinlikle Önerilen Araçlar**

- [Cihaz Kayıt Sorun Giderici Aracı](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - En yaygın cihaz kayıt sorunlarını gidermeye yardımcı olan kapsamlı bir araçtır.
- [Cihaz Kayıt Bağlantısını Test Edin](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) betiği - Bir cihazın sistem hesabı altındaki Cihaz Kaydı uç noktalarına erişe olduğundan emin olmak için kullanılan bir araç.
- [Azure AD Cihaz Temizleme Betiği](https://github.com/mzmaili/AzureADDeviceCleanup) - Ortamınıza eski cihazları aramak ve yönetmek için kullanılan bir araçtır.

Koşullu **Erişim'in** uyumlu bir cihaz için başarısız olması veya kullanıcılarınızı neden alıyor olabilir? Kuruluş kaynağına oturum açma isteği sırasında bu iletiden ulaşamayabilirsiniz.

1. **Cihaz, MDM'ye sahip gerekli bir cihaz durumuna sahip değil:**

Cihazın Intune gibi onaylı bir MDM sağlayıcısına kaydedilip uyumlu *olarak işaretlenir.* Intune hakkında daha fazla bilgi için bu belgeye [bakın.](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) Cihaz uyumluluğunu ve Intune'i daha iyi anlamak için, [Intune](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)ile yönettikleri cihazlar için kurallar ayarlamak üzere uyumluluk ilkesi kullanma. Bir cihazı Intune'a kaydetmede sorun giderme sorunlarıyla karşılaşılan sorunları gidermek için Microsoft'ta Cihaz kaydı sorunlarını [giderme makalesinde bulabilirsiniz.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) Daha fazla Intune desteği için bir destek isteği oluşturun. Bunu yapmak için [Intune Yardım ve Destek sayfasını ziyaret edin.](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/SupportMenu/helpSupport)

2. **Cihaz kuruluşlar ağına katılmadı:**

Kuruluş kaynaklarına erişim için cihazın doğrudan bağlantı veya sanal özel ağ (VPN) aracılığıyla ve ayrıca şirket içi veya Azure Active Directory'ye katılmış olması gerekir. İş cihazına kuruluş ağına katılmak için [bkz. İş cihazınızın kuruluş ağına katılma.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network) Kişisel/TEKM cihazı kaydetmek için bkz. Kişisel [cihazınızı kurum ağınıza kaydetme.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network)

- Cihazın ağa katıldığını doğrulamak için, buradaki kayıtlı cihazların veya iş [cihazlarının](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network#to-verify-that-youre-registered) adımlarını takip [edebilirsiniz.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network#to-make-sure-youre-joined) Sorunu Kuruluş ağı bağlantısı kapsamında yapmak için aşağıdaki yönergeleri izleyin:

    1. örneğin iş veya okul hesabınızla Windows'ta oturum alain@contoso.com.
    2. Vpn veya DirectAccess aracılığıyla kuruluş ağınıza bağlanabilirsiniz.
    3. Bağlandıktan sonra cihazınızı kilitlemek için **Windows logo tuşu+L** tuşlarına basın.
    4. İş veya okul hesabınızla cihazınızın kilidini açın ve sorunlu uygulama veya hizmete yeniden erişmeyi deneyin.

Buradan buraya **tekrar gelemedi hata iletisini görüyorsanız,** sorun muhtemelen başka bir yerdedir.

3. **İşletim sistemi desteklenmiyor:**

İşletim sisteminin desteklenen bir sürümünü çalıştırmış olduğundan emin olun; aşağıdakiler de dahil:

- **Windows İstemcisi:** Windows 7 veya sonrası

- **Windows Server**: Windows Server 2008 R2 veya sonrası

- **macOS**: macOS X veya sonrası

- **Android ve iOS**: Android ve iOS mobil işletim sistemlerinin en son sürümü

4. **Web tarayıcısı desteklenmiyor:**

Lütfen aşağıdaki desteklenen tarayıcıları bulun. Windows 1703 veya sonraki sürümlerde Chrome desteği için Windows 10 Hesapları uzantısı gereklidir. Edge 85+ için, cihaz uyumluluk bilgilerini düzgün bir şekilde geçmek için kullanıcının oturumlarının açık olması gerekir. Diğer ayrıntılar için buraya [bakın.](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support)

- **Windows 10**: Microsoft Edge, Internet Explorer, Chrome
- **Windows 8 / 8.1**: Internet Explorer, Chrome
- **Windows 7**: Internet Explorer, Chrome
- **iOS**: Microsoft Edge, Intune Yönetilen Tarayıcısı, Safari
- **Android**: **Microsoft Edge**: Intune Yönetilen Tarayıcı, Chrome
- **Windows Phone**: Microsoft Edge, Internet Explorer
- **Windows Server 2019**: Microsoft Edge, Internet Explorer, Chrome
- **Windows Server 2016**: Internet Explorer
- **Windows Server 2012 R2**: Internet Explorer
- **Windows Server 2008 R2**: Internet Explorer
- **macOS**: Chrome, Safari

Daha fazla bilgi için **buraya ileti ve sorun giderme** adımlarını buradan [edinebilirsiniz.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-device-remediation)
