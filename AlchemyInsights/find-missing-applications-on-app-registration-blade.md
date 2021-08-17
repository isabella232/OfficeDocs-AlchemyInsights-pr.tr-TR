---
title: Uygulama Kayıt blade'inde eksik uygulamaları bulma
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9654"
ms.openlocfilehash: 0dee7e44a8701e1df924b9657cce6cf9d90160e58277d667f6069a4cbcf87ce5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54057122"
---
# <a name="find-missing-applications-on-app-registration-blade"></a>Uygulama Kayıt blade'inde eksik uygulamaları bulma

1. Uygulama Kaydı portalında uygulamaları bulamıyorum.

    Uygulama çok kiracılı bir uygulama ise ve başka bir kiracıda kaydedilmişse, Uygulama Kaydı blade altında görüntülenmez. Bununla birlikte, kiracınıza erişildikten (kabul edildikten sonra) ve hizmet sorumlusu oluşturulduktan sonra Enterprise Applications blade altında bulabilirsiniz. Daha fazla bilgi için [bkz. Azure AD'de & hizmet sorumlularını kullanma - Microsoft kimlik platformu.](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)
2. Yönetici olmasına rağmen Uygulama Kaydı blade içinde uygulamalar görüntüye alınamıyor.

    Lütfen Azure portalında doğru dizinde olduğundan emin olun.
3. Uygulamam Enterprise Applications blade altında listelenmiyor, ancak PowerShell komutunu sorgula kullanılırken gösterilir.

    Bazen, uygulamayı Azure portaldan sildikten sonra portalda gösterilemez, ancak tamamen silinmemiş olabilir. Daha fazla bilgi için bkz.:
    - Daha önce silinmiş olan uygulamaların listesini alabilir ve Powershell komutunu kullanarak uygulamanın listede gösterip görmediğini **bakabilirsiniz: Get-AzureADDeletedApplication**. Daha fazla bilgi edinmek için [bkz. Get-AzureADDeletedApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureaddeletedapplication).
    - Uygulamayı tamamen kaldırmak için PowerShell'de şunları denemeniz gerekir: **Remove-AzureADApplication -ObjectId.** Daha fazla bilgi edinmek için [bkz. Remove-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplication).
    - Alternatif olarak, şu Powershell komutunu kullanarak silinen uygulamayı geri yüklemeyi abilirsiniz: **AzureADDeletedApplication -ObjectId'i Geri Yükleme.** Daha fazla bilgi için [bkz. Restore-AzureADDeletedApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).
4. Yeni Azure kiracımda önceden yüklenmiş tüm kurumsal uygulamaların listesini bulamıyorum.

    Azure AD'de varsayılan olarak önceden yüklenmiş kurumsal uygulama yoktur. Azure AD galerisinden göz atarak veya galeri dışı bir uygulama ekleyebilirsiniz. Daha fazla bilgi edinmek için bkz. Hızlı Başlangıç: Azure Active Directory [(Azure AD) kiracınıza uygulama ekleme](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal).
    Genel yöneticiyseniz, uygulama başlatıcısını kullanarak uygulamalarınıza [Microsoft 365 erişebilirsiniz.](https://docs.microsoft.com/microsoft-365/admin/manage/customize-the-app-launcher)
5. Uygulamalarım portalında uygulamalarım bulunamıyor.

    Uygulamalarım koleksiyonu sayfasında uygulamaların gizlenmey olduğundan emin olun. Daha fazla bilgi edinmek için [Bkz. Uygulamalarım portalında (Azure AD)](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-user-collections)Koleksiyonlar (önizleme).
6. Uygulamalarım portalında uygulamaları başlatmak için bkz. [Uygulamalarım portalında &](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-end-user-access)bulma - Azure AD.
7. Office 365 Mover uygulaması, yüklemeden sonra Enterprise Blade üzerinde göster görünmüyor.

    "Office 365 Mover" uygulaması, Uygulama Kaydı'nın altındaki Galeri Uygulamaları bölümü kullanılarak AAD'ye eklenmek zorunda olmayan çok Enterprise uygulamadır. Mover Office 365 erişmek için, uygulamada oturum açın; kullanıcıdan izinler için izin istemesi yeterli olur. Kullanıcı izin verdi mi, bu uygulama oturum açtığınız e-posta kimliğiyle kiracıya otomatik olarak eklenir.

    Uygulamada oturum olduktan sonra, bu uygulamanın girdisini AAD'de Enterprise Applications'ın blade altında bulabilirsiniz. Tam adı yazarak (yani "Büyük Office 365 Taşı" olarak) ya da yalnızca "office" için arama yapmanız ve uygulamayı listele çalışması gerekir. Daha fazla bilgi edinmek Office 365 Taşımacı uygulamanın zaten yüklü olduğunu söylüyor ancak Uygulama [Galerisi'nde Enterprise bakın.](https://docs.microsoft.com/answers/questions/30186/office-365-mover-says-its-already-installed-but-it.html)
8. Hızlı Başlangıç: Kimlik yönetimi için Azure Active Directory (Azure AD) kiracınızı kullanan uygulamaların listesini görüntülemek, Azure AD kiracınızı Kimlik Sağlayıcısı [(IdP)](https://docs.microsoft.com/azure/active-directory/manage-apps/view-applications-portal) olarak kullanmak üzere önceden ayarlanmış olan uygulamaların nasıl görüntü olduğunu gösterir.
9. [Azure Active Directory uygulamasına uygulama](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-adding-apps) ekleme veya kaldırma ile ilgili yaygın sorun giderme, kullanıcıların uygulamaları aynı uygulamada görüntülerken karşılaşacakları yaygın sorunları anlamanıza Azure Active Directory.
