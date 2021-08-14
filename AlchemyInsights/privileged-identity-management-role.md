---
title: Privileged Identity Management rolü
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "6825"
ms.openlocfilehash: 358e446192e6b58ace81afa06e0d65ae3a207282351ffc3ec9975a24779951fb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53973249"
---
# <a name="privileged-identity-managementpim-role"></a>Privileged Identity Management(PIM) rolü

**Bir rol etkinleştirdikten sonra izinler ver kullanıcılara verilmedi**

Azure AD Privileged Identity Management'de (PIM) bir rolü etkinleştirebilirsiniz, etkinleştirme anında ayrıcalıklı rolü gerektiren tüm portallara yayılmaz. Bazen, değişiklik yay bile olsa, portalda web önbelleğini önbelleğe almak değişikliğin hemen yürürlüğe alınmasını engellemeye neden olabilir.

Etkinleştirmeniz gecikirse şu adımları izleyin:

1. Azure portalında oturum açın ve sonra yeniden oturum açın. Bir Azure AD rolünü veya Azure kaynak rolünü etkinleştirebilirsiniz; etkinleştirmenizin aşamalarını da burada görüyorsunuz. Tüm aşamalar tamamlandıktan sonra bir 'Oturum açma' bağlantısı vardır. Oturumları imzalamak için bu bağlantıyı kullanabilirsiniz. Bu, etkinleştirme gecikmesi ile ilgili çoğu sorunu çözer.
2. PIM'de, rolün üyesi olarak listelenmiş olup kimliğinizi doğrulayın.
3. Kullanıcı Yöneticisi rolünü etkinleştir Exchange, oturum açma ve yeniden oturum açma. Sorun devam ederse bir destek bileti açın ve bunu sorun olarak yükseltin. Güvenlik ve Uyumluluk Merkezi'Exchange için Yönetici rolünü kullanıyorsanız, sonraki adıma bakın.
4. Güvenlik ve Uyumluluk Merkezi'ne erişmek için bir rol etkinleştirirseniz veya SharePoint Yöneticisi rolünü etkinleştirirseniz, etkinleştirme gecikmesi için birkaç dakika ile birkaç saat arasında bir gecikme yaşamanız gerekir. Bu bilinen bir sorundur ve bu sorunu en kısa sürede çözmek için bu ekiplerle birlikte etkin bir şekilde çalışıyoruz.

Daha fazla bilgi için bkz.:

- [PIM'de Azure AD rollerimi etkinleştirme](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [PIM'de Azure kaynak rollerimi etkinleştirme](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

**Rolün devre dışı bırakılması veya rol etkinleştirme süresinin dolması sonrasında izinler kaldırılamaz**

Azure AD Privileged Identity Management'de bir rolü devre dışı bırakıldığında veya bir rol etkinleştirme süresinin süresi dolduğunda, erişiminizin devam ettiği bir gecikme olabilir.

Devre dışı bırakmanız gecikirse şu adımları izleyin:

1. Exchange Yönetici rolünü veya rol etkinleştirme süresinin sona ererse ve izinler kaldırılmasına başlamadan önce önemli bir gecikme olduğunu fark ederseniz, bir destek bileti açın ve bu sorun hakkında Office'de Ayrıcalıklı Erişim Yönetimi (PAM) ekibiyle bilet dosyası dosyalaymanıza yardımcı olan destek mühendisinize yardım edin.
2. Etkinleştirme süresinin süresi dolmuşsa, ancak yine de tarayıcı oturumu açıksa, tarayıcınızı kapatın. Bu oturumu kapatana kadar rolü kullanmaya devamabilirsiniz. Bu bilinen bir sorundur ve etkinleştirmenin süresi dolduğunda her oturumun etkin olarak iptal edilebilir bir düzeltmesi için olası bir düzeltme üzerinde çalışmalarımız devam ediyor.

Gecikmeniz bu iki senaryodan farklı olursa lütfen bir destek bileti açın.
