---
title: Dynamics 365 Formlar İş Kuralları - İş Kuralı Bir Form için Ateş Değil
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: cbdedd2c5fcf5517243e60e36d86479d6c3f7814
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/18/2019
ms.locfileid: "36529039"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>Alan programlı olarak değiştirilirse OnChange olayı oluşmaz

Alan *öznitelik* kullanılarak programlı olarak değiştirilirse *OnChange* olayı oluşmaz. [setValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) yöntemi. *OnChange* olayının olay işleyicilerinin değeri ayarladıktan sonra çalışmasını istiyorsanız *formContext.data.entity özniteliğini* kullanmanız gerekir. [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) yöntemi kodunuzda.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
