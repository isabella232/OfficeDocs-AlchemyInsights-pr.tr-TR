---
title: Windows 10'da parmak izi kilidi açma seçeneğini kullanma
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
- "9001689"
- "3765"
ms.openlocfilehash: ba1f2e7b0bb54e89178a320b8579b8d1bfdaff9a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51796697"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>Windows 10'da parmak izi kilidi açma seçeneğini kullanma

**Windows Hello Parmak İzi Tanımayı Etkinleştirme**

Windows 10'un kilidini parmak izinizi kullanarak açmak için windows hello parmak izi kilidini en az bir parmağınızı ekleyerek (Windows'un tanımasını öğrenmesine izin vererek) ayarlamanız gerekir. 

1. Oturum açma **seçenekleri > Hesaplar ve > ayarlar'a gidin (veya** buraya [tıklayın).](ms-settings:signinoptions?activationSource=GetHelp) Kullanılabilir oturum açma seçenekleri listelenir. Örneğin:

    ![Oturum açma seçenekleri.](media/sign-in-options.png)

2. Windows Hello Parmak **İzi Tanıma'ya tıklayın veya** dokunun, ardından Ayarla **öğesine tıklayın.** Windows Hello kurulum penceresinde, Başla **'ya tıklayın.** Parmak izi algılayıcısı etkin hale gelecektir ve parmağınızı algılayıcıya şu şekilde koyabilirsiniz:

   ![Parmak izi algılayıcısı.](media/fingerprint-sensor.png)

3. Parmağınızı tekrar tekrar taramanızı soracak şekilde yönergeleri izleyin. Bu tamamlandığında, oturum açma için kullanmak istediğiniz diğer parmaklarınızı ekleme seçeneğiniz olur. Windows 10'da bir sonraki oturum açsanız, bu şekilde parmak izinizi kullanma seçeneğiniz olur.

**Windows Hello Parmak İzi Tanıma oturum açma seçeneği olarak kullanılamıyor**

Oturum açma seçeneklerinde Windows Hello Parmak İzi İşareti seçeneği gösterilmiyorsa, Windows bilgisayarınıza bağlı herhangi bir parmak izi okuyucusu/tarayıcısı farkında değildir veya sistem ilkesi bunun kullanımını engellemektedir (örneğin, bilgisayarınız çalışma alanınız tarafından yönetiliyorsa). Sorun gidermek için: 

1. Görev çubuğunda **Başlangıç** düğmesini seçin ve Cihaz **Yöneticisi'ni arayın.**

2. Cihaz Yöneticisi'ni açmak için **öğesine tıklayın veya dokunun.**

3. Cihaz Yöneticisi'nde, Biyometrik cihazları köşeli çift ayraçlarına tıklayarak genişletin.

   ![Biyometrik cihazlar.](media/biometric-devices.png)

4. Parmak izi tarayıcınız Synaptics WBDI tarayıcı gibi biyometrik bir cihaz olarak listelenmiş olmalı:

   ![Biyometrik cihazlar.](media/biometric-devices-expanded.png)

5. Parmak izi tarayıcınızın gösterilmezse ve tarayıcı bilgisayarınızla tümleşikse, bilgisayar üreticisinin web sitesine gidin. Bilgisayar modelinize uygun teknik destek bölümünde, yük makineniz olan bir tarayıcı için Windows 10 sürücüsü aratırsınız.

6. Tarayıcı pc'den ayrı ise (USB ile takılı) sahip olduğunuz tarayıcı modeline uygun Windows 10 cihaz sürücüsü yazılımını bulmak ve yüklemek için tarayıcı üreticisinin web sitesine gidin.
