---
title: Intune aygıtlarını uzaktan yönetmek için TeamViewer'ı kullanma
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1284"
- "6700008"
ms.openlocfilehash: 63e7f068f3c53240ad13d1679df460c97a1a94f4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555753"
---
# <a name="use-teamviewer-to-remotely-administer-intune-devices"></a>Intune aygıtlarını uzaktan yönetmek için TeamViewer'ı kullanma

Intune tarafından yönetilen aygıtlar [TeamViewer](https://www.teamviewer.com/)kullanılarak uzaktan yönetilebilir.

TeamViewer'ı kullanarak Intune'u yönetmek için şu adımları kullanın: 

Intune'da TeamViewer Bağlayıcısı'nı kurmak için TeamViewer'dan kimlik bilgileri alarak başlayın. Bu, yöneticinin Intune ve TeamViewer hizmeti arasındaki bağlantıyı kurmak için bir kerelik işlem olan Aygıtlar altında TeamViewer Bağlayıcı Ara Birimi'ne kimlik bilgilerini girmesini sağlar.

**Bölüm 1: Oturumu uzak bir aygıtla başlatma**

1. **Tüm aygıtların**altında, uzaktan oturum başlatmak istediğiniz aygıtı seçin.
2. Kaynak: **... Daha fazla**, **Yeni uzaktan yardım oturumu**seçin.
3. Uzak bir oturum oluşturmak istediğinizi kabul etmek için **Evet'i** seçin.
    "Yeni bir uzaktan oturum başlatma" isteği TeamViewer hizmeti tarafından onaylandıktan sonra, aygıt için Genel Bakış (veya Temel Bilgiler) bölmesinin ayrıntıları altında **uzaktan yardımı başlatma** seçeneğini görürsünüz. Bölmeyi genişletmek ve Uzaktan Yardım durumunu göstermek için **Daha Fazla yı** seçin.
4. Oturumu yönetici tarafında başlatmak için **uzak oturumu başlat'ı** seçin.
5. TeamViewer ikilisini (Windows) indirmeyi seçin ve **Çalıştır'ı**seçin.<br/>
    **Not** TeamViewer web sitesine açılan herhangi bir web tarayıcısayfasını yok sayabilirsiniz.

6. TeamViewer uygulamasının aygıtta değişiklik yapma isteğini kabul edin (yalnızca Windows).
7. TeamViewer uygulaması başlatılır ve uzak aygıtla bağlantının kimliğini doğrulamak için oturum kodunu içerir.

**Bölüm 2: Uzak bir oturum için hedeflenen aygıtta**

1. Intune şirket portalını açın.
2. Bildirim bayrağına bakın: "BT yöneticiniz uzaktan yardım oturumu için bu aygıtın denetimini istiyor" ve bildirimi seçin.
3. TeamViewer uygulamasını indirmeyi seçin veya TeamViewer uygulamasının uygulama mağazasından indirilmeyi kabul edin ve **Çalıştır'ı**seçin.
    **Not** TeamViewer web sitesine açılan herhangi bir web tarayıcısayfasını yok sayabilirsiniz.

4. TeamViewer uygulamasının aygıtta değişiklik yapma isteğini kabul edin (yalnızca Windows).
5. TeamViewer uygulaması başlatılır ve uzak aygıtla bağlantının kimliğini doğrulamak için oturum kodunu içerir.
6. Açılır pencere, oturumun başlamasına izin vermek isteyip istemediğinizi sorar.

**Not** TeamViewer hizmeti tarafından oluşturulan oturum kodları yalnızca tek seferlik kullanımdır. Bağlantıyı kaybederseniz, şunları

1. TeamViewer uygulamasıörneğini uzak aygıtta ve yönetici iş istasyonunda kapatın.
2. Uzak aygıttaki şirket portalını kapatın.
3. Yönetici portalından yeni bir "Yeni uzaktan Yardım oturumu" başlatın.
4. Yeni bildirimi almak için uzak aygıttaki şirket portalını yeniden açın.
5. TeamViewer uygulamasını daha önce olduğu gibi hem uzak aygıtta hem de yönetici iş istasyonunda indirin ve açın.