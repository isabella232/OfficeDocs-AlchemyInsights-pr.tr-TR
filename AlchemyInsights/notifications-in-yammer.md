---
title: Yammer’da bildirimler
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002878"
- "5480"
ms.openlocfilehash: ff4c13560b9cbf283e5c6b92a259debdf96cca62
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: HT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/27/2020
ms.locfileid: "43911922"
---
# <a name="notifications-in-yammer"></a>Yammer’da bildirimler

Uygun konuşmalarda yeni etkinlikle ilgili olarak sizi uyarmak için Yammer e-postayla [bildirimler gönderir](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996) veya Yammer’ı mobil cihazınızda kullanıyorsanız anında iletme bildirimleriyle uyarır. Varsayılan olarak Yammer ağınızdaki çok çeşitli etkinlik türleriyle ilgili bildirimler gönderir. Kullanıcılar e-posta ayarlarını Yammer web sitesi üzerinden güncelleştirebilir ve anında iletme bildirimleri mobil uygulama aracılığıyla yapılandırılır. 

Yammer, [Outlook’ta etkileşimli e-postalar](https://techcommunity.microsoft.com/t5/outlook-blog/interactive-yammer-emails-in-outlook-on-the-web-are-here/ba-p/1209420) için destek eklemiştir. Bazı e-postalar (iletinin kopyası) Web üzerinde Outlook’ta etkileşimli olacaktır. Önümüzdeki güncelleştirmelerden birinde bu özellik Outlook’un diğer sürümlerine de getirilecektir.

**Yammer’da bildirim türleri**

- E-postalar (Grubun güncelleştirmeleri, birinin sizi gruba davet etmesi, gelen kutunuzda ileti almanız vb.)
- Anında iletme bildirimleri (Sizden bahsedildiğinde, gelen kutunuzda ileti aldığınızda vb. mobil cihazlara gönderilir)
- Masaüstü açılan pencereleri (Yammer Masaüstü uygulamasını yüklediyseniz kullanıcılar için bildirimler görüntüler.)
- Zil bildirimleri (Yammer web sitesinin içinde kullanıcılar farklı olaylarla ilgili bildirimler görür. Her zaman bu bildirimlerle ilişkili e-posta veya anında iletme bildirimi olmayabilir.)

[Bildirimlerle ilgili daha ayrıntılı bilgiler](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996) sağlanmıştır.

**Bildirimleri yönetme**

Kullanıcıların kendi bildirimlerini yönetmesi gerekir. [Yammer e-posta ve mobil bildirimlerini etkinleştirme ve devre dışı bırakma](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996) konusunda bilgi sağlanmıştır.. 

Yöneticilerin tüm bildirimleri devre dışı bırakması veya kullanıcılar adına bildirimleri denetlemesi mümkün değildir. Yöneticiler [e-postalara eklenen logoyu ve kullanıcıların e-postayla gönderilen iletileri onaylaması gerekip gerekmediğini denetleyebilir](https://docs.microsoft.com/yammer/configure-your-yammer-network/configure-email-and-yammer).

**Kuruluşunuzdaki birçok kullanıcıya gönderilen e-posta bildirimleri**

Bazen Yammer tarafından tek bir e-posta bildirimi gönderilir ve bu bildirimi kuruluşunuzda beklenenden daha çok kullanıcı alır. Yammer’a dağıtım listesi veya bireysel olmayan başta türde bir e-posta adresi eklendiğinde bu durum oluşur. Yammer bir e-posta adresinin tek kullanıcıya mı ait olduğunu yoksa bunun bir e-postanın birçok alıcıya teslim edilmesine neden olacak bir e-posta adresi mi olduğunu her durumda bilemez. Bu sorun oluştuğunda Yammer’da [bu e-posta adresine sahip geçersiz kullanıcıyı askıya almak (devre dışı bırakmak)](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users) için eşlem gerçekleştirmeniz gerekir. 

Bu sorunun oluşma olasılığını azaltmak için:

1. Yammer’da [Office 365 kimliğini zorunlu tutmalısınız](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).
2. Dış gönderenlerin kuruluşunuza e-posta göndermesini engellemeli veya gönderenleri onaylı bir listeyle sınırlamalısınız.

Bu sorun oluşursa:

1. E-postanın alıcısını belirleyin; bu alıcı Yammer’daki kullanıcıyla eşleşmelidir. Örneğin all-in-sales@fabrikam.com tüm satış elemanlarını içeren bir dağıtım listesidir. Bu dağıtım listesi kullanıcılar tarafından alınan Yammer e-postasında tanımlanabilir.
2. [Ağ Yöneticisi’ndeki devre dışı bırakma (askıya alma) özelliğini](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users) kullanarak all-in-sales@fabrikam.com e-posta adresine sahip kullanıcıyı askıya alın. Askıya alma işlemi geri alınabilir, dolayısıyla silme işleminden daha güvenlidir. Kullanıcının silinmesi, 90 gün sonra otomatik olarak gerçekleşir.
3. İsteğe bağlı olarak, tek kullanıcı olmayan ve askıya alınması gereken diğer e-posta adreslerini belirlemek için [Kullanıcı Dışarı Aktarma](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data#ExportUsers) konusunu gözden geçirin.
