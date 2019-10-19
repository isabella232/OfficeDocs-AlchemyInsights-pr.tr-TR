---
title: Hata ÖzniteliğiValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 5ac56fa78c66cf3b246bc0cc01f040e27310d629
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/18/2019
ms.locfileid: "36527079"
---
# <a name="error-attributevaluemustbeunique"></a>Hata: ÖznitelikValueMustBeUnique

AttributeValueMustBeUnique hatasının en yaygın nedeni, farklı SourceAnchor (immutableId) ile iki nesne proxyadresleri ve / veya UserPrincipalName öznitelikleri için aynı değere sahip olmasıdır. AttributeValueMustBeUnique hata düzeltmek için:
  
1. Hataya neden olan yinelenen proxyAdresleri, userPrincipalName veya diğer öznitelik değerini tanımlayın. Ayrıca, çatışmada hangi iki (veya daha fazla) nesnenin yer aldığını belirleyin. Azure AD Connect Health tarafından eşitleme için oluşturulan rapor, iki nesneyi belirlemenize yardımcı olabilir.
    
2. Yinelenen değere sahip olmaya devam etmesi gereken nesnenin hangisi olmaması gerektiğini belirleyin.
    
3. Yinelenen değeri bu değere sahip olmaması gereken nesneden kaldırın. Nesnenin kaynağının bulunduğu dizinde değişiklik yapmanız gerektiğini unutmayın. Bazı durumlarda, çakışan nesnelerden birini silmeniz gerekebilir.
    
4. Şirket içi AD'de değişiklik yaptıysanız, Azure AD Connect'in hatanın düzeltilmesi için değişikliği eşitlemasına izin verin.
    

