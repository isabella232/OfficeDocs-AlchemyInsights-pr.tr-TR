---
title: Sorun giderme-Kullanıcı dizininde bulunamadı
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 512494a69ab274af00962cb9777a3479b4200fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725427"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Sorun giderme-Kullanıcı dizininde bulunamadı

Kullanıcılar, dizinde "Kullanıcı bulunamıyor" hata iletisi alıyorsa, lütfen sorun türünün Kullanıcı dizininde olmadığı durumlarda yeniden deneyin.

Sorunu gidermek için aşağıdaki adımlar tamamlanabilir.

- E-posta davetini kabul eden hesabın, daha sonra oturum açmak için kullanılan hesapla aynı olduğundan emin olun. Kullanıcının daveti kabul edip sitede oturum açarken aynı hesabı kullanmasını sağlayın. 

Daha fazla bilgi için Microsoft [hesabınızın diğer adlarını nasıl yöneteceğinizi </a> Microsoft 365 oturum açmayı yönetmeye](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases)bakın. 

- Kullanıcının hatayı aldığı her siteye göz atın. 

"/_Layouts/15/People.aspx/membershipgroupid = 0" (çift tırnak içinde) site URL 'sinin sonuna ekleyin. 

Örnek: https://< "contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Listeden kullanıcıyı seçin.

- Şeritteki **Kullanıcı Izinlerini kaldır** 'ı tıklatın. 
-  Kullanıcıyı geri ekleyin ve daveti kullanıcıya yeniden gönderin.

