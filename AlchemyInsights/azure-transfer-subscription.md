---
title: Azure faturalama sahipliğini aktarma
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
- "6849"
ms.openlocfilehash: 803d0105ad2bbaf2b18cea6aa556b6af5e09cb2d41812d4747aa703e6e7d7780
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54036116"
---
# <a name="transfer-azure-billing-ownership"></a>Azure faturalama sahipliğini aktarma

Aktarmak istediğiniz aboneliği içeren faturalama hesabının yöneticisi olarak [Azure portal](https://portal.azure.com/)'da oturum açın. Yönetici olup olmadığınızdan emin değilseniz veya yöneticinin kim olduğunu belirlemeniz gerekiyorsa [Hesap faturalama yöneticisini belirleme](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa) konusuna bakın.

1. _Maliyet Yönetimi + Faturalama_ için arama yapın.
1. Sol bölmeden **Abonelikler** seçeneğini belirleyin. Erişime bağlı olarak, bir faturalama kapsamı ve ardından **Abonelikler** veya **Azure abonelikleri**'ni seçmeniz gerekebilir.
1. Aktarmak istediğiniz abonelik için **Faturalama sahipliğini aktar**'ı seçin.
1. Aboneliğin yeni sahibi olacak hesabın faturalama yöneticisi olan bir kullanıcının e-posta adresini girin ve **Aktarım isteği gönder** seçeneğini belirleyin.
1. Kullanıcı, aktarım isteğinizi incelemek üzere yönergeler içeren bir e-posta alır. Aktarım isteğini onaylamak için kullanıcı, e-postadaki bağlantıyı seçer ve yönergeleri izler.

Aboneliğinizin faturalama sahipliğini, başka bir Azure Active Directory kiracısındaki kullanıcının hesabına aktarırsanız abonelikteki kaynakları yönetmek üzere kullanılan tüm [rol tabanlı erişim denetimi (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) atamalarının kalıcı olarak kaldırılacağını lütfen unutmayın. Abonelikteki kaynakları yönetme erişimi, yalnızca yeni sahipte bulunur. Bir abonelik için dizin değiştirme hakkında daha fazla bilgi için [Başka bir Azure Active Directory kiracısındaki kullanıcıya abonelik aktarma](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support) konusuna bakın.

_**Faturalarınız üzerindeki önemli etki**_: Bir Azure aboneliğinin faturalama sahipliğini aktardıysanız ücretleriniz eşit aralıklarla uygulanır. Faturalara, aşağıdakilere göre erişebilirsiniz:  

1. Aboneliğinizi, Azure portalındaki  [Abonelikler sayfasında](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade)   [faturalara erişime sahip bir kullanıcı](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support) olarak belirleyin, ardından  **Faturalar**'ı seçin.
1. PDF faturanızın bir kopyasını görüntülemek için  **Faturayı İndir** 'e tıklayın.  _Kullanılamaz_ ifadesini görüyorsanız  [Son faturalama dönemine ait bir faturayı neden görmüyorum?](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice) konusuna bakın.
1. Faturanızın bir PDF'ini ve ayrıntılı günlük kullanım dosyanızın (.CSV) bir kopyasını edinmek için **faturalama dönemi** seçeneğine tıklayarak günlük kullanımınızı da görüntüleyebilirsiniz. Daha fazla bilgi için  [Fatura ve kullanım verilerini alma](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support) konusuna bakın.

**Önerilen Belgeler**

- [Bir Azure aboneliğinin faturalama sahipliğini başka bir hesaba aktarma](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [Bir Azure aboneliğinin faturalama sahipliğini aktarma hakkında](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [Visual Studio, Microsoft İş Ortağı Ağı (MPN) ve Kullandıkça öde Geliştirme/Test aboneliklerini aktarma](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Sahiplik Aktarma hakkında SSS](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Sahiplik aktarma ile ilgili sorunları giderme](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
