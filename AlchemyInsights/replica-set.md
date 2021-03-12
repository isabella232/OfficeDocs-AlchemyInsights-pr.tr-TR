---
title: Çoğaltma kümesi
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
- "9004400"
- "9004395"
- "8265"
- "9276"
ms.openlocfilehash: 3834696ff59b7e96e90a5b660a489003dfa9729c
ms.sourcegitcommit: 581c696ec108184adae9d4bc8f47cb9247131de8
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714587"
---
# <a name="replica-set"></a>Çoğaltma kümesi

AADDS, yönetilen etki alanı olarak da adlandırılan bir etki alanıdır. Aslında, arka uç tarafından çalıştır ve bakımını yapılan iki etki alanı denetleyicisidir. İki DC bir ana DC ve bir çoğaltma DC içerir. AADDS'de (yönetilen etki alanı) yedeklemeler, Azure platformu tarafından yönetilen otomatik bir işlemdir. Yönetilen etki alanınız ile ilgili bir sorun varsa, Azure desteği yedeklemeden geri yüklemede size yardımcı olabilir.

Sanal bir ağda her çoğaltma kümesi oluşturabilirsiniz. Her sanal ağ, yönetilen bir etki alanının çoğaltma kümesi barındıran diğer tüm sanal ağlara eş olmalıdır. Bu yapılandırma, dizin çoğaltmayı destekleyen bir ağ ağı topolojisi oluşturur. Her çoğaltma kümesi farklı bir sanal alt ağda yer alan sanal ağ, birden çok çoğaltma kümesini destekleyenin.

Çoğaltma kümesi hakkında daha fazla ayrıntı için, Kavramlar Çoğaltma [kümelerini gözden geçirin.](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets)
