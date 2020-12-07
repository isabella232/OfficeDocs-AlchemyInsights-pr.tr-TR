---
title: Azure AD Connect'te parola geri yazmayı etkinleştirme
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002933"
- "5615"
ms.openlocfilehash: 0eecd89b2558359702935379d7ffbd8b7508f4cd
ms.sourcegitcommit: 62a83a1c6bd9779a1a11b749490bd11670d4b063
ms.translationtype: HT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/02/2020
ms.locfileid: "49560460"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a>Azure AD Connect'te parola geri yazmayı etkinleştirme

Self servis parola sıfırlama geri yazmayı etkinleştirmek için önce Azure AD Connect'te geri yazma seçeneğini etkinleştirin. Azure AD Connect sunucusunda aşağıdaki adımları tamamlayın:

1. Azure AD Connect sunucunuzda oturum açıp **Azure AD Connect** yapılandırma sihirbazını başlatın.
2. **Hoş Geldiniz** sayfasında, **Yapılandır**'ı tıklayın.
3. **Ek görevler** sayfasında **Eşitleme seçeneklerini özelleştir**'i seçin ve ardından **İleri**'ye tıklayın.
4. **Azure AD'ye Bağlanma** sayfasında Azure kiracınız için genel yönetici kimlik bilgisi girin ve ardından **İleri**'ye tıklayın.
5. **Dizinlere bağlanma** ve **Etki Alanı/OU** filtreleme sayfalarında **İleri**'ye tıklayın.
6. **İsteğe bağlı özellikler** sayfasında **Parola geri yazma**'nın yanında bulunan kutuyu seçin ve **İleri**'ye tıklayın.
7. **Yapılandırmaya hazır** sayfasında **Yapılandır**'a tıklayıp işlemin bitmesini bekleyin.
8. Yapılandırmanın bittiğini gördüğünüzde **Çıkış**'a tıklayın.

Azure AD Connect'te parola geri yazma etkinleştirildiğinde, geri yazma için Azure AD SSPR'yi yapılandırın.  SSPR'de parola geri yazmayı etkinleştirmek için aşağıdaki adımları tamamlayın:

1. Genel yönetici hesabınızı kullanarak Azure portal'da oturum açın.
2. **Azure Active Directory**'yi arayıp seçin, **Parolayı sıfırla**'yı tıklayın, ardından **Şirket İçi tümleştirme**'yi tıklayın.
3. **Şirket içi dizininizde parola geri yazılsın mı?** seçeneğini **Evet** olarak ayarlayın.
4. **Kullanıcıların, parolalarını sıfırlamadan hesaplarının kilidini açmasına izin verilsin mi?** seçeneğini **Evet** olarak ayarlayın.
5. Hazır olduğunuzda **Kaydet**’i tıklayın.

Daha fazla bilgi için bkz. [Şirket içi bir ortama Azure Active Directory self servis parola sıfırlama geri yazma özelliğini etkinleştirme.](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).

> [!NOTE]
>  Yönetici, Azure Portal'da bir kullanıcının parolasını sıfırladığında, kullanıcı şirket dışındansa veya parola karması eşitlenmişse, parola şirket içi bir ortama geri yazılır. Bu işlev şu anda Office Yönetici portalında desteklenmemektedir.