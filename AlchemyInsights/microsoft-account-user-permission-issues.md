---
title: Oluşturma ve paylaşılan bir posta kutusu kullanma
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 81bf8082198de1c44037291f23c434d06a77f02a
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34762420"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Sorun giderme sorun - kullanıcı dizinde bulunamadı

Kullanıcı hata iletisi "kullanıcı bulunamadı" dizinde alıyorsanız. Yeniden burada sorun türü kullanıcı dizininde değil deneyin.

Bu sorunu gidermek için aşağıdaki adımları tamamlanabilir.

- Daha sonra oturum açmak için kullanılan aynı hesabı e-posta daveti olduğu kabul hesabına emin olun. Kullanıcı daveti kabul etmek ve siteye imzalamak için aynı hesabı kullandığından emin olun. 

Daha fazla bilgi için bkz: [diğer adlar için Microsoft hesabınızı yönetmek nasıl</a> Office 365 oturumu yönetmek için](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases). 

- Kullanıcı hatayı alıyor her site için göz atın. 

Eklemek "/ _layouts/15/people.aspx/membershipgroupid=0" (çift tırnak içinde) site URL'SİNİN sonuna. 

Örnek: https://_lT _"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Kullanıcı listeden seçin.

- Şerit'ten **kullanıcı izinlerini Kaldır** ' ı tıklatın. 
-  Yeniden kullanıcı ekleyin ve davet kullanıcıya yeniden gönderin.

