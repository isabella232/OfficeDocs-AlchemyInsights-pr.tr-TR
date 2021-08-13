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
ms.openlocfilehash: 12490df735ca8c524058404df92db79c6c5682fe2ecafe2b42baed70fa3ab142
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53971359"
---
# <a name="user-provisioning"></a>Kullanıcı hazırlama

- Kullanıcı [sağlamak için isteğe bağlı sağlama](https://docs.microsoft.com/azure/active-directory/app-provisioning/provision-on-demand) özelliğini kullanın ve atılan adımlar hakkında ayrıntılı tanılama bilgileri alın.
- Kullanıcıları ve grupları sağlarken karşılaştığınız sorunları gidermek için, Şu sorun giderme [kılavuzuna bakın: Hiçbir kullanıcı sağnıyor.](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-config-problem-no-users-provisioned)
- Kullanıcıların sağlanmaz olduğunu gözlemlersanız, bkz. Azure Active Directory [(AD)](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs) için Günlük sağlama (önizleme). Belirli bir kullanıcıyla ilgili günlük girdilerini arama.
- Önceki sağlama döngüsünde gözden kaçırilen tüm kullanıcıları yakalamak için, belirli aralıklarla sağlamayı yeniden başlatın.
- Hizmetimiz, kullanıcıyı henüz değerlendirme fırsatı bu etmey olduğundan kullanıcı/grup sağlanmadı. Hazırlama yapılandırması sayfasında hem hazırlamanın ne kadar süreyle ilerle ilgili kılavuzu hem de ilerleme çubuğunu gözden geçirebilirsiniz. Ek ayrıntılar bölümünde belirtilen sabit durum kullanıcının oluşturulma/güncelleştirildikten/silindi tarihten önce geliyorsa, bu, kullanıcıyı henüz değerlendirmedik demektir. Bu senaryoda, en iyi şey sağlama hizmetinin bitip bitip bitene kadar beklemesini beklemektir. Durumu sabit bir şekilde sağlanmışsa, Azure Portal'daki kullanıcı arabiriminden yeniden başlatma gerçekleştirmenizi öneririz.
  - Hizmetimizin yalnızca kaynak sistem (kaynak sistem) kullanıcı/grup değişikliklerinin farkında olduğunu Azure Active Directory. Kullanıcı/grup doğrudan uygulamanın içinde kaldırılırsa (örneğin, ServiceNow), bu değişikliklerden haberdar olayız ve kaynak sistemde kullanıcının durumuna göre geri almayız. Bu senaryoda, değişikliği doğrudan hedef uygulamada geri almak en iyisidir.
- Hizmetimiz, kullanıcı/grubu değerlendirdi ve sağlanmazken belirlendi:
  - Kapsamı atanan kullanıcılar ve gruplar olarak ayardıysanız, kullanıcının/grubun uygulamaya atanmış olup değildir.
  - Kullanıcı/grup uygulamaya atanmışsa, bunların varsayılan erişim rolüne atanmaması gerekir. Bu rol, sağlama için kullanılamaz.
  - Öznitelik tabanlı bir yer arama filtresi ayardıysanız, kullanıcının belirttiğiniz ölçütlere uyanlara uygun olduğundan emin olur.
  - Kullanıcılar zaten hedef sistemde bulunuyorsa ve kullanıcının durumu kaynak ve hedef eşleşmede bulunuyorsa, başka işlem uygulamayacağız.
- Hizmetimiz kullanıcı sağlamayı denildi ve başarısız oldu. Bu senaryolar için, sağlama günlüklerinin sorun giderme ve öneriler sekmesini gözden geçirme:
  - Kullanıcıda gerekli bir öznitelik Eksik Azure Active Directory veya üçüncü taraf uygulamasının gerekli biçimiyle eşleşmez. Örneğin, bir kullanıcıda Ülke özniteliği ABD olması gerektiği zaman ABD olarak ayarlanmış olabilir.
  - Öznitelik, henüz hedef uygulamada olmayan bir başvuru özniteliğidir. Bilgi özniteliği, başka bir nesneyi(örneğin, bir grubun üyesi olan bir kullanıcı) olan bir özniteliktir. Kullanıcının kimliği grubun üye özniteliğinde yer alıyor olabilir, ancak yalnızca nesnenin zaten var olduğunu gösterirse işlenebilir.
