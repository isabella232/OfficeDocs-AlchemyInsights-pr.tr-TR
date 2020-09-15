---
title: Hata AttributeValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 4627a7ae34b0dd9f16538ef75ac8792672dcc056
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709171"
---
# <a name="error-attributevaluemustbeunique"></a>Hata: AttributeValueMustBeUnique

AttributeValueMustBeUnique hatasının en yaygın nedeni, farklı Sourcetutturucu olan iki nesnedir (Sanmutableıd) ProxyAddresses ve/veya UserPrincipalName öznitelikleri için aynı değere sahiptir. AttributeValueMustBeUnique hatasını düzeltmek için:
  
1. Hataya neden olan yinelenmiş proxyAddresses, userPrincipalName veya diğer öznitelik değerini tanımlayın. Ayrıca, çakışmaya hangi iki (veya daha fazla) nesne dahil olduğunu belirleyin. Eşitlemede Azure AD Connect Health tarafından oluşturulan rapor iki nesneyi tanımlamanıza yardımcı olabilir.
    
2. Hangi nesnenin yinelenen değeri ve hangi nesneyle olmaması gerektiğini belirleyin.
    
3. Bu değeri içermeyen nesneden yinelenen değeri kaldırın. Nesnenin kaynağı olduğu dizindeki değişikliği yapmanız gerektiğini unutmayın. Bazı durumlarda, çakışmada nesnelerden birini silmeniz gerekebilir.
    
4. Şirket içi AD 'de değişiklik yaptıysanız, Azure AD Connect eşitlemesini, hatanın düzeltilmesi için hatayı değiştirmeye izin verin.
    

