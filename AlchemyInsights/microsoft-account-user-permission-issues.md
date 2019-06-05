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
ms.openlocfilehash: 1825cfd0a78a29734d0a5128e19acbfba9115d32
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/04/2019
ms.locfileid: "34717366"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Sorun giderme sorun - kullanıcı dizinde bulunamadı

<p>Kullanıcılar <strong>hata iletisi alıyorsanız, &ldquo; &hellip;kullanıcı&rsquo;t dizinde bulunabilir. Lütfen yeniden deneyin&hellip; </strong> sorun türü olduğu <strong> &ldquo;kullanıcı değil, dizini.&rdquo;</strong>, sorunu gidermek için aşağıdaki adımları izleyin.</p> <ol> <li>Daha sonra oturum açmak için kullanılan aynı hesabı e-posta daveti olduğu kabul hesabına emin olun. Kullanıcı daveti kabul etmek ve siteye imzalamak için aynı hesabı kullandığından emin olun. <br /><br />Office 365 oturumu yönetmek için <a href="https://support.microsoft.com/en-us/help/12407/microsoft-account-how-to-manage-aliases">diğer adlar için Microsoft hesabınızı yönetme hakkında</a> daha fazla bilgi için bkz. <br /><br /></li> <li>Kullanıcı hatayı alıyor her site için göz atın. <br /><br />bir. Eklemek <strong> &ldquo;/_layouts/15/people.aspx/membershipgroupid=0&rdquo; </strong> (çift tırnak içinde) site URL'SİNİN sonuna. <br /><br />Örnek: https://&lt;contoso&gt;.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0 <br /><br />b. Kullanıcı listeden seçin. <br /><br />c. <strong>Şerit'ten kullanıcı izinlerini Kaldır</strong>' ı tıklatın. <br /><br />d. Yeniden kullanıcı ekleyin ve davet kullanıcıya yeniden gönderin.</li> </ol>

