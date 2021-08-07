---
title: 'RBAC rolleri '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "7265"
ms.openlocfilehash: 1faa9f69942d39b8d78c8f3e1316f93b52eeede6408dfabc89d0f7fe38b86fb3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923151"
---
# <a name="rbac-rules"></a>RBAC kuralları

İzin hatası alırsanız: 

- Nesne kimliği bulunan istemci, kapsam **(kod: AuthorizationFailed)** üzerinden eylem gerçekleştirmek için yetkilendirmeye sahip değildir: Kaynak oluşturmaya denemiş durumdayken, seçili kapsamda kaynak üzerinde yazma iznine sahip bir role atanmış bir kullanıcıyla oturum açanın. Örneğin, bir kaynak grubunda sanal makineleri yönetmek için, kaynak grubunda (veya üst kapsamda) [Sanal](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) Makine Katılımcısı rolünüz olması gerekir. Her bir yerleşik rolün izinlerinin listesi için bkz. [Azure kaynakları için yerleşik roller](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).
- Destek isteği oluşturma izniniz **yok:** Destek bileti oluşturmak veya güncelleştirmek için, şu anda Microsoft.Support/supportTickets/write iznine sahip, Destek İsteği Katılımcısı . [](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor)
- Artık rol ataması oluşturulamıyor **(kod: RoleAssignmentLimitExceeded)**: bir rol atamayı deneerek, bunun yerine gruplara roller ataarak rol atamalarının sayısını azaltmayı deneyin. Azure, abonelik başına **2000'e** kadar rol atamalarını destekler.

Azure RBAC rolleri hakkında daha fazla ayrıntı için bkz. [Azure RBAC rolleri.](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support)
