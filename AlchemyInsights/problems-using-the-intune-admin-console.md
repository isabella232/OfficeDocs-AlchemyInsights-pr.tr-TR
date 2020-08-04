---
title: Intune yönetici konsolu kullanarak sorunlar
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 7a36d502a92d360b06336ccfa6183f666f0260ab
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555881"
---
# <a name="problems-using-the-intune-admin-console"></a>Intune yönetici konsolu kullanarak sorunlar

**Intune yönetici portalında gezinirken "Erişim reddedildi".**

- Bir Intune özel rolün üyesiyseniz, hesabınıza bir Intune veya Enterprise Mobility Suite (EMS) lisansının atandığından emin olun.
- Aygıtları yönetmek için Configuration Manager kullanıyorsanız, Configuration Manager MDM için Intune kullanıcı koleksiyonunun bir parçası olmadığınızı doğrulayın.
- Intune rolleri bıçak çağınızda uygun rol tabanlı yönetim denetimi (RBAC) izinlerinin size atandığını doğrulayın.
- Kullanılan grubun dağıtım listesi olmadığını doğrulayın. Azure portalındaki Intune yalnızca Azure Etkin Dizin güvenlik gruplarına ait kullanıcı hesaplarını destekler. Gruplarınızı Azure portalı > **Intune**  >  **Grupları'nda**veya Azure portalında Azure Active Directory > gözden **geçirin.**

**Kullanıcı atanan Intune rolü için çok fazla izine sahiptir**

Kullanıcıya **Verilen**  >  izinleri gözden geçirmek için**Intune Intune**  >  **rolleriBenim izinleri**  >  **Dışa aktarın** gidin tavsiye edin.

**Bir role bir kapsam grubu ekledim, ancak bu roldeki kullanıcılar hala diğer kullanıcıları veya aygıtları görür.**

Kapsam grupları kullanıcıları veya aygıtları filtrelemez. Kapsam grupları:

- Kullanıcıların ilkeleri veya uygulamaları kimlere atayabileceğini sınırlayın.
- Aygıtlarda yalnızca belirli kullanıcıların uzak görevleri çalıştırabilmelerine izin verin.

Kapsam grupları hakkında daha fazla bilgi için [Microsoft Intune ile Rol tabanlı erişim denetimi (RBAC)](https://docs.microsoft.com/intune/role-based-access-control)'a bakın.

**Ben bir Intune rolü ne bir kullanıcı ekledi ama yine de Intune yönetici konsolu tam erişime sahip.**

Azure portalındaki Intune > **Kullanıcılar'a** gidin ve kullanıcının Azure portalında aşağıdaki rollerden hiçbirine atanmadığını doğrulayın:

- Genel yönetici
- Intune servis yöneticisi
- SharePoint yöneticisi

Daha fazla bilgi için [Microsoft Intune ile Rol tabanlı erişim denetimine (RBAC)](https://docs.microsoft.com/intune/role-based-access-control)bakın.

**Erişim Sorunları**

Daha fazla bilgi için [bkz.](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune)