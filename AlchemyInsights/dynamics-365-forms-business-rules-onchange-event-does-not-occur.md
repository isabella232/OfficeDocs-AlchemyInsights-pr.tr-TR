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
ms.openlocfilehash: 3cdd2175083e864b3bffc57a70bb6c6220843fad
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/29/2019
ms.locfileid: "37769359"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>Alan programlı olarak değiştirilirse OnChange olayı oluşmaz

Alan *öznitelik* kullanılarak programlı olarak değiştirilirse *OnChange* olayı oluşmaz. [setValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) yöntemi. *OnChange* olayının olay işleyicilerinin değeri ayarladıktan sonra çalışmasını istiyorsanız, kodunuzda *formContext.data.entity özniteliği* [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) yöntemini kullanmanız gerekir.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
