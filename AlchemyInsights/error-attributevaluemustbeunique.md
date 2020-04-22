---
title: Hata ÖzniteliğiValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: fa1fdb35f1af250bc98aa61c0e5111f1f1b8aac4
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703194"
---
# <a name="error-attributevaluemustbeunique"></a>Hata: ÖznitelikValueMustBeUnique

AttributeValueMustBeUnique hatasının en yaygın nedeni, farklı SourceAnchor (immutableId) ile iki nesne proxyadresleri ve / veya UserPrincipalName öznitelikleri için aynı değere sahip olmasıdır. AttributeValueMustBeUnique hata düzeltmek için:
  
1. Hataya neden olan yinelenen proxyAdresleri, userPrincipalName veya diğer öznitelik değerini tanımlayın. Ayrıca, çatışmada hangi iki (veya daha fazla) nesnenin yer aldığını belirleyin. Azure AD Connect Health tarafından eşitleme için oluşturulan rapor, iki nesneyi belirlemenize yardımcı olabilir.
    
2. Yinelenen değere sahip olmaya devam etmesi gereken nesnenin hangisi olmaması gerektiğini belirleyin.
    
3. Yinelenen değeri bu değere sahip olmaması gereken nesneden kaldırın. Nesnenin kaynağının bulunduğu dizinde değişiklik yapmanız gerektiğini unutmayın. Bazı durumlarda, çakışan nesnelerden birini silmeniz gerekebilir.
    
4. Şirket içi AD'de değişiklik yaptıysanız, Azure AD Connect'in hatanın düzeltilmesi için değişikliği eşitlemasına izin verin.
    

