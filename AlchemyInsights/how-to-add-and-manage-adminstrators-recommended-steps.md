---
title: Yöneticileri ekleme ve yönetme - önerilen adımlar
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
ms.openlocfilehash: 48a06fde215e007b6b81b32ab751ca8e4bba522d
ms.sourcegitcommit: 46e24d65cffd37b6988447c6738b3315303bbe13
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58339052"
---
# <a name="how-to-add-and-manage-administrators---recommended-steps"></a>Yöneticileri ekleme ve yönetme - önerilen adımlar

Sorun açıklamanıza bağlı olarak sizin için bir çözüm bulduk. Çoğu müşteri belgelerimizi takip ettikten sonra sorununuzu kendi kendine çöze kavuştur bulundu.

**Abonelik Yöneticisi'yi veya Ortak Yönetici'yi düzenleme**

- Abonelik Yöneticisi her iki rolü de düzenleyebilir, ancak Abonelik Yöneticisi yalnızca [Azure portalında](https://ms.portal.azure.com/#home)Ortak yöneticileri değiştirebilir.
- [Azure abonelik yöneticilerini ekleme veya değiştirme](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

**İç (AIRS) Abonelikler Co-Administrator Yöneticisini veya Aboneliği Güncelleştirme**

Hizmet Yöneticisi veya Ortak yönetici, aşağıdaki adımları kullanarak bu eyleme kendi kendine hizmet etmek için kullanabilir:

1. [Azure portalda](https://ms.portal.azure.com/#home) oturum açın ve sol blade'de **Maliyet Yönetimi + Faturalama'ya** tıklayın.
2. Aboneliğinizin sağ olduğu satıra tıklayın. Bu işlem, aboneliğinize genel bakış görünümünü açar.
3. Abonelik **blade'inde** Özellikler'e **tıklayın.** 
4. Hizmet Yöneticisi **düğmesine** tıklayın.
5. Hizmet Yöneticisi olarak ayarlamak istediğiniz kullanıcının e-posta adresini girin ve Tamam'a **tıklayın.**

**Ortak yönetici ekleme/değiştirme/kaldırma**

1. Hizmet Yöneticisi olarak [Azure portalında](https://ms.portal.azure.com/#home) oturum açın.
2. [Abonelikler'i](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) açın ve bir abonelik seçin. (Yardımcı yöneticiler yalnızca abonelik kapsamında atanabilir.)
3. Erişim denetimi **(IAM)** Klasik yöneticiler Eş yönetici ekle bölmesini açmak için Eş yönetici ekle'ye gidin (Ortak yönetici ekle seçeneği devre dışı bırakılmışsa, izinlere sahip  >    >    >   olmadığınız gösterilir). 
4. Eklemek istediğiniz kullanıcıyı seçin ve Ekle'ye **tıklayın.**

**Daha fazla bilgi edinin:**
- [Ortak Yönetici ekleme](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Ortak yöneticiyi kaldırma](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Hizmet Yöneticisi'ni değiştirme](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Hesap Yöneticisi'ne görüntüleme](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [RBAC ve Azure portalını kullanarak erişimi yönetme](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

**E-posta (AD) Azure Active Directory kullanıcı ekleme/silme**

Yeni kullanıcılar ekleyebilir veya var olan kullanıcıları Azure Active Directory (Azure AD) kuruluşundan silebilirsiniz:

1. Yeni kullanıcı eklemek için, Azure [portalında](https://ms.portal.azure.com/#home) kuruluş için Kullanıcı yöneticisi olarak oturum açın.
2. **Kullanıcılar Azure Active Directory ı** seçin ve **Ardından Yeni** kullanıcı **'ya tıklayın.**
3. Kullanıcı **sayfasında** gerekli bilgileri doldurun. **Oluştur'a tıklayın.** Kullanıcı oluşturulur ve Azure AD kiracınıza eklenir.

**Daha fazla bilgi:**

- [Yeni kullanıcı ekleme](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Kullanıcı silme](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Profili kullanarak kullanıcının profil bilgilerini ekleme veya Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

**Önerilen belgeler**

- [Rol tabanlı erişim denetimi (RBAC) nedir?](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [Azure'daki farklı rolleri anlama](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [Web'de yönetici rolü Azure Active Directory](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [Öğretici: RBAC ve Azure portalını kullanan bir kullanıcı için erişim izni ver](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [Azure'da RBAC sorunlarını giderme](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [Azure yönetim gruplarıyla kaynaklarınızı düzenleme](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [Azure faturalarının kopyasını e-posta yoluyla talep edin](https://azure.microsoft.com/blog/azure-email-invoices/)
- [Azure'da kredi kartı veya banka kartı ekleme, güncelleştirme veya kaldırma](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [Aboneliği yönetme (Yeniden Etkinleştir/İptal/Değiştir)](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



