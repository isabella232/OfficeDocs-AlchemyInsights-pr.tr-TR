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
ms.openlocfilehash: 7c4c9d1a76f395dfb2f831d555199b76c354ca57
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583956"
---
# <a name="rbac-rules"></a>RBAC kuralları

İzin hatasını alırsanız: 

- **Nesne kimliğine sahip istemci kapsam üzerinde eylem gerçekleştirme yetkisine sahip değil (kod: Authorizationbaşarısız oldu)**: bir kaynak oluşturmaya çalıştığınızda, şu anda seçili kapsamda kaynağa yazma izni olan bir rol atanmış bir kullanıcıyla oturumunuz açık olup olmadığını denetleyin. Örneğin, kaynak grubundaki sanal makineleri yönetmek için kaynak grubunda (veya üst kapsamda) [sanal makine katılımcısı](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) rolüne sahip olmanız gerekir. Yerleşik rollerin izinlerinin listesi için, [Azure kaynakları Için yerleşik rollere](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support)bakın.
- **Destek isteği oluşturmak için izniniz** yok: bir destek bileti oluşturmaya veya güncelleştirmeye çalıştığınızda, şu anda Microsoft. support/supportticket/Write iznine sahip bir rol atanmış olan bir kullanıcı ile oturumunuz açık olup olmadığını denetleyin; Örneğin, bu [katılımcı desteği](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).
- **Daha fazla rol ataması oluşturulamaz (kod: roleatamasayısı)**: rol atamayı denediğinizde, bunun yerine gruplara roller atayarak rol atamalarının sayısını azaltmayı deneyin. Azure, abonelik başına en çok **2000** rol atamasını destekler.

Azure RBAC rolleriyle ilgili daha fazla bilgi için [Azure RBAC rollerine](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support)bakın.
