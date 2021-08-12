---
title: Aktarım Hizmetleri - Tüm RDFE hizmetlerini başka bir aboneliğe taşıma
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
ms.openlocfilehash: 89217922b8b51f2548f9fff53bf80364c0e897b1d9b34bfb7016f0b0f197cf17
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53940113"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a>Aktarım Hizmetleri - Tüm RDFE hizmetlerini başka bir aboneliğe taşıma

**Kaynakları taşıma**

Azure kaynakları, kaynakları taşımak için Azure portalı, Azure PowerShell, Azure CLI veya REST API kullanılarak, aynı abonelik kapsamındaki başka bir Azure aboneliğine veya kaynak grubuna taşınabilirsiniz.

Kaynakları taşımadan önce bkz:

- [Kaynakları taşımadan önce denetim listesi](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [Taşınabilirsiniz hizmetler](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Taşımayı doğrulama](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [Hizmetler için taşıma kılavuzu](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

Var olan kaynakları başka bir kaynak grubuna veya aboneliğe taşımak için şunları kullanabilirsiniz:

- [Azure portalı](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [Azure PowerShell](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [Azure CLI](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [REST API](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

Öğretici: [Azure kaynaklarını başka bir kaynak grubuna veya aboneliğine taşıma](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)

**Azure Kaynak Yöneticisi ile hataları giderme**

Sık karşılaşılan bazı Azure dağıtım hataları hakkında bilgi edinmek ve bunları çözmek için bilgi almak için aşağıdaki makalelere bakın. Dağıtım hatanız için hata kodunu bulamıyorsanız bkz. Hata [kodunu bulma.](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code)

- [Dağıtım hatalarını giderme](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [Azure kaynaklarını yeni kaynak grubuna veya aboneliğe taşıma sorunlarını giderme](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

Unutmayın; Azure aboneliğinizi yükseltmek (örneğin, satın alınarak ücretsiz ödemeden geçiş yapmak gibi) için aboneliğinizi dönüştürmeniz gerekir.

- Ücretsiz deneme sürümü yükseltmek için bkz. Ücretsiz Denemenizi veya Microsoft Imagine Azure aboneliğinizi [Pay-As-You-Go aboneliğine yükseltme](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).
- Satın alınarak ödeyilen ödeme hesabını değiştirmek için bkz. Azure'a Göre Öde aboneliğinizi [farklı bir teklifle değiştirme.](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer)

**Azure aboneliğini kendi kiracınıza eklemek veya Azure Active Directory için:**

1. Oturum açın ve Azure portalında Abonelikler [sayfasından kullanmak istediğiniz aboneliği seçin.](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade)
2. Dizini **değiştir'i seçin.**
3. Görünen uyarıları gözden geçirerek Değiştir'i **seçin.**
4. Dizin abonelik için değiştirilir ve bir başarı iletisi alırsınız.
5. Yeni *dizininize* gitmek için Dizin anahtarınızı kullanın. Her şeyin düzgün bir şekilde olması 10 dakika kadar sürebilir.

**Önerilen Belgeler**

- [Azure aboneliğinin sahipliğini aktarma](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [Kaynakları yeni kaynak grubuna veya aboneliğe taşıma](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [Azure portalını kullanarak kaynakları yönetme](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
