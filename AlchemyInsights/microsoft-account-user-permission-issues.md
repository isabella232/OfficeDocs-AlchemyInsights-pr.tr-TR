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
ms.openlocfilehash: 81b9dafe8e27e5f73fe232c51ff56fed3fec29b4
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36754212"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Sorun giderme sorunu - Kullanıcı dizinde bulunamadı

Kullanıcılar dizinde "kullanıcı bulunamıyor" hata iletisi alıyorsanız. Lütfen Sorun Türü Kullanıcı dizininde olmadığı yerde yeniden deneyin.

Sorunu gidermek için aşağıdaki adımlar tamamlanabilir.

- E-posta davetini kabul eden hesabın daha sonra oturum açmada kullanılan hesapla aynı olduğundan emin olun. Daveti kabul etmek ve sitede oturum açmak için kullanıcının aynı hesabı kullandığından emin olun. 

Daha fazla bilgi için, [Office 365</a> oturumunu yönetmek için Microsoft hesabınıza takma](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases)adlar nasıl yönetilir' e bakın. 

- Kullanıcının hata aldığı her siteye göz atın. 

Site URL'sinin sonuna "/_layouts/15/people.aspx/membershipgroupid=0" (çift tırnak içinde) ekleyin. 

Örnek: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Listeden kullanıcıyı seçin.

- **Kullanıcı İzinlerini** Şeritten Kaldır'ı tıklatın. 
-  Kullanıcıyı geri ekleyin ve daveti kullanıcıya yeniden gönderin.

