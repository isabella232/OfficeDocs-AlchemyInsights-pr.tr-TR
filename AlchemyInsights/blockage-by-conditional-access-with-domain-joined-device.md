---
title: Etki alanına katılmış bir cihazla Koşullu Erişim tarafından engellendim
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/20/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9834"
- "9003257"
ms.openlocfilehash: 052311ffe71bcb65de2b5c2a964932b1fb99c373
ms.sourcegitcommit: c34ba92e19419dcb2d251b8a1afe4d180a939617
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/20/2021
ms.locfileid: "51038106"
---
# <a name="im-getting-blocked-by-conditional-access-with-domain-joined-device"></a>Etki alanına katılmış bir cihazla Koşullu Erişim tarafından engellendim

**Kesinlikle Önerilen Araçlar**

[Cihaz Kayıt Sorun Giderici Aracı](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - En yaygın cihaz kayıt sorunlarını gidermeye yardımcı olan araçtır.

[Cihaz Kayıt Bağlantısı betiği-](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) Bir cihazın sistem hesabı altındaki Cihaz Kaydı uç noktalarına erişemelerini sağlamaya yardımcı olan betik.

[Azure AD Cihaz Temizleme Betiği](https://github.com/mzmaili/AzureADDeviceCleanup) - Ortamınıza eski cihazları aramanızı ve yönetmenizi sağlayan betik.

İşte koşullu erişimin etki alanına (Karma Azure AD) katılmış bir cihazda başarısız olmasıyla ilgili bazı yaygın nedenler.

1. **Cihazda Azure AD PRT** yoktur. Cihazın Azure AD Birincil Yenileme Belirteci'ne (PRT) sahip olduğundan emin olun. PRT hakkında daha fazla bilgi için bu belgeye [bakın.](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)

Azure AD PRT'niz olup olduğunu doğrulamak için, cihazda komutu çalıştırabilirsiniz ve `dsregcmd/status` "AzureAdPrt" eşittir "EVET".

"AzureAdPrt" "HAYıR" ise, şunları kontrol edin:

- **AD FS ile** bir federasyon ortamınız olup olmadığı ve bu ortam kullanıcılarının ev ağlarından erişilemiyor olabilir: Bu durumda, "kullanıcıadı"sı olan" uç noktalarınıza extranet'den erişile olduğundan emin olun. AD FS'niz bir VPN'nin arkasında ise, kullanıcıların VPN'ye bağlana olduğundan emin olun ve cihaza yeniden oturum açın. Daha fazla bilgi için bu belgeye [bakın.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains)

- **Cihazın TPM'sinde** hata olup olmadığı ve dolayısıyla cihazın kimliğini doğrulayama durumunun doğrulanıp doğrulanamayıp doğrulanamama: TPM durumunun "Hazır" olup olmadığını görmek için "tpm.msc"yi kontrol edin. Yoksa, çalıştırın `dsregcmd/leave` ve cihazın Azure AD'ye yeniden katılmasına izin verme. Daha sonra yeniden deneyin. Daha fazla bilgi için bu belgeye [bakın.](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)

- **Üçüncü taraf bir kimlik sağlayıcısı kullanıyorsanız ve bu** sağlayıcı üçüncü taraf kimlik WS-Trust desteklemez. Belgelerimizde açıklandığı gibi, Azure AD'ye katılmış karma cihazlar bu durumda çalışamaz. Destek için lütfen Kimlik sağlayıcınızla birlikte çalışabilirsiniz.

2. **Windows 10** Hesapları veya Office uzantısı olmadan kullanıcılar Chrome tarayıcısını **kullanıyorsa Chrome, AAD'ye** katılmış veya karma AAD'ye katılmış cihazlarda PRT'yi otomatik olarak kullanmaz: Bu, "Kayıtsız cihaz" hata iletisi görüntülendiğinde cihaz tabanlı Koşullu Erişim ilkelerinin başarısızlığına yol açabilir. Chrome tarayıcısını doğru kullanmak için SCCM veya Intune aracılığıyla "Windows 10 Hesapları" veya "Kullanıcıların Chrome tarayıcısına Office uzantısını" yüklemeniz gerekir. Daha fazla bilgi için bu belgeye [bakın.](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support)

Uzantıyı uzaktan itmek mümkün yoksa, cihaz tabanlı Koşullu Erişim'in arkasındaki uygulamalara erişmek için kullanıcılara yukarıdaki uzantılardan birini el ile yüklemelerini bildirin. Daha fazla bilgi için bu belgeye [bakın.](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites)

3. Cihaz Azure AD'ye doğru bir şekilde katılmış, ancak Azure AD Connect'te yapılan eşitleme değişiklikleri veya **Azure portalında** yapılan eşitleme değişiklikleri nedeniyle yanlışlıkla silinmiş veya devre dışı bırakılmış olabilir: Böyle bir durumda, "AzureAdJoined" ve "PRT" durumu cihazda geçerli olarak gösterse bile cihaz nesnesi artık tam olarak katılmış bir cihaz olarak tanınmıyor.

Bu sorunu çözmek için, `dsregcmd/leave` etkilenen cihazlarda çalıştırın ve Azure AD'ye yeniden katılmalarına izin ver. Daha fazla bilgi için bu belgeye [bakın.](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices)

> [!NOTE]
> Cihazlarınız Windows 10 1809 güncelleştirmesinde, VPN/Bulut Proxy'si ile çalışıyor ve "AzureAdPrt" durumu veya SSO sorunu olan herhangi bir uygulamayla ilgili sorunları görüyorsanız (PRT'niz olsa bile outlook posta kutusuna bağlanıyorsa), bu makinelerde PRT hatalarını önlemek için [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) veya Nisan toplu güncelleştirmesi [KB4549949'u](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) gördüğünüzden emin olun.

















