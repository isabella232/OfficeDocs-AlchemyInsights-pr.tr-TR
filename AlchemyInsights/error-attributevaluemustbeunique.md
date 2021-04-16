---
title: Error AttributeValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 35eb88624a5535e136ac1d01faf8e905bf00eb45
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813780"
---
# <a name="error-attributevaluemustbeunique"></a>Hata: AttributeValueMustBeUnique

AttributeValueMustBeUnique hatasının en yaygın nedeni, ProxyAddresses ve/veya UserPrincipalName özniteliklerinde farklı SourceAnchor (immutableId) olan iki nesnedir. AttributeValueMustBeUnique hatasını düzeltmek için:
  
1. Yinelenen proxyAddresses, userPrincipalName veya hataya neden olan diğer öznitelik değerini seçin. Ayrıca, çakışmaya hangi iki (veya daha fazla) nesne dahil olduğunu da belirleme. Eşitleme için Azure AD Connect Health tarafından oluşturulan rapor, iki nesneleri tanımlamanıza yardımcı olabilir.
    
2. Hangi nesnenin yinelanan değere sahip olmaya devam edeceğini ve hangi nesnenin sahip olması gerektiğini belirleme.
    
3. Yinelenen değeri, bu değere sahip OLASILIK olmaz olan nesneden kaldırın. Nesnenin kaynak bulunduğu dizinde değişiklik yapmaları gerektiğini unutmayın. Bazı durumlarda, çakışan nesnelerden birini silmeniz gerekiyor olabilir.
    
4. Değişikliği şirket içi AD'de yaptıysanız, hatanın düzeltilemeyecek şekilde Azure AD Connect tarafından eşitlensin.
    

