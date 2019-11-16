---
title: Sorun giderme sorunu - Kullanıcı dizinde bulunamadı
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 59713231da25be441e7c05d788337e66bf17265a
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 11/15/2019
ms.locfileid: "37768821"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Sorun giderme sorunu - Kullanıcı dizinde bulunamadı

Kullanıcılar dizinde "kullanıcı bulunamıyor" hata iletisi alıyorsa, lütfen Sorun Türü Kullanıcı'nın dizinde olmadığı yerlerde yeniden deneyin.

Sorunu gidermek için aşağıdaki adımlar tamamlanabilir.

- E-posta davetini kabul eden hesabın daha sonra oturum açmada kullanılan hesapla aynı olduğundan emin olun. Daveti kabul etmek ve sitede oturum açmak için kullanıcının aynı hesabı kullandığından emin olun. 

Daha fazla bilgi için, [Office 365</a> oturumunu yönetmek için Microsoft hesabınıza takma adlar nasıl yönetilir'](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases)e bakın. 

- Kullanıcının hata aldığı her siteye göz atın. 

Site URL'sinin sonuna "/_layouts/15/people.aspx/membershipgroupid=0" (çift tırnak içinde) ekleyin. 

Örnek: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Listeden kullanıcıyı seçin.

- **Kullanıcı İzinlerini** Şeritten Kaldır'ı tıklatın. 
-  Kullanıcıyı geri ekleyin ve daveti kullanıcıya yeniden gönderin.

