---
title: Kullanıcı hazırlama
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
- "9004348"
- "8428"
ms.openlocfilehash: bd415b2d44bccf0c2b3eccb4e38452498b748b3a
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482912"
---
# <a name="user-provisioning"></a>Kullanıcı hazırlama

- Kullanıcı [sağlamak ve adımlar hakkında](https://docs.microsoft.com/azure/active-directory/app-provisioning/provision-on-demand) ayrıntılı tanılama almak için isteğe bağlı sağlama özelliğini kullanın.
- Kullanıcıları ve grupları sağlarken karşılaştığınız sorunları gidermek için, Sorun giderme [kılavuzuna bakın. Kullanıcı sağlandı.](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-config-problem-no-users-provisioned)
- Kullanıcıların sağlanmaz olduğunu gözlemlersanız, Azure Active [Directory'de (AD)](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs) sağlama günlüklerine (önizleme) bakın. Belirli bir kullanıcıyla ilgili günlük girdilerini arama.
- Önceki sağlama döngüsünde kaçırilen tüm kullanıcıları yakalamak için sağlamayı düzenli aralıklarla yeniden başlatın.
- Hizmetimiz kullanıcıyı henüz değerlendirme fırsatı bulamamıştır, çünkü kullanıcı/grup sağlanmadı. Hazırlamanın ne kadar sürece sürecesi ile ilgili kılavuzu ve sağlama yapılandırma sayfasındaki ilerleme çubuğunu gözden geçirebilirsiniz. Ek ayrıntılar bölümünde belirtilen sabit durum kullanıcının oluşturulma/güncelleştirilmeden/silinmeden önce geliyorsa, kullanıcıyı henüz değerlendirmedik demektir. Bu senaryoda, yapacak en iyi şey sağlama hizmetinin bitip bitimini beklemektir. Sabit bir durum elde edildi ise, Azure Portal'da kullanıcı arabiriminden yeniden başlatma gerçekleştirmenizi öneririz.
  - Hizmetimizin yalnızca kaynak sistem (Azure Active Directory) kullanıcı/grup değişikliklerinin farkında olduğunu unutmayın. Kullanıcı/grup doğrudan uygulamada kaldırılırsa (örneğin, ServiceNow), bu değişikliklerin farkındayız ve kaynak sistemde kullanıcının durumuna göre geri almayız. Bu senaryoda, değişikliği doğrudan hedef uygulamada geri almak en iyisidir.
- Hizmetimiz, kullanıcı/grubu değerlendirdi ve sağlanması gerektiğini belirledi:
  - Kapsamı atanan kullanıcılar ve gruplar olarak ayardıysanız, kullanıcı/grubun uygulamaya atanmış olup olduğunu kontrol edin.
  - Kullanıcı/grup uygulamaya atanmışsa, bunların varsayılan erişim rolüne atanmay olduğundan emin olur. Bu rol, sağlama için kullanılamaz.
  - Özniteliği temel alan bircoping filtresi ayardıysanız, kullanıcının belirttiğiniz ölçütlere uygun olduğundan emin olur.
  - Kullanıcılar zaten hedef sistemde bulunuyorsa ve kullanıcının durumu kaynak ve hedef eşleşmede bulunuyorsa, başka bir işlemde yer almayacağız.
- Hizmetimiz kullanıcıya sağlamayı çalıştı ve başarısız oldu. Bu senaryolar için, sağlama günlüklerinin sorun giderme ve öneriler sekmesini gözden geçirebilirsiniz:
  - Kullanıcıda gerekli bir öznitelik Azure Active Directory'de eksik olabilir veya üçüncü taraf uygulamanın gerekli biçimiyle eşleşmez. Örneğin, bir kullanıcının Ülke özniteliği ABD olması gerektiği zaman ABD olarak ayarlanmış olabilir.
  - Öznitelik, henüz hedef uygulamada olmayan bir başvuru özniteliğidir. Bilgi tutarlısı özniteliği, örneğin bir grubun üyesi olan bir kullanıcı gibi başka bir nesneye başvuran özniteliktir. Kullanıcının kimliği grubun üye özniteliğinde yer alıyor olabilir, ancak yalnızca kullanıcı nesnesinde zaten var olduğunu gösterirse işlenebilir.
