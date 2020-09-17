---
title: Windows 10 ' da parmak izi kilidini kullanma seçeneğini kullanma
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001689"
- "3765"
ms.openlocfilehash: 99f037f62748c06d77b526e35f67b711885c4a1e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47795264"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>Windows 10 ' da parmak izi kilidini kullanma seçeneğini kullanma

**Windows Hello parmak Izini etkinleştirme**

Parmak izinizi kullanarak Windows 10 ' un kilidini açmak için, en az bir parmağınızı ekleyerek (Windows 'un tanıyacağı konusunda izin vererek) Windows Hello parmak Izini ayarlamanız gerekir. 

1. **> hesap > oturum açma seçenekleri** 'ne gidin (veya [burayı](ms-settings:signinoptions?activationSource=GetHelp)tıklatın). Kullanılabilir oturum açma seçenekleri listelenir. Örneğin:

    ![Oturum açma seçenekleri.](media/sign-in-options.png)

2. **Windows Hello parmak izi**'ne tıklayın veya dokunun, ardından **Ayarla**'ya tıklayın. Windows Hello kurulumu **penceresinde başlayın 'ı tıklatın.** Parmak izi algılayıcısı etkinleştirilir ve parmağınızı algılayıcının üzerine yerleştirmenizi istenecektir:

   ![Parmak izi algılayıcısı.](media/fingerprint-sensor.png)

3. Parmağınızı izleyerek parmağınızı sürekli taramanızı ister. Bu tamamlandığında, oturum açmak için kullanmak isteyebileceğiniz başka parmağınızı ekleme seçeneğiniz olur. Windows 10 ' da bir sonraki oturum açışınızda, parmak izinizi kullanarak bunu yapabilirsiniz.

**Windows Hello Parmak Izi oturum açma seçeneği olarak kullanılamaz**

Windows Hello Parmak Izi **oturum açma seçeneklerinde**bir seçenek olarak gösterilmiyorsa, Windows 'un bilgisayarınıza bağlı parmak izi okuyucusunun/tarayıcısının farkında olmadığı veya sistem ilkesinin kullanımını engellediğini (ÖRNEĞIN, PC 'niz iş yeriniz tarafından yönetiliyorsa). Sorun gidermek için: 

1. Görev çubuğundaki **Başlat** düğmesini seçin ve **Cihaz Yöneticisi 'ni**arayın.

2. **Aygıt Yöneticisi 'ni**açmak için tıklayın veya dokunun.

3. Aygıt Yöneticisi 'nde, Çift Ayraca tıklayarak biyometrik cihazları genişletin.

   ![Biyometrik cihazlar.](media/biometric-devices.png)

4. Parmak izi tarayıcınız, Synaptics ILEDI tarayıcısı gibi bir biyometrik aygıt olarak listelenmelidir:

   ![Biyometrik cihazlar.](media/biometric-devices-expanded.png)

5. Parmak izi tarayıcınız gösterilmiyorsa ve tarayıcı bilgisayarınızla tümleşikse, bılgısayar üreticisinin Web sitesine gidin. PC modelinizin teknik destek bölümünde, yükleyebileceğiniz bir tarayıcı için Windows 10 sürücüsü arayın.

6. Tarayıcı PC 'den ayrıdır (USB ile bağlı), sahip olduğunuz tarayıcı modeli için Windows 10 cihaz sürücüsü yazılımını bulmak için tarayıcı üreticisinin Web sitesine gidin.
