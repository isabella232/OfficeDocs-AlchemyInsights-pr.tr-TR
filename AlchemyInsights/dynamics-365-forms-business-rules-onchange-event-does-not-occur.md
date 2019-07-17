---
title: Dynamics 365 iş kuralları - tetikleme değil bir Form için iş kuralı oluşturur.
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: 4ade8d2f68b465298e2d6efff3eef4f04f25c3bf
ms.sourcegitcommit: a413a0e27ef4ab8c484fa9fccff8bbef381c8b96
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35749043"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>Alanı program aracılığıyla değiştirildiğinde OnChange olayı gerçekleştirilmiyor

Alanı kullanarak programlı olarak değiştirildiğinde *OnChange* olayı oluşmaz *özniteliği.* [DeğerBelirle](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) yöntemi. Kullanmaları gereken değeri ayarlandıktan sonra çalıştırılacak *OnChange* olayı için olay işleyicileri isteyip istemediğinizi *özniteliği formContext.data.entity.* [fireOnchange](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) yöntemi, kodunuzda.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
