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
ms.openlocfilehash: 800baae2d748708d8cb7a5fb0e73fce5dcf455cb
ms.sourcegitcommit: 2d617ae59eed0ce8b571339ceefce6473c03b94c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52569767"
---
# <a name="create-user"></a>Kullanıcı oluşturma

**DUYURU:**

- [4 Ocak 2021'den](/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) itibaren WebView oturum açma desteği Google tarafından kullanımdan silinecek. Uygulamalarınızın, Google'ın uyumluluğu test [etme kılavuzuna](https://go.microsoft.com/fwlink/?linkid=2157323) göre etkilendiğini test edin.
- Kullanıcılarınızı tüketici Google hesaplarıyla oturum aken sistem webview veya sistem tarayıcısını kullanmaya emin olun. Daha fazla bilgi için [bkz. Yalnızca Chrome tarayıcısını kullanarak](/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications)uygulamada oturum açma sorunları .

**Azure AD dizinimde yeni bir kullanıcı oluşturamıyor**

1. Yeni standart kullanıcı oluşturma yetkinizin olduğundan emin olmak. Yalnızca Genel yönetici veya Kullanıcı yöneticisi rolü Azure Active Directory (AD) yeni bir standart kullanıcı oluşturabilir. Bu rollerden biri değilseniz, bir yöneticiden sizi bu rollerden birini eklemesi veya sizin için yeni kullanıcı hesabı oluşturması için bir yöneticiden izin isteme.
1. Kullanıcı adının Azure AD'niz içinde doğrulanmış bir etki alanında olduğundan emin olun. Azure AD'sinde doğrulanmış özel etki alanı adları yoksa *.onmicrosoft.com ile sona eren Azure AD ilk etki onmicrosoft.com.
1. Kullanıcı adının şirket içi AD'niz tarafından Azure AD ile şirket dışında bir etki alanında olduğundan emin olun. Kullanıcılar şirket içinde şirket dışından şirket dışından alınan etki alanı adlarına sahip olarak buluta ek olamaz.
1. Başka hiçbir kullanıcının veya kişinin, yeni kullanıcıya atamak istediğiniz kullanıcı adına zaten sahip olduğundan emin olmak. Kullanıcı adları, Azure AD genelinde benzersiz olmalıdır.
1. Bkz. [Azure AD'niz için](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) Azure AD rolleri ve yöneticileri.
1. Azure [AD'nizin](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) etki alanı adlara bakın.
1. Eylemi [kimin ne zaman](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) gerçekleştirmiş olduğu gibi yakın zamanda oluşturulan veya silinen bir kullanıcı hakkında daha ayrıntılı bilgi görmek için Denetim günlüklerini gözden geçirebilirsiniz.
1. Yeni kullanıcı ekleme hakkında daha fazla bilgi için [bkz. Azure AD'niz içinde](/azure/active-directory/active-directory-users-create-azure-portal)yeni kullanıcı oluşturmak için Azure portalını kullanma.
1. [Azure AD yönetim rolleri](/azure/active-directory/active-directory-assign-admin-roles): Etki alanı içinde yönetici Azure Active Directory
1. Yeni kullanıcı [oluşturmak için Azure AD PowerShell'i de kullanabilirsiniz.](/powershell/module/azuread/new-azureaduser?view=azureadps-2.0)
