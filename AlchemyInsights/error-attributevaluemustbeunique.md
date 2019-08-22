---
title: Hata AttributeValueMustBeUnique
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
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36527079"
---
# <a name="error-attributevaluemustbeunique"></a>Hata: AttributeValueMustBeUnique

AttributeValueMustBeUnique hatanın en yaygın nedeni, farklı SourceAnchor (immutableId) ile iki nesne ProxyAddresses ve/veya UserPrincipalName öznitelikleri için aynı değere sahip olabilir. AttributeValueMustBeUnique hatayı düzeltmek için:
  
1. Yinelenen proxyAddresses, userPrincipalName veya hataya neden olan diğer öznitelik değeri tanımlar. Ayrıca hangi iki (veya daha fazla) nesne çakışmasına katılan tanımlayın. Azure AD bağlantı durumu eşitleme için tarafından oluşturulan rapor iki nesneleri belirlemenize yardımcı olabilir.
    
2. Hangi nesnenin çoğaltılmış değerine sahip devam etmesi gerektiğini ve hangi nesne gerektiği tanımlayın.
    
3. Yinelenen değer bu değere sahip olmaması nesneden kaldırır. Burada gelen nesne kaynaklanacağı dizininde değişikliği yapmak zorunda unutmayın. Bazı durumlarda, çakışan nesnelerden birini silmeniz gerekebilir.
    
4. Üzerinde şirket AD değişikliği yaptıysanız, eşitleme ayarlarını değiştir hata sabit için Azure AD bağlantı sağlar.
    

