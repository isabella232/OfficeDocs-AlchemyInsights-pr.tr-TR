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
ms.openlocfilehash: f3564063a3adf291ec4909ffeb2f6de0e478da96
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430358"
---
# <a name="problem-with-single-user"></a>Tek kullanıcıyla ilgili sorun

- Hizmet, kullanıcıyı henüz değerlendirme fırsatı olmadı diye kullanıcıya sağlanmadı. Hazırlamanın ne kadar sürece sürecesi ile ilgili kılavuzu ve sağlama yapılandırma sayfasındaki ilerleme çubuğunu gözden geçirebilirsiniz. Ek ayrıntılar bölümünde belirtilen sabit durum kullanıcının oluşturulma/güncelleştirilmeden/silinmeden önce geliyorsa, kullanıcıyı henüz değerlendirmedik demektir. Bu senaryoda, yapacak en iyi şey sağlama hizmetinin bitip bitimini beklemektir.

  - Hizmetimizin yalnızca kaynak sistem (Bulut İk) kullanıcıya yapılan değişikliklerden haberdar olduğunu unutmayın. Azure AD'nin değişikliği algılaması ve Active Directory'ye akışı için kaynak sistemde geçerli bir değişiklik olması gerekir.
- Sağlama hizmeti kullanıcıyı değerlendirdi ve sağlanmaz olarak belirledi:
  - Özniteliği temel alan bircoping filtresi ayardıysanız, kullanıcının belirttiğiniz ölçütlere uygun olduğundan emin olur.
  - Kullanıcılar zaten hedef sistemde bulunuyorsa ve kullanıcının durumu kaynak ve hedef eşleşmede bulunuyorsa, başka bir işlemde yer almayacağız.
- Sağlama hizmeti, kullanıcıya sağlamayı denendi ve başarısız oldu. Bu senaryolar için, sağlama günlüklerinin sorun giderme ve öneriler sekmesini gözden geçirebilirsiniz:
  - Şirket içi Active Directory'de veya Azure AD'de kullanıcıda gerekli bir öznitelik eksik olabilir. Örneğin, userPrincipalName veya sAMAccountName oluşturma kuralları doğru değeri oluşturmaz.
  - Eşleşen öznitelik (genellikle employeeId) şirket içi Active Directory'de veya Azure AD'de benzersiz bir kullanıcıyla çözümlenemmektedir. Örneğin, AD'de aynı çalışankimsi olan iki kullanıcı vardır ve hizmet aynı kaynak girdi için yinelenen hedef girdileri belirten bir hata kodu döndürür.

Tek bir kullanıcının ve grupların günlüklerini gözden geçirmek için bkz. Belirli bir kullanıcıyla ilgili [bir sorunun sağlama günlüklerini gözden geçirme.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs)
