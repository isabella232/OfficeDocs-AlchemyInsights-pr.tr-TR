---
title: Desteklenen abonelik türleri
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003560"
- "6675"
ms.openlocfilehash: dcf5855bff8725ea746196c1f07d689ce1797f8c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820702"
---
# <a name="supported-subscription-types"></a>Desteklenen abonelik türleri

Daha fazla bilgi için lütfen desteklenen abonelik türlerini gözden geçin.

[Desteklenen abonelik türleri](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#supported-subscription-types)

**Fatura sahipliğini aktar**

Azure [portal'da, aktarımını](https://ms.portal.azure.com/) istediğiniz aboneliğin olduğu fatura hesabının Hesap Yöneticisi olarak

- **Maliyet Yönetimi + Faturalama**'da arama yapın. Sol **bölmeden** Abonelikler'i seçin. Erişime bağlı olarak, bir faturalama kapsamı ve ardından **Abonelikler** veya **Azure abonelikleri**'ni seçmeniz gerekebilir.
- Aktarımını istediğiniz abonelik için Fatura sahipliğini aktar'ı seçin
- Aboneliğin yeni sahibi olacak hesabın faturalama yöneticisi olan kullanıcının e-posta adresini girin ve aktarım isteği **gönder'i seçin**
- Kullanıcı, aktarım isteğinizi incelemek üzere yönergeler içeren bir e-posta alır. Aktarım isteğini onaylamak için kullanıcı, e-postadaki bağlantıyı seçer ve yönergeleri izler.

Not: Aboneliğinizin fatura sahipliğini başka bir Azure AD kiracısında kullanıcının hesabına aktarıyorsanız, abonelikte kaynakları yönetmeye yönelik tüm rol tabanlı erişim [denetimi (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) atamaları kalıcı olarak kaldırılır. Abonelikteki kaynakları yönetme erişimi, yalnızca yeni sahipte bulunur. Daha fazla bilgi için [bkz. Başka bir Azure AD kiracısı üzerinden kullanıcıya abonelik aktarma.](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support)

**Aboneliğin Sahipliğini Aktarma**

Abonelik Sahipliği Aktarım önkoşulları, abonelikte kaynakları yönetmek için rol tabanlı erişim (RBAC) erişimi kaybeder. Var olan bir aboneliği bir kiracıya ekleme hakkında daha fazla bilgi için bkz. Azure aboneliğini [Azure Active Directory'ye ilişkilendirme veya ekleme.](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory?WT.mc_id=Portal-Microsoft_Azure_Support)

- Mevcut faturalandırma döneminden devreden bir miktarla Abonelik Aktarımı yeni hesapta yeni ödeme aracına aktarlanmaz. Yeni hesapta kullanıcılara kullanılabilen tek bilgi, aboneliğinizin geçen ayki maliyetidir. Kullanım ve faturalama geçmişinin kalan kalanı abonelikle birlikte aktarlanmaz.
- Kurumsal Sözleşme (EA) aboneliklerinin fatura sahipliğini aktarma şu anda yalnızca Kurumsal Sözleşme Portalında desteklenmemektedir
- Visual Studio, BizSpark, Microsoft İş Ortağı Ağı gibi kredi odaklı bir aboneliği yeni bir kullanıcıya aktarmak için, aktarım isteğini kabul etmek için Visual Studio/Microsoft iş ortağı ağı lisansının olması gerekir
- Sanal Makineler, diskler ve web siteleri gibi tüm kaynaklar yeni hesaba başarıyla aktarıldı. Aşağıdaki kaynaklar kiracılar arası abonelik aktarımında etkilenebilir:

**Azure AD Etki Alanı Hizmetleri**

Azure Anahtar Kasaları

- [Sql ile ilgili kullanıcılar ve veritabanları,](https://docs.microsoft.com/azure/sql-database/sql-database-aad-authentication-configure?WT.mc_id=Portal-Microsoft_Azure_Support) özellikle de müşterinin Azure Active Directory ile ilgili bir kimlik doğrulaması kullandığında etki etki
- Azure Active Directory kimlik doğrulamasıyla yapılandırılan **Uygulama** Hizmetleri etki etki olabilir
- **Visual Studio Ekibi** Azure aboneliklerine bağlı hizmet hesapları, bağlı Azure aboneliği iptal edilirken erişimi geçici olarak kaybedebilir

**Önerilen Belgeler**

Fatura sahipliğini kabul etme adımları:

- Fatura sahipliğini korumak ancak aboneliğinizin türünü değiştirmek için, bkz: [Azure aboneliğinizi başka bir teklife değiştirme](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Visual Studio, Microsoft İş Ortağı Ağı (MPN) ve Kullandıkça öde Geliştirme/Test aboneliklerini aktarma](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Kurumsal Sözleşme (EA) aboneliklerinin fatura sahipliğini aktarma](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transfer-billing-ownership-of-enterprise-agreement-ea-subscriptions)
- [Sahiplik Aktarma hakkında SSS](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Sahiplik aktarma ile ilgili sorunları giderme](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)