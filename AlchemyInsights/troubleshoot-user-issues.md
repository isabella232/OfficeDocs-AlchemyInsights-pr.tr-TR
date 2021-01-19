---
title: Kullanıcı sorunlarını giderme
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7813"
- "9004358"
ms.openlocfilehash: d9964e50bdea0c41ac14ab3783b579034b5f2c8c
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901341"
---
# <a name="announcements"></a>İlere

Uygulamalarınızın etkilenip etkilenmediğini test etmek için, test uyumluluğu hakkında Google 'ın yönergelerini izleyin. Google 'ın Kılavuzu https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support .

Tüketici Google hesaplarıyla kullanıcılarınıza oturum açarken System WebView veya sistem tarayıcısını kullandığınızdan emin olun. Daha fazla bilgi için, [yalnızca Chrome tarayıcısını kullanarak uygulamada oturum açma sorunları](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications)konusuna bakın.


**Azure AD dizininde yeni bir Kullanıcı oluşturamıyorum**

Azure AD 'de yeni bir Kullanıcı oluşturmamada sorun gidermek için aşağıdaki adımları uygulayın:

1. Yeni bir standart Kullanıcı oluşturma yetkiniz olduğundan emin olun. Yalnızca Azure Active Directory (AD) genel yöneticisi veya Kullanıcı Yöneticisi rolü yeni bir standart kullanıcı oluşturabilir. Bu rollerden birinde değilseniz, bir yöneticiden Bu rollerden birine eklemesini veya yeni kullanıcı hesabını oluşturmanızı isteyin.
2. Kullanıcı adının Azure AD 'inizde doğrulanan bir etki alanında olduğundan emin olun. Azure AD 'inizde hiçbir doğrulanmış özel etki alanı adı yoksa, *. onmicrosoft.com ile biten Azure AD başlangıç etki alanınızı kullanabilirsiniz.
3. Kullanıcı adının şirket içi AD 'dan Azure AD 'e federe olmayan bir etki alanında olduğundan emin olun. Kullanıcılar şirket içi içinden federe olan etki alanı adlarıyla buluta eklenemez.
4. Başka bir kullanıcının veya kişinin, yeni kullanıcıya atamak istediğiniz kullanıcı adına sahip olmadığından emin olun. Kullanıcı adları, Azure AD 'de benzersiz olmalıdır.
5. Azure AD 'inizde [Azure AD rollerine ve yöneticilerine](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) bakın.
6. Azure AD 'inizde [etki alanı adlarını](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Domains) görün.
7. Son oluşturduğunuz veya silinen bir kullanıcı hakkında, eylemi gerçekleştirmenin ne zaman olduğu gibi daha ayrıntılı bilgileri görmek için [Denetim günlüklerini](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Audit) gözden geçirin.
8. Yeni Kullanıcı ekleme hakkında daha fazla bilgi için [Azure AD 'nizde yeni bir kullanıcı oluşturmak üzere Azure Portal 'ı kullanma](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory) konusuna bakın.
9. Azure AD 'de yönetici rolü izinleri hakkında daha fazla bilgi için [Azure AD yönetim rollerine](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)bakın.
10. Azure AD PowerShell kullanarak bir Kullanıcı oluşturma hakkında ayrıntılı bilgi için, [Yeni Kullanıcı oluşturmak üzere Azure AD PowerShell](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser)bölümüne bakın.

**Self Servis kaydolma sorunu**

Self Servis kaydolma ile ilgili sorunları gidermek için aşağıdaki adımları uygulayın:

