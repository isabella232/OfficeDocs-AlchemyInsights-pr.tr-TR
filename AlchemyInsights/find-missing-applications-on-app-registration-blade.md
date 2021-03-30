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
ms.openlocfilehash: 00b5821e2edad8b60ff60b1f85264d81c72277e4
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51405224"
---
# <a name="find-missing-applications-on-app-registration-blade"></a>Uygulama Kaydı blade'de eksik uygulamaları bulma

1. Uygulama Kaydı portalında uygulamaları bulamıyorum.

    Bir uygulama çok kiracılı bir uygulama ise ve başka bir kiracıda kaydedilmişse, Uygulama Kayıt Blade altında görüntülenmez. Bununla birlikte, kiracınıza erişildikten (izin alındıktan sonra) ve hizmet sorumlusu oluşturulduğunda Enterprise Applications blade altında bulabilirsiniz. Daha fazla bilgi için Azure AD& Microsoft kimlik platformunda Uygulamalar ve [hizmet sorumluları bilgilerine bakın.](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)
2. Yönetici olmasına rağmen Uygulama Kaydı blade'inde uygulamalar görüntüye alınamıyor.

    Lütfen Azure portalında doğru dizinde olduğundan emin olun.
3. Uygulamam Enterprise Applications blade altında listelenmiyor, ancak PowerShell komutunu sorgulayana kadar gösterilir.

    Bazen uygulamayı Azure portaldan sildikten sonra portalda gösterilemez, ancak tümüyle silinmemiş olabilir. Daha fazla bilgi için bkz.:
    - Daha önce silinmiş olan uygulamaların listesini alabilir ve Powershell komutunu kullanarak uygulamanın listede gösterip gösterildiğini **bakabilirsiniz: Get-AzureADDeletedApplication.** Daha fazla bilgi edinmek için [bkz. Get-AzureADDeletedApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/get-azureaddeletedapplication)
    - Uygulamayı tamamen kaldırmak için PowerShell'de şunları abilirsiniz: **Remove-AzureADApplication -ObjectId.** Daha fazla bilgi edinmek için [remove-AzureADApplication (AzureAD) bakın.](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplication)
    - Alternatif olarak, şu Powershell komutunu kullanarak silinen uygulamayı geri yüklemeyi **abilirsiniz: AzureADDeletedApplication -ObjectId'yi Geri Yükleme.** Daha fazla bilgi edinmek için [restore-AzureADDeletedApplication (AzureAD) bakın.](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication)
4. Yeni Azure kiracımda önceden yüklenmiş tüm kurumsal uygulamaların listesini bulamıyorum.

    Azure AD'de varsayılan olarak önceden yüklenmiş kurumsal uygulama yoktur. Azure AD galerisinden göz atarak veya galeri dışı bir uygulama ekleyebilirsiniz. Daha fazla bilgi edinmek için [bkz. Hızlı Başlangıç: Azure Active Directory (Azure AD) kiracınıza uygulama ekleme.](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal)
    Genel yöneticiyseniz, Microsoft 365 Uygulama Başlatıcısı'nı [kullanarak uygulamalarınıza kolayca erişebilirsiniz.](https://docs.microsoft.com/microsoft-365/admin/manage/customize-the-app-launcher)
5. Uygulamalarım portalında uygulamalarım bulunamıyor.

    Uygulamalarım koleksiyonu sayfasında uygulamaların gizlenmey olduğundan emin olun. Daha fazla bilgi edinmek için [Uygulamalarım portalında (Azure AD) Koleksiyonlar'a (önizleme) bakın.](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-user-collections)
6. Uygulamalarım portalında uygulamaları başlatmak için Bkz. Uygulamalarım & uygulamaları kullanma hakkında bilgi edinin [- Azure AD.](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-end-user-access)
7. Office 365 Mover uygulaması, yüklemeden sonra Enterprise Applications blade'de görünmüyor.

    "Office 365 Mover" uygulaması, Kurumsal Uygulama Kaydı altındaki Galeri Uygulamaları bölümü kullanılarak AAD'ye eklenmek zorunda olmayan çok amaçlı bir uygulamadır. Office 365 Mover uygulamasına erişmek için, uygulamada oturum açmanız yeterli olur ve kullanıcıdan izinler için onay istemesi yeterli olur. Kullanıcı izin verdi mi, bu uygulama oturum açtığınız e-posta kimliğiyle kiracıya otomatik olarak eklenir.

    Uygulamada oturum açma sonrasında, bu uygulamanın girdisini AAD'de Enterprise Applications'ın blade'inde bulabilirsiniz. Tam adı yazarak (örneğin, "Office 365 Taşımacısı" yazarak veya "office" aramasıyla) bu uygulamayı arayabilirsiniz; uygulama listelesin. Daha fazla bilgi edinmek [için, Office 365 Taşımacı'nın](https://docs.microsoft.com/answers/questions/30186/office-365-mover-says-its-already-installed-but-it.html)zaten yüklü olduğunu ancak Kurumsal Uygulama galerisinde listelenmiyor olduğunu söylüyor.
8. Hızlı Başlangıç: Kimlik yönetimi için Azure Active Directory (Azure AD) kiracınızı kullanan uygulamaların listesini görüntülemek, Azure AD kiracınızı Kimlik Sağlayıcısı [(IdP)](https://docs.microsoft.com/azure/active-directory/manage-apps/view-applications-portal) olarak kullanmak üzere önceden ayarlanmış uygulamalar olarak da bilinen uygulamaları nasıl görüntüleymenizi gösterir.
9. [Azure Active Directory'ye uygulama ekleme veya](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-adding-apps) kaldırmayla ilgili genel sorunları gidermek, azure Active Directory'de uygulama görüntülemeyle ilgili olarak karşılaşılan yaygın sorunları anlamanıza yardımcı olur.
