---
title: Office uygulamaları için oturum açma sorunları
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 08bb0a94066f071f2ba0e9c54378f0d479191496
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938375"
---
# <a name="blank-sign-in-screen-in-office-apps"></a>Boş oturum açma ekranı Office apps içinde

Bu sorunu gidermek için aşağıdakileri deneyin:
- [Windows](https://support.microsoft.com/help/4027667/windows-10-update) ve [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)ile ilgili en son güncelleştirmeleri yükleyin.
- Internet Explorer Seçenekleri sıfırla: **Araçlar** > **Internet Seçenekleri** > **Gelişmiş** > **Internet Explorer Ayarlarını Sıfırla** (özel ayarları kaybedersiniz unutmayın) ve Office için yeniden oturum açmayı deneyin.
- Windows Defender uygulama koruma (WDAG) veya benzer güvenlik duvarı veya virüsten koruma programını devre dışı bırakın:
    1. Denetim Masası ' nda **Programlar**gidin ve sonra da **Windows özelliklerini aç veya kapat'ı**seçin.
    2. Windows Defender uygulama koruyucusu etkinse, devre dışı bırakmayı deneyin.<br/>
    **Not:** Bilgisayarı yeniden başlatmanız gerekebilir.
- Microsoft.AAD.BrokerPlugin [AAD WAM eklenti](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) herhangi bir uygulama veya güvenlik duvarı/anti-virus programı tarafından engelleniyor değil emin olun.
- Windows kimlik bilgileri yöneticisini kullanarak [Office açık kimlik bilgileri](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) .<br/>
    **Not:** Office 2016 için kayıt defteri yolları için 16.0 değişti. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)

Daha fazla bilgi için bkz: [oturum bileşeninde Office 2016 yapı 16.0.7967 Windows 10 üzerinde güncelleştirme sonra bağlantı sorunları](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).