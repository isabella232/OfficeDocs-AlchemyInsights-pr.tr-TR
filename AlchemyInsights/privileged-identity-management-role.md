---
title: Ayrıcalıklı kimlik yönetimi rolü
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
ms.openlocfilehash: 726511d016462f56c48a4272b57abc3e9f0cbc3d
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 11/17/2020
ms.locfileid: "49089148"
---
# <a name="privileged-identity-managementpim-role"></a>Ayrıcalıklı kimlik yönetimi (PıM) rolü

**Rol etkinleştirildikten sonra izinler verilmez**

Azure AD ayrıcalıklı kimlik yönetimi 'nde (PıM) bir rol etkinleştirdiğinizde, etkinleştirme ayrıcalıklı rol gerektiren tüm portallarına anında yaymayabilir. Bazen, değişiklik yayılsa bile, portalda Web önbelleğe alma, değişikliğin hemen etkinleşmez.

Etkinleştirme gecikirse, şu adımları izleyin:

1. Azure portalında oturumu kapatın ve yeniden oturum açın. Bir Azure AD rolünü veya bir Azure Kaynak rolünü etkinleştirdiğinizde, etkinleştirme aşamaları görüntülenir. Tüm aşamalar tamamlandığında, ' oturumu Kapat ' bağlantısını görürsünüz. Oturumu kapatabilirsiniz. Bu, çoğu durumda etkinleştirme gecikmesini çözecektir.
2. PıM 'de, rolün üyesi olarak listelendiğini doğrulayın.
3. Exchange Yöneticisi rolünü etkinleştiriyorsanız, oturumunuzu kapatıp yeniden oturum açın. Sorun devam ederse, bir destek bileti açın ve bunu sorun olarak yükseltin. Güvenlik ve Uyumluluk Merkezi 'ne erişmek için Exchange Yöneticisi rolünü kullanıyorsanız, sonraki adıma bakın.
4. Güvenlik ve Uyumluluk Merkezi 'ne erişmek için bir rol etkinleştiriyorsanız veya SharePoint Yöneticisi rolünü etkinleştiriyorsanız, birkaç dakikadan birkaç saat kadar birkaç etkinleştirme gecikmeyle karşılaşırsınız. Bu bilinen bir sorundur ve bu ekiple en kısa sürede bu sorunu çözmek için etkin bir şekilde çalışmaktadır.

Daha fazla bilgi için bkz.:

- [PıM 'de Azure AD rollerimi etkinleştirme](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [PıM 'de Azure Resource rollerimi etkinleştirme](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

**Rolün etkinliğini kaldırdıktan sonra izinler kaldırılmıyor veya rol etkinleştirme süresi dolarsa**

Azure AD ayrıcalıklı kimlik yönetimi 'nde bir rolün etkinliğini kaldırdığınızda veya bir rol etkinleştirme dönemi sona erdiğinde, erişime sahip olduğunuz bir gecikme olabilir.

Devre dışı bırakma işlemi gecikirse, şu adımları izleyin:

1. Exchange Yöneticisi rolünü devre dışı bırakırsanız veya rol etkinleştirme dönemi sona erdiğinde, bir destek bileti açın ve Office 'in sahip olduğu ayrıcalıklı erişim yönetimi (PAM) ekibiyle bir bilet dosyalarınıza yardımcı olmak için destek mühendisinizden yardım alın.
2. Etkinleştirme süresi dolduysa, ancak hala tarayıcı oturumu açıksa tarayıcınızı kapatın. Bu oturumu kapatana kadar rolü kullanmaya devam edebilirsiniz. Bu bilinen bir sorundur ve etkinleştirmenin süresi dolduğunda oturumu etkin bir şekilde iptal etmek için olası bir düzeltmeye bakıyoruz.

Gecikme bu iki senaryodan farklıysa lütfen bir destek bileti açın.
