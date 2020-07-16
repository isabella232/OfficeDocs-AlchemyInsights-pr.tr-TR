---
title: Yammer'da dosya açma veya indirme sorunu
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6041"
- "9003112"
ms.openlocfilehash: 6dfcbe9abfc23219a61e81785d31c11f7a0fa95c
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148438"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a>Yammer'da dosya açma veya indirme sorunu

Klasik Yammer, iletilere ve gruplara dosya yüklemeleri için birden çok seçeneği destekler. Ağ yapılandırmasına bağlı olarak, dosyalar SharePoint'te depolama için varsayılan dır.

Yeni Yammer dosya seçici henüz klasik Yammer mevcut tüm seçenekleri desteklemez. Gelecekteki bir güncelleştirme ek özellikler ekler. Daha fazla bilgi için bkz: [Bir Yammer konuşma gönderisine dosya veya resim ekle.](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8)

**Dosya açılmıyor veya indiremiyor**  

Bir dosya Yammer'a yüklenebilir, ancak SharePoint Online'daki bir dosyaya da bağlantı verebilir. Sorun gidermek için önce dosyanın konumunu belirlemeniz gerekir. Dosya Yammer'a yüklenmişse, *.yammer.com URL'si olacaktır. Gerekli URL'lerin ve IP adreslerinin engelinin kaldırDığından emin olun. Daha fazla bilgi için, [Yammer için sabit kodlu IP adreslerini kullanarak](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592)blog yazısına bakın tavsiye edilmez.

Aynı zamanda genel yönetici olan bir kullanıcının dosyayı karşıdan yükleyip indiremeyeceğini kontrol edin. Dosya özelse, Özel İçerik Modu'nu kullanmanız gerekebilir. Daha fazla bilgi için, daha sonra [Yammer özel içeriği izleyin](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content)bakın.  

**Yammer ağ düzeyinde konuklar ve SharePoint Online dosyaları**  

[Yammer'daki ağ düzeyindeki konuklar](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) Azure AD B2B kullanmaz ve Yammer hizmetine dahil olduğundan SharePoint'te depolanan Yammer dosyalarına erişemezler. Bu kimliği kullanarak SharePoint Online'daki belge kitaplıklara erişebilen harici bir AAD B2B kullanıcısı oluşturun. Yammer'da gelecekteki Azure AD B2B konuk desteği hakkında daha fazla bilgi için, [Yammer Preview - Müşteri Koşulları ve SSS'de İşletmeden İşletmeye (B2B) Konuk desteğine](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer)bakın.