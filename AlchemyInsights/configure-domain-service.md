---
title: Etki alanı hizmetini yapılandırma
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7931"
- "9004400"
ms.openlocfilehash: 51e0bd78240627876721cbce654188afac1ee365
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885684"
---
# <a name="unable-to-enable-aad-ds-or-deployment-is-failing"></a>AAD etkinleştirilemiyor-DS veya dağıtım başarısız oluyor

Azure AD etki alanı hizmeti 'nin (AAD-DS) etkinleştirilmemiş veya dağıtılmadığı sorunu çözmek için aşağıdaki adımları uygulayın:

1. Var olan bir sanal ağı kullanıyorsanız, portalda AAD-DS 'de eşitleme yapmak için gereken bağlantı noktalarını engelleyen kurallar için NSG 'inizi denetleyin https://aka.ms/aadds-networking .
2. Bu sorun giderme kılavuzunda, hata iletinizin yanıtlanmadığını denetleyin  https://aka.ms/aadds-troubleshoot-enable .
3. Azure AD etki alanı Hizmetleri 'ni yeni bir sanal ağda dağıtmayı deneyin.
4. AAD 'yi dağıtma-DS: [AAD etki alanı Hizmetleri oluşturma ve yapılandırma](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance)
5. Azure AD etki alanı Hizmetleri 'ni dağıtma konusunda sorun yaşıyorsanız, bir kez daha çalışmanızı öğrenmenize yardımcı olacak genel hataları çözmek için [Azure AD etki alanı Hizmetleri sorunlarını giderme](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) konusuna bakın. 

**AAD devre dışı bırakılamıyor-DS**

AAD-DS duraklatılamıyor. Yönetilen etki alanınızı kullanmayı durdurmak istiyorsanız, silinmesi gerekir.
Yönetilen etki alanınızı silmek için, [AAD etki alanı hizmetini silme](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds)konusuna bakın.



