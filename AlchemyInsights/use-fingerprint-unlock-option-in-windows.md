---
title: E-Windows 10'de parmak izi kilidi açma seçeneğini kullanma
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
ms.openlocfilehash: a171d889705a0035981465bdaa5a8f07b9d2eb7200ba4c948f2aaccbf2cc0a21
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972019"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>E-Windows 10'de parmak izi kilidi açma seçeneğini kullanma

**Parmak İzi Windows Hello Etkinleştirme**

Parmak izinizi Windows 10 kilidini açmak için en az bir parmağınızı ekleyerek (tanımayı öğrenmesine Windows) parmak izi Windows Hello parmak izi ayarlamanız gerekir. 

1. Oturum açma **Ayarlar > hesapları > gidin (veya** buraya [tıklayın).](ms-settings:signinoptions?activationSource=GetHelp) Kullanılabilir oturum açma seçenekleri listelenir. Örneğin:

    ![Oturum açma seçenekleri.](media/sign-in-options.png)

2. Parmak İzi **Tanıma'ya Windows Hello dokunun** ve ardından Ayarla **öğesine tıklayın.** Kurulum Windows Hello, Başla **'ya tıklayın.** Parmak izi algılayıcısı etkin hale gelecektir ve parmağınızı algılayıcıya şu şekilde koyabilirsiniz:

   ![Parmak izi algılayıcısı.](media/fingerprint-sensor.png)

3. Parmağınızı tekrar tekrar taramanızı soracak şekilde yönergeleri izleyin. Bu tamamlandığında, oturum açma için kullanmak istediğiniz diğer parmaklarınızı ekleme seçeneğiniz olur. bu e-posta Windows 10 oturum açsanız bile, bunu yapmak için parmak izinizi kullanma seçeneğiniz olur.

**Windows Hello Parmak izi oturum açma seçeneği olarak kullanılamıyor**

Oturum açma seçeneklerinde Windows Hello Parmak İzi seçeneği gösterilmiyorsa, bu Windows'in bilgisayarınıza bağlı herhangi bir parmak izi okuyucusu/tarayıcısı hakkında bilgi sahibi olmadığını veya sistem ilkesi bunun kullanımını engelley example (örneğin, bilgisayarınız çalışma alanınız tarafından yönetiliyorsa) anlamına gelir. Sorun gidermek için: 

1. Görev çubuğunda **Başlangıç** düğmesini seçin ve Cihaz **Yöneticisi'ni arayın.**

2. Cihaz Yöneticisi'ni açmak için **öğesine tıklayın veya dokunun.**

3. Cihaz Yöneticisi'nde, Biyometrik cihazları köşeli çift ayraçlarına tıklayarak genişletin.

   ![Biyometrik cihazlar.](media/biometric-devices.png)

4. Parmak izi tarayıcınız Synaptics WBDI tarayıcı gibi biyometrik bir cihaz olarak listelenmiş olmalı:

   ![Biyometrik cihazlar.](media/biometric-devices-expanded.png)

5. Parmak izi tarayıcınızın gösterilmezse ve tarayıcı bilgisayarınızla tümleşikse, bilgisayar üreticisinin web sitesine gidin. Bilgisayar modelinizin teknik destek bölümünde, yüklerini kurabilirsiniz Windows 10 tarayıcı sürücüsü için arama yapabilirsiniz.

6. Tarayıcı pc'den ayrı ise (USB ile takılı) sahip olduğunuz tarayıcı modeline uygun Windows 10 sürücü yazılımını bulmak ve yüklemek için tarayıcı üreticisinin web sitesine gidin.
