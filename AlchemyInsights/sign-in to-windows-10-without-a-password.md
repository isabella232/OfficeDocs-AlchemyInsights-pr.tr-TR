---
title: Parola kullanmadan Windows 10 oturum açma
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
- "9001690"
- "3766"
ms.openlocfilehash: fbf190d433eabfee5b45348d05d918222a385314a431812aa5f5926aacf11560
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54107540"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a>Parola kullanmadan Windows 10 oturum açma

Başlangıçta parola yazmamak için Windows varsa PIN, yüz tanıma veya parmak izi gibi Windows Hello güvenli oturum açma seçeneklerindan birini öneririz. Güvenli oturum açma özelliğini gerçekten devre dışı bırakmak için aşağıdaki "Oturum açmada otomatik olarak oturum Windows 10" yönergelerine bakın.

**Hesap Windows Hello alternatifleri için güvenlik sağlama**

Oturum açma **Ayarlar > hesapları > gidin (veya** buraya [tıklayın).](ms-settings:signinoptions?activationSource=GetHelp) Kullanılabilir oturum açma seçenekleri listelenir. Örneğin:

![Oturum açma seçenekleri.](media/sign-in-options.png)

Yapılandırmak için seçeneklerden birini tıklatın veya dokunun. Parolayı bir sonraki Windows açsanız veya kilidini açsanız bile, parola yerine yeni seçeneği kullanabilirsiniz. 

**E-postada otomatik olarak oturum Windows 10**

**Not:** Otomatik oturum açma kullanışlı bir oturum açmadır, ancak özellikle de bilgisayarınıza birden çok kişi tarafından erişilse bir güvenlik riski getirir. 

1. Görev çubuğunda Başlat **düğmesine** tıklayın veya dokunun.

2. Kullanıcı Hesapları penceresini açmak için **netplwiz** yazın ve Enter tuşuna basın.

3. Kullanıcı **Hesapları'nın** altında, hesap başlatıldığında otomatik olarak oturum açmasını istediğiniz Windows tıklayın.

4. "Kullanıcıların bu bilgisayarı kullanmak için kullanıcı adı ve parola girmeleri gerekir" onay kutusunun işaretini kaldırın.

    ![Kullanıcıların bir kullanıcı adı ve parola seçeneği girmeleri gerekir.](media/users-must-enter-username.png)

5. **Tamam**'a tıklayın. Seçtiğiniz hesabın parolasını girmeniz ve onaylamanız istenir. Bitirmek **için Tamam'a** tıklayın. Bir Windows 10 başlatıldığında, seçtiğiniz hesapta otomatik olarak oturum açılır.
