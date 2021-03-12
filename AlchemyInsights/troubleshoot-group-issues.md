---
title: Grup sorunlarını giderme
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
- "7814"
- "9004358"
ms.openlocfilehash: 7e2957a27305e8fb0bfd10e21189cef9870c5aaa
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/18/2021
ms.locfileid: "50714444"
---
# <a name="troubleshoot-group-issues"></a>Grup sorunlarını giderme

**Bir grubu Azure AD rolüne atamam gerekiyor**

Azure AD rolüne Azure Active Directory (AD) grubu atamak için aşağıdaki adımları uygulayın:

1. Yeni grup oluşturma - Yeni grup oluşturmak için:

    a. Ayrıcalıklı rol yöneticisi veya genel yönetici izinleriyle Azure AD yönetim merkezinde oturum açın. 
    b. Azure Active Directory > Grupları'> Yeni > seçin. 
    c. Grubu oluşturun.

2. Rolü grup oluşturma sırasında veya grup oluşturulduktan sonra gruba attayin.

    a. Grup oluşturma sırasında gruba rol atamak için, iki durumlu Azure AD rollerini açıp gruba atanabilir ve grubu oluşturabilirsiniz.
    b. Oluşturulduktan sonra gruba rol atamak için, yeni oluşturulan grubun Atanan roller sekmesine gidin ve rolü gruba attayabilirsiniz.

**Azure AD rolüne atanan bir grubun üyeliğini yönetmem gerekiyor**

