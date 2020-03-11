---
title: Windows 10'da parmak izi kilidini açma seçeneğini kullanma
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001689"
- "3765"
ms.openlocfilehash: 8a5059c722c306ad79811140062cec7f52f31766
ms.sourcegitcommit: 00e4266575438f55bdc18db05ed54aafcb75a3c9
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/11/2020
ms.locfileid: "42588335"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>Windows 10'da parmak izi kilidini açma seçeneğini kullanma

**Windows Hello Parmak İzini Etkinleştir**

Parmak izinizi kullanarak Windows 10'un kilidini açmak için en az bir parmak ekleyerek (Windows'un tanımayı öğrenmesine izin vererek) Windows Hello Parmak İzi'ni ayarlamanız gerekir. 

1. Hesaplar **> Ayarlar>a** gidin (veya [buraya](ms-settings:signinoptions?activationSource=GetHelp)tıklayın). Kullanılabilir oturum açma seçenekleri listelenir. Örneğin:

    ![Oturum açma seçenekleri.](media/sign-in-options.png)

2. **Windows Hello Parmak İzi'ni**tıklatın veya dokunun, ardından **Ayarla'yı**tıklatın. Windows Hello kurulum **penceresinde, Başlat'ı**tıklatın. Parmak izi sensörü devreye girer ve parmağınızı sensörün üzerine yerleştirmeniz istenir:

   ![Parmak izi sensörü.](media/fingerprint-sensor.png)

3. Parmağınızı tekrar tekrar tetmenizi isteyecek olan talimatları uygulayın. Bu işlem tamamlandığında, oturum açma için kullanmak isteyebileceğin diğer parmakları ekleme seçeneğiniz olur. Windows 10'da bir daha oturum açtığınızda, bunu yapmak için parmak izinizi kullanma seçeneğiniz olacaktır.

**Windows Hello Parmak İzi oturum açma seçeneği olarak kullanılamıyor**

Windows Hello Parmak İzi Oturum **Açma seçeneklerinde**bir seçenek olarak gösterilmiyorsa, Bu, Windows'un bilgisayarınıza bağlı herhangi bir parmak izi okuyucusunun/tarayıcısının farkında olmadığı veya bir sistem ilkesinin kullanımını engellediği anlamına gelir (örneğin bilgisayarınız işyeriniz tarafından yönetiliyorsa). Sorun gidermek için: 

1. Görev Çubuğu'ndaki **Başlat** düğmesini seçin ve **Aygıt Yöneticisi'ni**arayın.

2. **Aygıt Yöneticisi'ni**açmak için tıklatın veya dokunun.

3. Device Manager'da, köşeli ayraçlarını tıklatarak Biyometrik aygıtları genişletin.

   ![Biyometrik cihazlar.](media/biometric-devices.png)

4. Parmak izi tarayıcınız Synaptics WBDI tarayıcısı gibi biyometrik bir aygıt olarak listelenmelidir:

   ![Biyometrik cihazlar.](media/biometric-devices-expanded.png)

5. Parmak izi tarayıcınız gösterinmiyorsa ve tarayıcı bilgisayarınıza entegre edilmişse, BILGISAYAR üreticisinin web sitesine gidin. PC modelinizin teknik destek bölümünde, yükleyebileceğiniz bir tarayıcı için Windows 10 sürücüsü arayın.

6. Tarayıcı bilgisayardan ayrıysa (USB üzerinden bağlıysa), sahip olduğunuz tarayıcı modeli için Windows 10 aygıt sürücüsü yazılımını bulmak ve yüklemek için tarayıcı üreticisinin web sitesine gidin.
