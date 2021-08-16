---
title: Sorun giderme - Kullanıcı dizinde bulunamadı
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 79429f8e9523ad6b08cd2cd2b19dd221bac797d00de142cbb18826b86fb5ae4e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54098190"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Sorun giderme - Kullanıcı dizinde bulunamadı

Kullanıcılar dizinde "kullanıcı bulunamadı" hata iletisini alıyorsa, sorun türü Dizinde yer almayan Kullanıcı'nın olduğu yerde lütfen yeniden deneyin.

Sorunu gidermek için aşağıdaki adımlar tamamlandıktan sonra.

- E-posta davetini kabul eden hesabın, daha sonra oturum aedken kullanılan hesap ile aynı olduğundan emin olun. Kullanıcının daveti kabul etmek ve sitede oturum a açması için aynı hesabı kullanıyor olduğundan emin olun. 

Daha fazla bilgi için [bkz. Oturum açma bilgilerini yönetmek için Microsoft </a> hesabınız için diğer Microsoft 365.](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases) 

- Kullanıcının hatayı alan sitelere göz atabilirsiniz. 

Site URL'sinin sonuna "/_layouts/15/people.aspx/membershipgroupid=0" (çift tırnak içinde) ekleyin. 

Örnek: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Listeden bir kullanıcı seçin.

- Şeritten **Kullanıcı İzinlerini Kaldır'a** tıklayın. 
-  Kullanıcı'ya yeniden ekleme ve kullanıcıya yeniden daveti yeniden davet etme.

