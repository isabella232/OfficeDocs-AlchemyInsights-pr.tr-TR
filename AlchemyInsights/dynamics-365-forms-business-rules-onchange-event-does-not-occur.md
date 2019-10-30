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
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a><span data-ttu-id="14b66-102">Alan programlı olarak değiştirilirse OnChange olayı oluşmaz</span><span class="sxs-lookup"><span data-stu-id="14b66-102">OnChange event does not occur if the field is changed programmatically</span></span>

<span data-ttu-id="14b66-103">Alan *öznitelik* kullanılarak programlı olarak değiştirilirse *OnChange* olayı oluşmaz. [setValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) yöntemi.</span><span class="sxs-lookup"><span data-stu-id="14b66-103">The *OnChange* event does not occur if the field is changed programmatically using the *attribute.*[setValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) method.</span></span> <span data-ttu-id="14b66-104">*OnChange* olayının olay işleyicilerinin değeri ayarladıktan sonra çalışmasını istiyorsanız, kodunuzda *formContext.data.entity özniteliği* [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) yöntemini kullanmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="14b66-104">If you want event handlers for the *OnChange* event to run after you set the value you must use the *formContext.data.entity attribute* [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) method in your code.</span></span>

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
