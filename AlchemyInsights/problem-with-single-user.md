---
title: Tek kullanıcıyla ilgili sorun
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8469"
ms.openlocfilehash: 8d8821cda94b2af244fa317707421f9d197b6052fb316789cd286ea8b4adf19e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53960171"
---
# <a name="problem-with-single-user"></a>Tek kullanıcıyla ilgili sorun

- Hizmet, kullanıcıyı henüz değerlendirme fırsatı bu etmey olduğundan kullanıcıya sağlanmadı. Hazırlama yapılandırması sayfasında hem hazırlamanın ne kadar süreyle ilerle ilgili kılavuzu hem de ilerleme çubuğunu gözden geçirebilirsiniz. Ek ayrıntılar bölümünde belirtilen sabit durum kullanıcının oluşturulma/güncelleştirildikten/silindi tarihten önce geliyorsa, bu, kullanıcıyı henüz değerlendirmedik demektir. Bu senaryoda, en iyi şey sağlama hizmetinin bitip bitip bitene kadar beklemesini beklemektir.

  - Hizmetimizin yalnızca kaynak sistem (Bulut İk) kullanıcıya yapılan değişikliklerden haberdar olduğunu unutmayın. Azure AD'nin değişikliği algılaması ve Active Directory'ye akışı için kaynak sisteminde geçerli bir değişiklik olması gerekir.
- Sağlama hizmeti, kullanıcıyı değerlendirdi ve sağlanmaz olarak belirlendi:
  - Öznitelik tabanlı bir yer arama filtresi ayardıysanız, kullanıcının belirttiğiniz ölçütlere uyanlara uygun olduğundan emin olur.
  - Kullanıcılar zaten hedef sistemde bulunuyorsa ve kullanıcının durumu kaynak ve hedef eşleşmede bulunuyorsa, başka işlem uygulamayacağız.
- Sağlama hizmeti kullanıcıya sağlamayı çalıştı ve başarısız oldu. Bu senaryolar için, sağlama günlüklerinin sorun giderme ve öneriler sekmesini gözden geçirme:
  - Kullanıcıda gerekli bir öznitelik şirket içi Active Directory veya Azure AD'de eksik olabilir. Örneğin userPrincipalName veya sAMAccountName oluşturma kuralları doğru değeri oluşturmaz.
  - Eşleşen öznitelik (genellikle çalışanKimsi), şirket içi Active Directory veya Azure AD'daki benzersiz bir kullanıcıya çözümlenemediğini belirtir. Örneğin, AD'de aynı çalışankiki iki kullanıcı vardır ve hizmet, aynı kaynak girdi için yinelenen hedef girdileri belirten bir hata kodu döndürür.

Tek kullanıcı ve grupların günlüklerini gözden geçirmek için [bkz. Belirli bir kullanıcıyla](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs)ilgili soruna ilişkin sağlama günlüklerini gözden geçirme .
