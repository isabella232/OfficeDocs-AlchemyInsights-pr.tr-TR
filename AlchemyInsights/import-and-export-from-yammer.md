---
title: Yammer'dan içeri ve dışarı aktarma
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9735"
- "9003224"
ms.openlocfilehash: dcdf569f96e51a62899761589ef6f9f317517c3a
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037255"
---
# <a name="import-and-export-from-yammer"></a>Yammer'dan içeri ve dışarı aktarma

**İçeri aktar**

Kullanıcı içeri aktarma seçenekleri, Yammer ağınızı [Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode)için Yerel Modda olup olmadığınıza bağlı olarak değişir.

- **Yerel Olmayan Mod:** Kullanıcılar, Grup ayarları içinde Adres Defteri'den [](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) [Ekle](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) 'yi kullanarak gruplara (100 kullanıcıyla sınırla) veya Ağ Yöneticisi içindeki Toplu Güncelleştirme kullanılarak ağa aktarabilirsiniz.
- **Yerel Mod:** Grup üyeliği ve ağ üyeliği işlemleri [Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users)yönetim portalında, [Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)portalında veya başka bir Azure AD seçeneği kullanılarak yapılmalıdır. Yerel Mod'daki ağların artık Toplu Güncelleştirme ve diğer eski özelliklere erişimi yoktur.

> [!IMPORTANT]
> Yammer, Veri Dışarı Aktarma özelliği başka bir ağda kullanılmış olsa bile Ağ Yöneticisi'nin içinde içerik içeri aktarmayı hiçbir zaman desteklemez. İçerik iş ortağı çözümleri veya Yammer REST API'leri tarafından yeniden posta olabilir.

**Dışarı Aktar**

[Ağ Verilerini Ağ Yöneticisi'nin içinde](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) dışarı aktarma, iletiler ve dosyalar dahil olmak üzere Yammer ağlarından içerik dışarı aktarmaya izin verir. Ekler aşırı büyük olabilir ve dışarı aktarma işleminin tamamlanması önemli ölçüde zaman alır. Etkin ağların, Veri Dışarı Aktarma [API'si](https://developer.yammer.com/docs/data-export-api) kullanılarak gün veya haftaya göre parçalar halinde dışarı aktarmasını öneririz. Microsoft Desteği bu amaç için özel betikler sağlamaz.

Tek bir [kullanıcının içeriğini dışarı aktaran](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) ayrı bir GDPR dışarı aktarma vardır.