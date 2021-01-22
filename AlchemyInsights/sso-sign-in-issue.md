---
title: Sorunsuz SSO kullanıcı oturum açma sorunları
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "7811"
ms.openlocfilehash: 347ef8f8176583f2a7c15fa82435eeb118b58c39
ms.sourcegitcommit: 67c873fa6e23ec39a826d60ac830969073bf79e1
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935216"
---
# <a name="seamless-sso-user-sign-in-issues"></a>Sorunsuz SSO kullanıcı oturum açma sorunları

Kullanıcının kimliği doğrulandıktan sonra, tarayıcı kullanıcının kimlik bilgilerini önbelleğe alar, böylece aynı tarayıcıda uygulama otomatik olarak aynı hesapla oturum açılır. Bu, başka bir kullanıcının veya tek bir kullanıcının bir cihazda birden çok hesapta oturum açmalarını zorlaştırabilirsiniz. Bunu çözmek için: 1. Başka bir tarayıcıda oturum açmayı deneyin. 2. Tarayıcının önbelleğini ve/veya tanımlama bilgilerini temizleyin ve yeniden oturum açmayı deneyin.

Hala oturum açma sorunları yaşıyorsanız, çözüm adımlarını tanılamak ve otomatikleştirmek için aşağıdaki adımları öneririz:

1. Azure [portalında test deneyimini kullanırken daha iyi](https://docs.microsoft.com/azure/active-directory/manage-apps/access-panel-extension-problem-installing) tanı ve çözüm sağlamak için Azure Active Directory'ye (Azure AD) yardımcı olması için Uygulamalarım Güvenli Tarayıcı Uzantısı'ı yükleyin.
2. Azure portalında uygulama yapılandırma sayfasındaki test deneyimini kullanarak hatayı yeniden üretin. Daha fazla bilgi edinmek için bkz. [SAML tabanlı çoklu oturum açma](https://docs.microsoft.com/azure/active-directory/azuread-dev/howto-v1-debug-saml-sso-issues)uygulamalarında Hata Ayıklama.
3. Uygulamalarım Güvenli Tarayıcı Uzantısı ile Azure portalında test deneyimini kullanırsanız, **4. adımı atlayabilirsiniz.**
4. SAML tabanlı çoklu oturum açma yapılandırma sayfasını açmak için:
    - Azure [portalını açın](https://portal.azure.com/) ve Genel Yönetici **veya** **Coadmin olarak oturum açın.**
    - Ana sol **gezinti menüsünün** en üstünde **Tüm** hizmetler'i seçerek Azure Active Directory Uzantısını açın.
    - Filtre arama kutusuna "Azure Active Directory" yazın ve **Azure Active Directory öğesini** seçin.
    - Azure Active **Directory** sol gezinti menüsünden Kurumsal Uygulamalar'ı seçin.
    - Tüm **uygulamalarınızı** görüntülemek için Tüm Uygulamalar'ı seçin. Burada göstermek istediğiniz uygulamayı görmüyorsanız, Tüm Uygulamalar  Listesi'nin en  üstünde yer alan Filtre denetimi kullanın ve Göster seçeneğini Tüm **Uygulamalar** olarak **ayarlayın.**
    - Çoklu oturum açma için yapılandırmak istediğiniz uygulamayı seçin.
    - Uygulama yüklenirken, **uygulamanın sol gezinti** menüsünde Çoklu oturum açma seçeneğini belirleyin.
    - **SAML tabanlı SSO'ya seçin.**
5. Hataya bağlı olarak, izlanması önerilen adımlar hakkında daha fazla bilgi edinmek için BKZ. SAML tabanlı çoklu oturum açma yapılandırılmış uygulamalarda oturum açma [sorunları.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#application-not-found-in-directory)
6. Diğer kullanıcı oturum açma sorunlarını gidermek için aşağıdaki kılavuza bakın:
    - [Tek Sign-On SAML protokolü](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol)
    - [Nasıl kullanılır: Azure Active Directory raporlarını kullanarak oturum açma hatalarında sorun giderme](https://docs.microsoft.com/azure/active-directory/reports-monitoring/howto-troubleshoot-sign-in-errors)
    - [Beklenmeyen izin istemi](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt)
    - [Kullanıcı izni hatası](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)
    - [Uygulamalarım'da oturum a açma sorunları](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel)
    - [Uygulama oturum açma sayfasında hata](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-application-error)
    - [Microsoft Uygulamasında oturum açma sorunu](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft)
