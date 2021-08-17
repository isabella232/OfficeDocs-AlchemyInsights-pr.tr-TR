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
ms.openlocfilehash: 45cf530c3258fa3c7008c3e8251fdb7b74be6911d0487f58c5ce2530e25ca282
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54110700"
---
# <a name="replica-set"></a>Çoğaltma kümesi

AADDS, yönetilen etki alanı olarak da çağrılır. Aslında, arka uç tarafından çalıştırarak bakımını yapılan iki etki alanı denetleyicisi vardır. İki DC bir ana DC ve bir de çoğaltma DC'si içerir. AADDS'de (yönetilen etki alanı) yedeklemeler, Azure platformu tarafından yönetilen otomatik bir işlemdir. Yönetilen etki alanınız ile ilgili bir sorun varsa, Azure desteği yedekten geri yüklemede size yardımcı olabilir.

Her bir kopya kümesi için bir sanal ağ oluşturabilirsiniz. Her sanal ağ, yönetilen bir etki alanının çoğaltma kümesi barındıran diğer tüm sanal ağlara eş olmalıdır. Bu yapılandırma, dizin çoğaltmayı destekleyen bir ağ ağı topolojisi oluşturur. Her çoğaltma kümesi farklı bir sanal alt ağda olmalıdır ve sanal ağ birden çok çoğaltma kümelerini destekleyene.

Çoğaltma kümesi hakkında daha fazla ayrıntı için bkz. [Kavram Çoğaltma kümeleri](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets).
