---
title: Sorun giderme sorunu - Kullanıcı dizinde bulunamadı
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 3b863c5e9962dd29ca2ed41d113041d74830f615
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43702758"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Sorun giderme sorunu - Kullanıcı dizinde bulunamadı

Kullanıcılar dizinde "kullanıcı bulunamıyor" hata iletisi alıyorsa, lütfen Sorun Türü Kullanıcı'nın dizinde olmadığı yerlerde yeniden deneyin.

Sorunu gidermek için aşağıdaki adımlar tamamlanabilir.

- E-posta davetini kabul eden hesabın daha sonra oturum açmada kullanılan hesapla aynı olduğundan emin olun. Daveti kabul etmek ve sitede oturum açmak için kullanıcının aynı hesabı kullandığından emin olun. 

Daha fazla bilgi için, [Microsoft 365</a> oturumunu yönetmek için Microsoft hesabınıziçin takma adları nasıl yönetebilirsiniz'](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases)e bakın. 

- Kullanıcının hata aldığı her siteye göz atın. 

Site URL'sinin sonuna "/_layouts/15/people.aspx/membershipgroupid=0" (çift tırnak içinde) ekleyin. 

Örnek: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Listeden kullanıcıyı seçin.

- **Kullanıcı İzinlerini** Şeritten Kaldır'ı tıklatın. 
-  Kullanıcıyı geri ekleyin ve daveti kullanıcıya yeniden gönderin.

