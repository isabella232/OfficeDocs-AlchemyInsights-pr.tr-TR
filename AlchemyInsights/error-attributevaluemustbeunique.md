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
ms.custom: Adm_O365
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 7b98b68fabff6c048f1bab6cf506355114d18658
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29916544"
---
# <a name="error-attributevaluemustbeunique"></a>Hata: AttributeValueMustBeUnique

AttributeValueMustBeUnique hatanın en yaygın nedeni, farklı SourceAnchor (immutableId) ile iki nesne ProxyAddresses ve/veya UserPrincipalName öznitelikleri için aynı değere sahip olabilir. AttributeValueMustBeUnique hatayı düzeltmek için:
  
1. Yinelenen proxyAddresses, userPrincipalName veya hataya neden olan diğer öznitelik değeri tanımlar. Ayrıca hangi iki (veya daha fazla) nesne çakışmasına katılan tanımlayın. Azure AD bağlantı durumu eşitleme için tarafından oluşturulan rapor iki nesneleri belirlemenize yardımcı olabilir.
    
2. Hangi nesnenin çoğaltılmış değerine sahip devam etmesi gerektiğini ve hangi nesne gerektiği tanımlayın.
    
3. Yinelenen değer bu değere sahip olmaması nesneden kaldırır. Burada gelen nesne kaynaklanacağı dizininde değişikliği yapmak zorunda unutmayın. Bazı durumlarda, çakışan nesnelerden birini silmeniz gerekebilir.
    
4. Üzerinde şirket AD değişikliği yaptıysanız, eşitleme ayarlarını değiştir hata sabit için Azure AD bağlantı sağlar.
    

