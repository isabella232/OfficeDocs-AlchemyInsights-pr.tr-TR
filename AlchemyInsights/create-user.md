---
title: Kullanıcı oluşturma
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003231"
- "9403"
ms.openlocfilehash: 742ff857141d08031302fdcff7e49b3eef90e0f7
ms.sourcegitcommit: 186281d0b87d67f041c127d4334faa937da9a48a
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747030"
---
# <a name="create-user"></a>Kullanıcı oluşturma

**DUYURU:**

- [4 Ocak 2021'den](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) itibaren WebView oturum açma desteği Google tarafından kullanımdan silinecek. Uygulamalarınızı, Google'ın uyumluluğu test etme [kılavuzuna uyarak etkilendiğini](https://go.microsoft.com/fwlink/?linkid=2157323) test edin.
- Kullanıcılarınızı tüketici Google hesaplarıyla oturum aken sistem web görünümü veya sistem tarayıcısını kullanmaya emin olun. Daha fazla bilgi için, [yalnızca Chrome tarayıcısını kullanarak uygulamada oturum açma sorunlarına bakın.](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications)

**Azure AD dizinimde yeni bir kullanıcı oluşturamıyor**

1. Yeni bir standart kullanıcı oluşturma yetkisine sahip olduğunuzdan emin olmak. Yalnızca Azure Active Directory'de (AD) Genel yönetici veya Kullanıcı yöneticisi rolü yeni bir standart kullanıcı oluşturabilir. Bu rollerden birisinde değilseniz, bir yöneticiden sizi bu rollerden birini eklemesi veya sizin için yeni kullanıcı hesabı oluşturması için sorun.
1. Kullanıcı adının Azure AD'niz içinde doğrulanmış bir etki alanında olduğundan emin olun. Azure AD'sinde doğrulanmış özel etki alanı adları yoksa, *.onmicrosoft.com ile sona eren Azure AD başlangıç etki alanınızı kullanabilirsiniz.
1. Kullanıcı adının şirket içi AD'nizin Azure AD'sinde şirket dışından olmayan bir etki alanında olduğundan emin olun. Kullanıcılar şirket içi şirket dışından şirket dışından gelen etki alanı adlarına sahip olarak buluta ek kullanılamaz.
1. Yeni kullanıcıya atamak istediğiniz kullanıcı adının başka bir kullanıcı veya kişide yer alamaması gerekir. Kullanıcı adları Azure AD genelinde benzersiz olmalıdır.
1. [Azure AD'niz için Azure AD rollerine](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) ve yöneticilerine bakın.
1. Azure [AD'nizin](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) etki alanı adlara bakın.
1. Eylemi [kimin ve ne](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) zaman gerçekleştirmiş olduğu gibi, yakın zamanda oluşturulmuş veya silinmiş bir kullanıcı hakkında daha ayrıntılı bilgi görmek için Denetim günlüklerini gözden geçirebilirsiniz.
1. Yeni kullanıcı ekleme hakkında daha fazla bilgi için [Bkz. Azure AD'niz içinde yeni kullanıcı oluşturmak için Azure portalını kullanma.](/azure/active-directory/active-directory-users-create-azure-portal)
1. [Azure AD yönetim rolleri](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles): Azure Active Directory'de yönetici rolü izinleri
1. Yeni kullanıcı oluşturmak [için Azure AD PowerShell'i de kullanabilirsiniz.](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser?view=azureadps-2.0)
