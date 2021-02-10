---
title: Güvenlik gruplarında sorun
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8252"
- "9004397"
ms.openlocfilehash: 1198b79c3301bd2752a7385a6ba6746c8f0c2b5b
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177636"
---
# <a name="issue-with-security-groups"></a>Güvenlik gruplarında sorun

**Ağ Hatası AADDS104 alıyorsanız**

Azure Active Directory Etki Alanı Hizmetleri'nin (AD DS) ağ hatalarının en yaygın nedeni geçersiz ağ güvenlik grubu kurallarıdır. Sanal ağın ağ güvenlik grubunun belirli bağlantı noktalarına ve protokollere erişime izin vermesi gerekir. Bu bağlantı noktaları engellenmişse, Azure platformu yönetilen etki alanını izleyamaz veya güncelleştiramaz. Azure AD ile Azure AD DS arasındaki eşitleme de etkiyi etkiler. Hizmette kesinti olmasını önlemek için varsayılan bağlantı noktalarını açık tutabilirsiniz.

Ağ güvenliği grubu yapılandırma sorunlarının yaygın uyarılarını anlamak ve çözmek için bkz. Güvenlik Grupları [Ekleme ve Doğrulama.](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules)