1. Ayrıcalık yükseltmesini önlemek için, varsayılan olarak yalnızca ayrıcalıklı rol yöneticisi ve genel yönetici role atanmış bir grubun üyeliğini değiştirebilir. Bununla birlikte, böyle bir gruba sahip atamayı seçebilir ve bu görev için temsilci atayın. Daha fazla bilgi için Azure [Active Directory'de rol atamalarını yönetmek için bulut gruplarını kullanma.](https://docs.microsoft.com/azure/active-directory/roles/groups-concept)
2. Azure AD'de gruplara rol atamaya yönelik sık sorulan sorular ve sorun giderme ipuçları için, bulut gruplarına atanan sorun [giderme rollerine bakın.](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting)

**Dinamik gruplar**

1. Yerleşik kullanıcı özniteliklerini bulamıyorsanız, özniteliğin desteklenen özellikler listesinde olduğundan emin olur.
2. Yerleşik cihaz özniteliklerini arıyorsanız, özniteliğin cihaz öznitelikleri listesinde olduğundan emin olun 
3. Yerleşik kullanıcı ve cihaz özniteliklerine ek olarak, Uzantı Özniteliklerini [de kullanabilirsiniz.](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership#extension-properties-and-custom-extension-properties) Şirket içi Windows Server AD'den veya bağlı bir SaaS uygulamasından uzantı özniteliklerini eşitledikten sonra, öznitelikler kural oluşturucus un açılan listesinde görünür olmalıdır. Özel öznitelik adı, PowerShell kullanarak kullanıcının özniteliği sorgulanır ve öznitelik adı aranarak dizinde bulunabilir. Bunlar, kural söz dizimsinde kurallar oluşturmada da kullanılabilir.
4. Kiracınıza uygun lisansa sahip olduğundan emin olmak. Dinamik gruplar için kiracının Azure AD P1 Premium lisansına sahip olduğu gerekir. Azure AD lisans planları listesine buradan [erişilebilir.](https://azure.microsoft.com/pricing/details/active-directory/) Enterprise Mobility + Security lisans planları burada [erişilebilir.](https://www.microsoft.com/microsoft-365/enterprise-mobility-security/compare-plans-and-pricing)
5. Dinamik grubu oluştururken kullanıcının rolünün genel yönetici, intune yöneticisi, grup yöneticisi veya kullanıcı yöneticisi olduğundan emin olmak.
6. Lütfen grubun doldurmak için zaman olmasına izin ver. Kiracının boyutuna bağlı olarak, grubun ilk kez veya kural değişikliği sonrasında doldurmak için 24 saat kadar sürebilir.
7. Daha fazla bilgi için [bkz. Dinamik grup üyeliği için öznitelik tabanlı kurallar oluşturma.](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership)

**Grubu silmem gerekiyor**

1. Gruplar, Azure AD Powershell modülünde Remove-AzureADGroup cmdlet'i kullanılarak dizinden silinebilir.
2. Azure AD'de eşitlenen bir grubu silmeyi denemeden önce, hatalardan kaçınmak için tüm atanmış lisansları sildikten emin olun.
3. Grupları silme hakkında daha fazla bilgi için bkz. [Atanmış lisansla grubu silme.](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced#deleting-a-group-with-an-assigned-license)

**Silinmiş bir grubu geri yüklemem gerekiyor**

1. Bir Office 365 grubu silinirse, kalıcı silme işleminin gerçekleşmesi için yalnızca 30 gün içinde geri yüklenebilir. Kalıcı olarak silindikten sonra, grup artık geri yüklenebilir. Grupları geri yükleme hakkında daha fazla bilgi edinmek için buraya [tıklayın.](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)
2. Bu işlev, güvenlik grupları ve dağıtım grupları için desteklenmiyor.
3. Bir Office 365 grubunu geri yükleme yetkinizin olduğundan emin olmak. Genel yöneticiler, grup yöneticileri, kullanıcı hesabı yöneticileri, intune hizmet yöneticileri, iş ortağı katman1 veya katman2 desteği ve grubun sahibi grubu geri yükleyebilir.
4. Dinamik grup silindiğinde ve geri yüklendiklerinden, yeni bir grup olarak görülür ve kurala göre yeniden doldurulur. Bu işlem 24 saat kadar sürebilir.
5. Silinmiş bir grubu geri yükleme hakkında daha fazla bilgi için Bkz. [Azure Active Directory'de silinmiş office 365 grubunu geri yükleme.](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)

**Grup süre sonu ilkesi yapılandırması**

1. Bu işlev yalnızca Office 365 grupları için desteklenitir; güvenlik grupları ve dağıtım grupları için desteklanmaz.
2. Office 365 gruplarının süre sonu ilkesi yapılandırma ve kullanma için Azure AD Premium lisansı gerekir.
3. Şu anda, kiracıda Office 365 grupları için tek bir süre sonu ilkesi yalndırıldı.
4. Yalnızca Genel yöneticiler, grup yöneticileri, kullanıcı yöneticileri ve grubun sahibi grubu yeniler.
5. Office 365 grubunun süresi dolduğunda, bu grup silinir ve kalıcı silme işleminin gerçekleşmesi için 30 gün içinde geri yüklenebilir. Kalıcı olarak silindikten sonra, grup artık geri yüklenebilir. Grupları geri yükleme hakkında daha fazla bilgi edinmek için buraya [tıklayın.](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)

**Etkinlik tabanlı otomatik yenileme**

SharePoint, Outlook ve Teams'den yapılan kullanıcı etkinlikleri, grup otomatik yenilemeyi tetikler. Etkinlikler, grubun süresi dolmadan 35 gün önce denetlenir. Geçerli grup yaşam döngüsü boyunca etkinlik varsa, grup otomatik olarak yenilenir ve grup sahiplerine e-posta bildirimi gönderilmez.

**Süresi dolan gruplar için bildirim zamanlaması**

1. E-posta bildirimleri Office 365 grup sahiplerine grubun sona erme tarihinden 30 gün, 15 gün ve 1 gün önce gönderilir.
2. Süre sonu ilk kez ayarlanıyorsa, sona erme aralığından daha eski olan tüm gruplar sona erme tarihine 35 gün olarak ayarlanır.
3. Grup son kullanma tarihi, ilkenin güncelleştirilmiş tarihine göre değil, grubun yenileme tarihine göre hesaplanır. Sona erme ilkesi güncelleştirilmişse, son kullanma tarihi değişmez.
4. Daha fazla bilgi için Bkz. Grup Süre Sonu ilkesi ve yenileme [e-postaları](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-lifecycle) ve Azure Active Directory'de silinmiş [office 365 grubunu geri yükleme.](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)

**Grup oluşturma izni**

Yeni grup oluşturma yetkinizin olduğundan emin olmak. Genel yöneticiler Azure portalında veya Erişim Paneli'nden grup oluşturma özelliğini devre dışı bırakabilirsiniz. Sizin için yeni grup oluşturmak veya size uygun izinler vermek için bir yöneticiye ihtiyacınız olabilir.

1. [Azure portalda yeni grup oluşturma ve üye ekleme](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-groups-create-azure-portal)
2. [Powershell MSOnline'da grup oluşturma](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#create-groups)
3. [PowerShell'de grup oluşturma özelliğini devre dışı bırakma](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#disable-group-creation-by-your-users) 
4. [Office 365'te kimlerin grup oluşturanı yönetme](https://docs.microsoft.com/microsoft-365/solutions/manage-creation-of-groups) 
5. [Powershell aracılığıyla Office 365 karşılama bildirimini devre dışı bırakma](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup)
6. [Azure AD yönetim rolleri](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)

**Grup oluşturma izinlerini yönetme**

1. Genel yöneticiler, Azure portallarında veya Access Panel'de oluşturulmuş güvenlik veya Office 365 grupları için grup oluşturma izinlerini yönetebilir. Bunun için, **Kullanıcılar Azure portallarında** güvenlik grupları oluşturabilir veya Kullanıcılar, Azure portalları ayarlarında Genel **(Ayarlar)**> Grupları'nda **Office 365** grupları oluşturabilir.
2. Ayrıca Azure AD P1 Premium lisansınız varsa, grup oluşturma seçeneğini kısıtlayan bir kullanıcı grubu da kullanabilirsiniz.

**Office 365 grubunun yeni üyeleri için hoş geldiniz bildirimini devre dışı bırakma**

Office 365 gruplarına eklenen kullanıcılara gönderilen karşılama `UnifiedGroupWelcomeMessageEnabled` bildirimi, Powershell'de **False ayarıyla devre** dışı bırakılabilir. Bu ayar hakkında bilgi edinmek için buraya [tıklayın.](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup)













