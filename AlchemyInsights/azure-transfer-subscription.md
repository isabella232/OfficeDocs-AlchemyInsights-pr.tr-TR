---
title: Azure Faturalandırma sahipliğini aktarma
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
- "6849"
ms.openlocfilehash: e9a1e74b321e2c2dda5f7a4f69681a0acf0635d5
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 11/03/2020
ms.locfileid: "48922173"
---
# <a name="transfer-azure-billing-ownership"></a>Azure Faturalandırma sahipliğini aktarma

Aktarmak istediğiniz aboneliğin bulunduğu faturalandırma hesabının Yöneticisi olarak [Azure portalında](https://portal.azure.com/) oturum açın. Yönetici olduğunuzdan emin değilseniz veya kim olduğunu belirlemeniz gerekiyorsa, [Hesap faturalandırma yöneticisini belirleme](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa)konusuna bakın.

- **Maliyet yönetimi + faturalamayla** arama yapın.
- Sol bölmeden **abonelikler** 'i seçin. Erişime bağlı olarak, bir faturalandırma kapsamı ve ardından **abonelikler** veya **Azure abonelikleri** 'ni seçmeniz gerekebilir.
- Aktarmak istediğiniz aboneliğin **Faturalama sahibini aktarma** seçeneğini belirleyin
- Aboneliğin yeni sahibi olacak hesabın faturalama yöneticisi olan bir kullanıcının e-posta adresini girin ve ardından **aktarım isteği gönder** 'i seçin
- Kullanıcı, aktarım isteğinizi gözden geçirmeniz için yönergeler içeren bir e-posta alır. Aktarım isteğini onaylamak için kullanıcı e-postadaki bağlantıyı seçer ve yönergeleri izler.

**Not** : aboneliğinizin fatura sahipliğini başka BIR Azure AD kiracısındaki bir kullanıcının hesabına aktarırsanız, abonelikteki kaynakları yönetmek için tüm [rol tabanlı ERIŞIM denetimi (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)atamaları kalıcı olarak kaldırılır. Yalnızca yeni sahibin abonelikteki kaynakları yönetme erişimi olur. Daha fazla bilgi için, [başka bir Azure AD kiracısındaki bir kullanıcıya abonelik aktarma](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support)konusuna bakın.

**Önerilen belgeler**

- [Azure aboneliğinin fatura sahipliğini başka bir hesaba aktarma](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [Bir Azure aboneliği için fatura sahipliğini aktarma hakkında](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [Visual Studio, Microsoft Iş ortağı ağı (MPN) ve siz kullandıkça öde dev/test abonelikleri aktarılıyor](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Sahiplik aktarma SSS](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Aktarım sahipliği sorunlarını giderme](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
