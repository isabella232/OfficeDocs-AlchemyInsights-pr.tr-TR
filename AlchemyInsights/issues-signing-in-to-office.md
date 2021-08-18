---
title: Microsoft 365 uygulamalarda oturum açma sorunları
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 7a8a0b68fc211e99b22e857d51d1de54e53a69357f75a0c60b1e83078cd5b27f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54088056"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Microsoft 365 uygulamalarında boş Microsoft 365 ekranı

Bu sorunu çözmek için şunları deneyin:
- Windows ve [Office](https://support.microsoft.com/help/4027667/windows-10-update) [için en son güncelleştirmeleri yükleyin.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- Internet Explorer seçeneklerini sıfırlama: Araçlar   >  **Internet Seçenekleri**  >  **Gelişmiş**  >  **Internet Explorer'ı sıfırlama Ayarlar** (özel ayarları kaybedeceğinizi unutmayın) gidin ve sonra Internet Explorer'da yeniden oturum Office deneyin.
- Güvenlik duvarını (WDAG) Windows Defender Application Guard güvenlik duvarı veya virüsten koruma programını devre dışı bırakma:
    1. Denetim Masası'nda **Programlar'a gidin** ve **Windows'ı seçin.**
    2. Etkin Windows Defender Application Guard, devre dışı bırakmayı deneyin.<br/>
    **Not:** Bilgisayarı yeniden başlatmanız gerekiyor olabilir.
- Microsoft.AAD.BrokerPlugin [AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) eklentisinin herhangi bir uygulama veya güvenlik duvarı/virüsten koruma programı tarafından engelli olmadığını kontrol edin.
- [Kimlik Office Yöneticisi'ni kullanarak](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) Windows temizleme.<br/>
    **Not:** Office 2016'nın kayıt defteri yolları 16.0 olarak değişti. (Örneğin: \Software\Microsoft\Office\16.0\Common\Identity\)

Daha fazla bilgi için bkz. [Windows 10'de Office 16.0.7967](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)derlemesi ile Office sonra oturum açma ile ilgili bağlantı Windows 10.