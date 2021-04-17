---
title: Parola kullanmadan Windows 10'da oturum açma
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
ms.openlocfilehash: 1c03f00f7b41ea16d3106b19b998edeea6114603
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830566"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a>Parola kullanmadan Windows 10'da oturum açma

Windows başlangıçta parola yazmamak için PIN, yüz tanıma veya parmak izi gibi (varsa) Windows Hello güvenli oturum açma seçeneklerindan birini öneririz. Güvenli oturum açma özelliğini gerçekten devre dışı bırakmak için aşağıdaki "Windows 10'da otomatik olarak oturum açma" yönergelerine bakın.

**Hesap parolasının güvenli Windows Hello alternatifleri**

Oturum açma **seçenekleri > Hesaplar ve > ayarlar'a gidin (veya** buraya [tıklayın).](ms-settings:signinoptions?activationSource=GetHelp) Kullanılabilir oturum açma seçenekleri listelenir. Örneğin:

![Oturum açma seçenekleri.](media/sign-in-options.png)

Yapılandırmak için seçeneklerden birini tıklatın veya dokunun. Windows'u bir sonraki başlatacak veya kilidini açmayacaksanız, parola yerine yeni seçeneği kullanabilirsiniz. 

**Windows 10'da otomatik olarak oturum açma**

**Not:** Otomatik oturum açma kullanışlı bir oturum açmadır, ancak özellikle de bilgisayarınıza birden çok kişi tarafından erişilse bir güvenlik riski getirir. 

1. Görev çubuğunda Başlat **düğmesine** tıklayın veya dokunun.

2. Kullanıcı Hesapları penceresini açmak için **netplwiz** yazın ve Enter tuşuna basın.

3. Kullanıcı **Hesapları'nın** altında, Windows başlatıldığında otomatik olarak oturum açmasını istediğiniz hesaba tıklayın.

4. "Kullanıcıların bu bilgisayarı kullanmak için kullanıcı adı ve parola girmeleri gerekir" onay kutusunun işaretini kaldırın.

    ![Kullanıcıların bir kullanıcı adı ve parola seçeneği girmeleri gerekir.](media/users-must-enter-username.png)

5. **Tamam**'a tıklayın. Seçtiğiniz hesabın parolasını girmeniz ve onaylamanız istenir. Bitirmek **için Tamam'a** tıklayın. Windows 10 yeniden başlatıldığında, seçtiğiniz hesapta otomatik olarak oturum açılır.
