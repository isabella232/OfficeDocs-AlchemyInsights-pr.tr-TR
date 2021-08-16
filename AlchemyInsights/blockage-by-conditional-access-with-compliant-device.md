---
title: Uyumlu cihazla Koşullu Erişim tarafından engellendim
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
ms.openlocfilehash: 709749b1a62f2d9cdabfb3fe4b7538c22101d7109204d9163f6059336b817bf8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54019168"
---
# <a name="im-getting-blocked-by-conditional-access-with-compliant-device"></a>Uyumlu cihazla Koşullu Erişim tarafından engellendim

**Kesinlikle Önerilen Araçlar**

- [Cihaz Kayıt Sorun Giderici Aracı](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - En yaygın cihaz kayıt sorunlarını gidermeye yardımcı olan kapsamlı bir araçtır.
- [Cihaz Kayıt Bağlantısını Test Edin betiği](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) - Bir cihazın sistem hesabı altındaki Cihaz Kaydı uç noktalarına erişe olduğundan emin olmak için kullanılan bir araç.
- [Azure AD Cihaz Temizleme Betiği](https://github.com/mzmaili/AzureADDeviceCleanup) - Ortamınıza eski cihazları aramak ve yönetmek için kullanılan bir araçtır.

Koşullu Erişim'in uyumlu bir cihazda başarısız olması veya kullanıcılarınızı neden  kurumsal bir kaynağa yönelik oturum açma isteği sırasında buradan alamayabilirsiniz.

1. **Cihaz, MDM ile gerekli bir cihaz durumuna sahip değildir:**

Cihazın Intune gibi onaylı bir MDM sağlayıcısına kayded olduğunu ve uyumlu olarak *işaretlenen olduğunu doğrulama.* Intune hakkında daha fazla bilgi için bu belgeye [bakın.](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) Cihaz uyumluluğu ve Intune'la ilgili daha iyi anlamak için, [bkz. Intune](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)ile yönetmek zorunda olduğunuz cihazlar için kurallar ayarlamak için uyumluluk ilkesi kullanma. Cihazı Intune'a kaydetmekte sorun ediyorsanız, Sorun giderme ayrıntılarını Microsoft'ta cihaz kaydı sorunlarını [giderme makalesinde bulabilirsiniz.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) Intune desteğine daha fazla bilgi için bir destek isteği oluşturun. Bunu yapmak için [Intune Yardım ve Destek sayfasını ziyaret edin.](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/SupportMenu/helpSupport)

2. **Cihaz kuruluşlar ağına katılmadı:**

Kuruluş kaynaklarına erişim için cihazın doğrudan bağlantı veya sanal özel ağ (VPN) aracılığıyla kuruluşun ağına bağlı olması ve ayrıca şirket içi veya İnternet'e Azure Active Directory. İş cihazına kuruluş ağına katılmak için [bkz. İş cihazınızı kuruluş ağınıza katılma](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network). Kişisel/BYOD cihazı kaydetmek için bkz. Kişisel cihazınızı [kuruluş ağınıza kaydetme](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network).

- Cihazın ağa katıldığını doğrulamak için, burada kayıtlı cihazların veya iş [cihazlarının](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network#to-verify-that-youre-registered) adımlarını takip [edebilirsiniz.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network#to-make-sure-youre-joined) Sorunun kapsamını Kuruluş ağı bağlantısı olarak kapsamına etmek için aşağıdaki yönergeleri izleyin:

    1. İş veya Windows, örneğin okul hesabınızla oturum alain@contoso.com.
    2. Bağlan VPN veya DirectAccess aracılığıyla kuruluş ağınıza bağlanabilirsiniz.
    3. Bağlandıktan sonra, cihazınızı kilitlemek **Windows logo tuşu+L** tuşlarına basın.
    4. İş veya okul hesabını kullanarak cihazınızın kilidini açın ve sorunlu uygulama veya hizmete erişmeyi yeniden deneyin.

Buradan buraya **tekrar alaasınız hata** iletisini görüyorsanız, sorun büyük olasılıkla başka bir yerdedir.

3. **İşletim sistemi desteklenmiyor:**

İşletim sisteminin desteklenen bir sürümünü, aşağıdakiler gibi çalıştırmış olduğundan emin olun:

- **Windows İstemcisi**: Windows 7 veya sonrası

- **Windows :** Windows Server 2008 R2 veya sonrası

- **macOS**: macOS X veya daha yenisi

- **Android ve iOS:** Android ve iOS mobil işletim sistemlerinin en son sürümü

4. **Web tarayıcısı desteklenmiyor:**

Lütfen aşağıda desteklenen tarayıcıları bulabilirsiniz. Windows 1703 veya sonraki sürümleri ile Chrome desteği için Windows 10 uzantısı gereklidir. Edge 85+ için, cihaz uyumluluk bilgilerini doğru şekilde geçmek için kullanıcının oturumlarının olması gerekir. Diğer ayrıntılar için buraya [bakın.](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support)

- **Windows 10:** Microsoft Edge, Internet Explorer, Chrome
- **Windows 8 / 8.1**: Internet Explorer, Chrome
- **Windows 7**: Internet Explorer, Chrome
- **iOS:** Microsoft Edge, Intune Managed Browser, Safari
- **Android**: **Microsoft Edge**: Intune Managed Browser, Chrome
- **Windows Phone**: Microsoft Edge, Internet Explorer
- **Windows Server 2019**: Microsoft Edge, Internet Explorer, Chrome
- **Windows Server 2016:** Internet Explorer
- **Windows Server 2012 R2**: Internet Explorer
- **Windows Server 2008 R2**: Internet Explorer
- **macOS**: Chrome, Safari

Daha fazla bilgi için buraya **iletinin ve sorun giderme** adımlarını [bulabilirsiniz.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-device-remediation)
