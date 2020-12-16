---
title: Aktarma hizmetleri-tüm RDFE hizmetlerini başka bir aboneliğe taşıma
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
- "9004116"
- "7196"
ms.openlocfilehash: d6744484fe42f09f03de562a00fd56712607d418
ms.sourcegitcommit: ec88047d550006a1df4b6f10a3f513218113b9a5
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/15/2020
ms.locfileid: "49692180"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a>Aktarma hizmetleri-tüm RDFE hizmetlerini başka bir aboneliğe taşıma

**Kaynakları taşıma**

Azure kaynakları, Azure portalı, Azure PowerShell, Azure CLı veya REST API 'yi kullanan aynı aboneliğin altındaki başka bir Azure aboneliğine veya kaynak grubuna geçebilir.

Kaynakları taşıyabilmek için önce bkz:

- [Kaynakları taşımadan önce denetim listesi](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [Taşınamayan hizmetler](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Taşıma nasıl doğrulanır](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [Hizmetler için kılavuzu taşıma](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

Var olan kaynakları başka bir kaynak grubuna veya aboneliğe taşımak için şunları kullanabilirsiniz:

- [Azure portalı](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [Azure PowerShell](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [Azure CLı](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [REST APı 'SI](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

Öğretici: [Azure kaynaklarını başka bir kaynak grubuna veya aboneliğe taşıma](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)

**Azure Resource Manager ile ilgili sorunları giderme**

Bazı yaygın Azure dağıtım hatalarını öğrenmek ve bunları çözmek için bilgi almak için aşağıdaki makalelere bakın. Dağıtım hatasının hata kodunu bulamazsanız, [hata kodu bul](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code)'a bakın.

- [Dağıtım hatalarını giderme](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [Azure kaynaklarını yeni kaynak grubuna veya aboneliğe taşıma sorunlarını giderme](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

Azure aboneliğinizi ücretsiz olarak öde-to-to-to-to-to-to-to-to-to-to-to-to-to-to-to-to-to-

- Ücretsiz deneme sürümünü güncelleştirmek için, [ücretsiz deneme sürenizi yükseltme veya Microsoft 'un size devam eden ödeme Için Azure aboneliğini yükseltme](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription)konusuna bakın.
- Bir Kullandıkça Öde hesabını değiştirmek için, bkz: [Azure öde-to](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer)-to-to-to-to-to-to-to-to-to

**Azure Active Directory kiracınıza bir Azure aboneliği eklemek veya ilişkilendirmek için:**

1. Oturum açın ve [Azure portalında abonelikler sayfasından](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade)kullanmak istediğiniz aboneliği seçin.
2. **Dizini Değiştir**'i seçin.
3. Görüntülenen tüm uyarıları gözden geçirin ve ardından **Değiştir**'i seçin.
4. Abonelik için Dizin değiştirilmiştir ve bir başarı iletisi alırsınız.
5. Yeni dizine gitmek için *Dizin* değiştiriciyi kullanın. Her şeyin düzgün görünmesi 10 dakika kadar sürebilir.

**Önerilen belgeler**

- [Azure aboneliğinin sahipliğini aktarma](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [Kaynakları yeni kaynak grubuna veya aboneliğe taşıma](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [Azure portalını kullanarak kaynakları yönetme](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