1. Uygulamalarınızla self servis kayıt özelliğini kullanmak için, önce kiracınıza self servis kaydolma özelliğini etkinleştirin. 
2. Uygulamanın self servis kaydolma özelliğini desteklemesi için Kullanıcı akışına ekleyin. Bu uygulamanın oturum açma sayfasına bir sonraki gidiişinizde bir seçenek **_hesap yok? Bir tane oluşturun!_* _. Bu, self servis kaydolma işlemini başlatır.
3. Azure AD 'de bir organizasyonu doldurmak üzere self servis kaydolma 'yı kullanma hakkında bilgi için, [Azure AD 'ye self servis kaydolma](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-self-service-signup)bölümüne bakın.
4. Bir veya daha fazla uygulamayla Kullanıcı akışını ilişkilendirdikten sonra, bu uygulamayı ziyaret eden kullanıcılar Kullanıcı akışında yapılandırılan seçenekleri kullanarak kayıt yapabilir ve Konuk hesabı edinebilir. Oturum açma ve Konuk hesabı kazanma hakkında daha fazla bilgi için, kullanıcılar [Konuk kullanıcıları Için self servis kayıt](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-user-flow)bilgilerini görebilir.

_ *Dış kullanıcıyı davet etme sorunu**

Dış kullanıcıyı davet etme ile ilgili sorunları gidermek için aşağıdaki adımları uygulayın:

Kullanıcının daveti olarak kullanıcının oturum açtığında kullandığı e-posta adresine bir Kullanıcı daveti yolladığınızdan emin olun. Daveti bir kullanıcının proxy e-posta adresine gönderirseniz, Kullanıcı bunu açamaz. Daha fazla bilgi için [Azure AD B2B belgelerine](https://docs.microsoft.com/azure/active-directory/external-identities/)bakın.

**Kullanıcıya lisans atayamaz**

Bir kullanıcıya lisans atama konusundaki sorunları gidermek için aşağıdaki adımları uygulayın:

1. Kullanıcı lisanslarını yönetmek için, gerekli yönetici rollerinden biriyle bir hesap kullandığınızdan emin olun: genel yönetici, Lisans Yöneticisi veya Kullanıcı Yöneticisi. Kullanıcının rolünü Kullanıcı dikey sekmesinin **Dizin rolü** sekmesinde denetleyebilirsiniz.
2. Azure Portal 'ı ve lisans atamasını kullanıyorsanız, sağ üst köşedeki bildirime tıklayın. Bu, yanlış olan neyin ayrıntılarını içeren bir blade açar. Çoğu durumda sorunu anlayabilmek ve çözmek yeterlidir.
3. Lisans bir kullanıcıya atanmadan önce Kullanıcı için **Kullanım konumu** özelliğinin ayarlandığından emin olun. Kullanıcı dikey penceresinde **profil** sekmesini görüntüleyerek kullanıcının bu özelliği ayarlandığını doğrulayın.
4. Atamaya çalıştığınız ürün için yeterli lisans olduğundan emin olun. Azure portalında kullanılabilen lisansların sayısını, [Azure Active Directory-> lisanları > tüm ürünleri](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/LicensesMenuBlade/Products)görebilirsiniz.
5. Kullanıcının, atamak istediğiniz yeni lisansınızla çakışan başka lisansı var. Örneğin, kullanıcının Exchange Online (plan 1) hizmeti etkinse, Exchange Online (plan 2) ile lisans atayamazsınız. Yeni lisans atamasına izin vermek için hizmetlerden birini devre dışı bırakın. Azure portalını veya PowerShell cmdlet 'lerini kullanıyorsanız, **Sorun ayrıntıları** sayfasında çakışmaya neden olan hizmetler listelenir.
6. Bir lisansı kaldırmaya çalışıyorsanız ve başarısız olan kullanıcının, kaldırmaya çalıştığınız hizmetlere bağlı başka lisansları olabilir. Azure portalını veya PowerShell cmdlet 'lerini kullanıyorsanız, hata iletisi bağımlılıkları olan belirli hizmetleri listeler.
7. Bir kullanıcıya bir lisansın neden eklendiğini/kaldırıldığını öğrenmek istiyorsanız (örneğin, kuruluşunuzda başka bir değişiklik yapmış olabilir), denetim günlüklerine bakın. Tüm değişiklikleri göstermek için filtreyi **Lisans aktivitelerine** ayarlayın; bu, bunları gerçekleştiren "aktör" de dahildir.
8. Exchange Online kullanıyorsanız, kiracınızdaki bazı kullanıcılar aynı proxy adresi değeriyle yanlış yapılandırılmış olabilir. Bu tür durumlarda, lisans işlemi başarısız olduğunda genel hata iletileri görebilirsiniz. [Bu makale](https://docs.microsoft.com/exchange/troubleshoot/administration/proxy-address-being-used) , [uzak PowerShell kullanarak Exchange Online 'a bağlanma](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)hakkında bilgi içeren bu sorun hakkında daha fazla bilgi içermektedir. Kiracınızda hangi kullanıcıların aynı proxy adresini içerdiğini belirlemek için, bu Exchange Online cmdlet 'ini yürütün:

Zamanında

Get-Recipient | WHERE {$ _. Tam adresler-eşleşme <user principal name> } | fL ad, alıcının türü, emailaadresler





