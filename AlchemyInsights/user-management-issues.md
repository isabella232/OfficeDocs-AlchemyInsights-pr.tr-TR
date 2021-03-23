---
title: Kullanıcı yönetimi sorunları
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
- "9209"
- "9005371"
ms.openlocfilehash: 4b61686381de0cafa38857ca7a96b3a81aa191ec
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037512"
---
# <a name="user-management-issues"></a>Kullanıcı yönetimi sorunları

**'Kullanıcı ataması gerekli' özelliğini devre dışı bırakarak (bu özelliği Hayır olarak ayarla) geçerli atanan kullanıcılara ne olur?**

Gerekli Kullanıcı **ataması devre dışı** bırakılama şu anda atanmış olan kullanıcıları ETKILEMEZ. Bu özelliği devre dışı bırakmak yalnızca tüm kullanıcıların uygulamaya erişmesine olanak sağlar. Listelenen tüm kullanıcılar ve uygulamanın gruplarına atanan kullanıcılar yine geçerli olacaktır.

- Uygulamanızı belirli kullanıcı kümesiyle kısıtlamak için bkz. - Azure AD uygulamasını bir kullanıcı kümesiyle kısıtlama [- Microsoft kimlik platformu | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-restrict-your-app-to-a-set-of-users#:~:text=Select%20the%20application%20you%20want%2cand%20set%20it%20to%20Yes.).
- Kullanıcıları ve grupları Azure Active Directory'de (Azure AD) kurumsal uygulamalara atamak için, Azure portaldan veya PowerShell kullanarak Azure Active Directory'de bir uygulama için kullanıcı atamalarını [yönetme'ye bakın.](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal)
- Uygulama oluşturma ve yönetim izinlerini temsilci olarak görmek için bkz. [Temsilci uygulama yönetimi yöneticisi izinleri - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/roles/delegate-app-roles).
- **Belirli kurumsal uygulamaları kullanıcılardan gizleme** - Aşağıdaki adımları kullanarak tüm Microsoft 365 uygulamalarını **Uygulamalarım panelinden** gizleyebilirsiniz. Uygulamalar, Office 365 portalında görünmeye devam eder.

 1. Dizininiz için genel yönetici olarak Azure portalında oturum açın. 
 2. **Azure Active Directory'yi seçin.** 
 3. **Kullanıcılar'ı seçin.** 
 4. Kullanıcı **ayarlarını seçin.** 
 5. Kurumsal **uygulamalar'ın altında,** **son kullanıcıların uygulamalarını başlatma ve görüntülemeyi yönet'e tıklayın.** 
 6. Kullanıcılar **Office 365 portalında yalnızca Office 365 uygulamalarını** görebilir, Evet'e **tıklayın.** 
 7. **Kaydet**’e tıklayın. 
 8. Daha fazla ayrıntı için bkz. Azure AD kurumsal [uygulamasında kullanıcının deneyiminden Kurumsal | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/manage-apps/hide-application-from-user-portal#:~:text=%20Hide%20an%20application%20from%20the%20end%20user,6%20Click%20Properties.%207%20Click%20Save.%20See%20More.)

- Birçok kuruluşa Hizmet Olarak Yazılım (SaaS) uygulaması sunuyorsanız, uygulamanızı herhangi bir Azure Active Directory (Azure AD) kiracısı üzerinden oturum açma kabul etmek üzere yapılandırabilirsiniz. Bu yapılandırmaya "uygulamanızı çok kiracılı yapma" denir. Herhangi bir Azure AD kiracısı kullanıcıları, kendi hesaplarını sizin uygulamanız ile kullanmaya izin verdikten sonra uygulamanıza oturum açabilecektir. Daha fazla bilgi için Azure [AD kullanıcılarında oturum açma uygulamaları oluşturma - Microsoft kimlik platformu | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant).

- **Son kullanıcı uygulamaya atandıktan sonra uygulamaya nasıl erişebilir?**

Enterprise application blade'daki her uygulamanın son kullanıcılara erişmesi için bir bağlantı vardır. Kullanıcılar uygulamaya Uygulamam portalı **üzerinden de** kolay bir şekilde erişebilirsiniz.

- **Kullanıcılar tarafından hangi uygulamaların ve uygulama türünün kullanılıyor olduğunu bilmek mi istiyor musunuz?**

Son 30 günlük oturum açma raporlarını Azure Active Directory portal.azure.com > oturum açma> raporları **> indirebilirsiniz.**

- Kiracı genelinde yönetici [iznini bir uygulamaya nasıl ver ve son](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) kullanıcıların uygulamalara nasıl izin ver olduğunu [yapılandırmayı öğrenin.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent)

- Onayın [nasıl çalıştığını anlama ve](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) [Uygulamalara onayı yönetme.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests)


