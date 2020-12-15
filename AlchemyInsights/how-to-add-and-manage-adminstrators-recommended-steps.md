---
title: Yönetim önerileri nasıl eklenir ve yönetilir-önerilen adımlar
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/07/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004114"
- "7194"
ms.openlocfilehash: 142bf1474ac0e0eac5cecb9dddd35e28b6b6631e
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/08/2020
ms.locfileid: "49678868"
---
# <a name="how-to-add-and-manage-adminstrators---recommended-steps"></a>Yönetim önerileri nasıl eklenir ve yönetilir-önerilen adımlar

**Abonelik yöneticisini veya ortak yöneticiyi düzenleme**

- Hesap Yöneticisi her iki rolü de düzenleyebilir, abonelik Yöneticisi yalnızca [Azure portalında](https://ms.portal.azure.com/#home)ortak yöneticileri değiştirebilirler.
- [Azure aboneliği yöneticilerini ekleme veya değiştirme](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

**Abonelik Yöneticisi 'ni veya Iç (GERÇEKLEŞTIRILECEKTIR) abonelikleri için Co-Administrator güncelleştirme**

Hizmet Yöneticisi veya ortak yönetici, aşağıdaki adımları kullanarak bu eyleme Self-sunabilir:

1. [Azure portalında](https://ms.portal.azure.com/#home) oturum açın ve sol dikey, **maliyet yönetimi + faturalandırma** 'ı tıklatın.
2. Aboneliğinizle birlikte satır öğesine tıklayın. Bu, aboneliğinizin genel görünümünü açar.
3. **Abonelik** dikey penceresinde **Özellikler**'e tıklayın. 
4. **Hizmet Yöneticisi** düğmesine tıklayın.
5. Hizmet Yöneticisi olarak ayarlamak istediğiniz kullanıcının e-postasını girin ve **Tamam 'a** tıklayın.

**Yönetici ekleme/değiştirme/kaldırma**

1. [Azure portalında](https://ms.portal.azure.com/#home) hizmet yöneticisi olarak oturum açın.
2. [Abonelikleri](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) açın ve bir abonelik seçin. (Birlikte Yönetim Yardımcıları yalnızca abonelik kapsamında atanabilir.)
3. **Access Control (IAM)**  >  **Klasik yöneticileri** ekleme ortak  >    >  **yönetici** Ekle bölmesini açmak için yardımcı yönetici Ekle  'yi (ortak yönetici Ekle seçeneği devre dışıysa) açın.
4. Eklemek istediğiniz kullanıcıyı seçin ve **Ekle**'ye tıklayın.

**Daha fazla bilgi edinin:**
- [Yardımcı yönetici ekleme](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Yardımcı yöneticiyi kaldırma](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Hizmet yöneticisini değiştirme](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Hesap yöneticisini görüntüleme](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [RBAC ve Azure portalını kullanarak erişimi yönetme](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

**Azure Active Directory (AD) kullanarak kullanıcıları ekleme/silme**

Azure Active Directory (Azure AD) kuruluşunuzdan yeni kullanıcılar ekleyebilir veya varolan kullanıcıları silebilirsiniz:

1. Yeni bir kullanıcı eklemek için, kuruluş için Kullanıcı Yöneticisi olarak [Azure portalında](https://ms.portal.azure.com/#home) oturum açın.
2. **Azure Active Directory**'yi seçin, **Kullanıcılar** 'ı seçin ve ardından **Yeni Kullanıcı**'ya tıklayın.
3. **Kullanıcı** sayfasında, gerekli bilgileri doldurun. **Oluştur**'a tıklayın. Kullanıcı oluşturulur ve Azure AD kiracınıza eklenir.

**Daha fazla bilgi**:

- [Yeni Kullanıcı ekleme](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Kullanıcı silme](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Azure Active Directory kullanarak kullanıcının profil bilgilerini ekleme veya güncelleştirme](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

**Önerilen belgeler**

- [Rol tabanlı erişim denetimi (RBAC) nedir?](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [Azure 'da farklı rolleri anlama](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [Azure Active Directory 'de yönetici rolü izinleri](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [Öğretici: RBAC ve Azure portalını kullanarak bir kullanıcıya erişim Izni verme](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [Azure 'da RBAC sorunlarını giderme](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [Azure Yönetim gruplarıyla kaynaklarınızı düzenleme](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [Azure faturasının kopyasını e-posta yoluyla isteme](https://azure.microsoft.com/en-us/blog/azure-email-invoices/)
- [Azure 'dan kredi veya banka kartı ekleme, güncelleştirme veya kaldırma](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [Aboneliği yönetme (yeniden etkinleştirme/Iptal etme/değiştirme)](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



