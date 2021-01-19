---
title: Etki alanı denetleyicisi
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7909"
- "9003233"
ms.openlocfilehash: d4cbe80c3e8f0ce32fcbe89e852f24efd6f50575
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901317"
---
# <a name="domain-controller"></a>Etki alanı denetleyicisi

**AAD etkinleştirilemiyor-DS veya dağıtım başarısız oluyor**

Azure AD etki alanı hizmeti 'nin (AAD-DS) etkinleştirilmemiş veya dağıtılmadığı sorunu çözmek için aşağıdaki adımları uygulayın:

1. Var olan bir sanal ağı kullanıyorsanız, portalda AAD-DS 'de eşitleme yapmak için gereken bağlantı noktalarını engelleyen kurallar için NSG 'inizi denetleyin https://aka.ms/aadds-networking .
2. Bu sorun giderme kılavuzunda, hata iletinizin yanıtlanmadığını denetleyin  https://aka.ms/aadds-troubleshoot-enable .
3. Azure AD etki alanı Hizmetleri 'ni yeni bir sanal ağda dağıtmayı deneyin.
4. [Azure AD etki alanı Hizmetleri oluşturmaya yönelik öğretici](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance)'de sağlanan AAD-DS 'yi dağıtmaya yönelik Başlarken Kılavuzunu izleyin.
5. Azure AD etki alanı Hizmetleri 'ni dağıtma konusunda sorun yaşıyorsanız, bir kez daha çalışmanızı öğrenmenize yardımcı olacak genel hataları çözmek için [Azure AD etki alanı Hizmetleri sorunlarını giderme](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) konusuna bakın. 

**AAD devre dışı bırakılamıyor-DS**

AAD-DS duraklatılamıyor. Yönetilen etki alanınızı kullanmayı durdurmak istiyorsanız, silinmesi gerekir.

Sorunlarla karşılaşırsanız, yaygın hata iletilerini ve daha fazla işlem yapmanıza yardımcı olacak ilgili sorun giderme adımları için [, bkz.](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot)
