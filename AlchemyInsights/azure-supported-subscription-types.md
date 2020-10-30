---
title: Desteklenen Abonelik türleri
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
- "9003560"
- "6675"
ms.openlocfilehash: 46bc60435c3f8477e9f274d90c39d0f1c6a523c6
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/28/2020
ms.locfileid: "48807983"
---
# <a name="supported-subscription-types"></a>Desteklenen Abonelik türleri

Devam etmek için lütfen desteklenen abonelik türlerini gözden geçirin.

[Desteklenen Abonelik türleri](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#supported-subscription-types)

**Fatura sahipliğini aktarma**

Aboneliğinizi aktarmak istediğiniz aboneliği içeren faturalandırma hesabının [Hesap Yöneticisi](https://ms.portal.azure.com/) olarak Azure portalı

- **Maliyet yönetimi + faturalamayla** arama yapın. Sol bölmeden **abonelikler** 'i seçin. Erişime bağlı olarak, bir faturalandırma kapsamı ve ardından **abonelikler** veya **Azure abonelikleri** 'ni seçmeniz gerekebilir.
- Aktarmak istediğiniz aboneliğin faturalama sahibini aktarma seçeneğini belirleyin
- Aboneliğin yeni sahibi olacak hesabın faturalama yöneticisi olan bir kullanıcının e-posta adresini girin ve ardından **aktarım isteği gönder** 'i seçin
- Kullanıcı, aktarım isteğinizi gözden geçirmeniz için yönergeler içeren bir e-posta alır. Aktarım isteğini onaylamak için kullanıcı e-postadaki bağlantıyı seçer ve yönergeleri izler.

Not: aboneliğinizin fatura sahipliğini başka bir Azure AD kiracısındaki bir kullanıcının hesabına aktarırsanız, abonelikteki kaynakları yönetmek için tüm [rol tabanlı erişim denetimi (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) atamaları kalıcı olarak kaldırılır. Yalnızca yeni sahibin abonelikteki kaynakları yönetme erişimi olur. Daha fazla bilgi için, [başka bir Azure AD kiracısındaki bir kullanıcıya abonelik aktarma](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support)konusuna bakın.

**Aboneliğin sahipliğini aktarma**

Aboneliğin kaynaklarını yönetmek için abonelik sahipliği aktarma önkoşulları rol tabanlı Access (RBAC) erişimleri kaybolur. Kiracıya var olan bir aboneliği ekleme hakkında daha fazla bilgi için [Azure Active Directory 'ye Azure aboneliği ilişkilendirme veya ekleme](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory?WT.mc_id=Portal-Microsoft_Azure_Support)konusuna bakın.

- Geçerli fatura döngüden mevcut bir bekleyen tutarla abonelik transferi yeni hesaptaki yeni ödeme gerecini aktarmayacaktır. Yeni hesaptaki kullanıcıların kullanabildiği tek bilgi, aboneliğiniz için geçen ayın maliyetidir. Kalan kullanım ve faturalandırma geçmişi abonelikle aktarılmaz.
- Kurumsal Sözleşme (EA) aboneliklerinin fatura sahipliğini aktarma Şu anda yalnızca Kurumsal Sözleşme portalında desteklenmektedir
- Visual Studio, BizSpark, Microsoft Iş ortağı ağı gibi kredi yönelimli bir aboneliği aktarmak, yeni bir kullanıcıya
- Sanal makineler, diskler ve Web siteleri gibi tüm kaynaklar yeni hesaba başarıyla aktarılır. Aşağıdaki kaynaklar çapraz kiracı aboneliği aktarımında etkilenebilir:

**Azure AD etki alanı Hizmetleri**

Azure Anahtar Kasası

- [SQL ilişkili kullanıcılar ve veritabanları](https://docs.microsoft.com/azure/sql-database/sql-database-aad-authentication-configure?WT.mc_id=Portal-Microsoft_Azure_Support) , özellikle de müşteri Azure Active Directory ile ilgili kimlik doğrulama kullandığında etkilenebilir
- Azure Active Directory kimlik doğrulamasıyla yapılandırılan **uygulama hizmetleri** etkilenebilir
- **Visual Studio ekibi** Azure abonelikleri 'ne bağlı hizmetler, bağlı Azure aboneliği iptal edildiğinde geçici olarak erişimi kaybedebilir

**Önerilen belgeler**

Faturalama sahipliği kabul edildikten sonraki adımlar:

- Fatura sahipliğini korumak, ancak aboneliğinizin türünü değiştirmek için, bkz: [Azure aboneliğinizi başka bir teklife geçme](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Visual Studio, Microsoft Iş ortağı ağı (MPN) ve siz kullandıkça öde dev/test abonelikleri aktarılıyor](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Kurumsal Sözleşme (EA) aboneliklerinin fatura sahipliğini aktarma](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transfer-billing-ownership-of-enterprise-agreement-ea-subscriptions)
- [Sahiplik aktarma SSS](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Aktarım sahipliği sorunlarını giderme](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)