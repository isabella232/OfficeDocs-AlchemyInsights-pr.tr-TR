---
title: Hata AttributeValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 7a97d1a5ff352b55833bd457e3220a56130d7e7e
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29499654"
---
# <a name="error-attributevaluemustbeunique"></a>Hata: AttributeValueMustBeUnique

AttributeValueMustBeUnique hatanın en yaygın nedeni, farklı SourceAnchor (immutableId) ile iki nesne ProxyAddresses ve/veya UserPrincipalName öznitelikleri için aynı değere sahip olabilir. AttributeValueMustBeUnique hatayı düzeltmek için:
  
1. Yinelenen proxyAddresses, userPrincipalName veya hataya neden olan diğer öznitelik değeri tanımlar. Ayrıca hangi iki (veya daha fazla) nesne çakışmasına katılan tanımlayın. Azure AD bağlantı durumu eşitleme için tarafından oluşturulan rapor iki nesneleri belirlemenize yardımcı olabilir.
    
2. Hangi nesnenin çoğaltılmış değerine sahip devam etmesi gerektiğini ve hangi nesne gerektiği tanımlayın.
    
3. Yinelenen değer bu değere sahip olmaması nesneden kaldırır. Burada gelen nesne kaynaklanacağı dizininde değişikliği yapmak zorunda unutmayın. Bazı durumlarda, çakışan nesnelerden birini silmeniz gerekebilir.
    
4. Üzerinde şirket AD değişikliği yaptıysanız, eşitleme ayarlarını değiştir hata sabit için Azure AD bağlantı sağlar.
    

