---
title: Edge tarayıcısı kullanılarak göstergeler çalışmıyor
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11230"
- "9005470"
ms.openlocfilehash: 2a48a49ec52a585e450edf448bc9203cd9c3f935
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326281"
---
# <a name="indicators-dont-work-using-edge-browser"></a>Edge tarayıcısı kullanılarak göstergeler çalışmıyor

Siz bir Gösterge oluşturduktan sonra, Edge (SmartScreen) tarafından buna gerek yok. Daha fazla bilgi için [bkz. IP'ler ve URL'ler/etki alanları için göstergeler oluşturma.](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/indicator-ip-domain)

## <a name="step-1-ensure-the-following"></a>1. Adım: Aşağıdakilerin

- Göstergenin doğru olduğunu doğrulayın (IP/URL'de yazım hatası yok, doğru eylem, doğru RBAC grupları).
- Olası gecikme sürelerini dikkate almak için göstergeyi oluşturdukten sonra en az 2 saat bekleyin.
- Sistemlerin Uç Nokta için Microsoft Defender'a ekli olduğunu onaylayın.
- Sistemlerin Bulut ile iletişim kurayalı olduğunu doğrulayın.
- Test sitesine gidip SmartScreen'in etkinleştirildiğinden ve erişilebilir olduğunu [doğrulayın.](https://demo.smartscreen.msft.net)

## <a name="step-2-troubleshoot-the-potential-issue"></a>2. Adım: Olası sorunu giderme

- İstemcinin gereksinimleri karşı olduğundan emin olun. Ayrıntılar için [bkz. IP'ler ve URL'ler/etki alanları için göstergeler oluşturma.](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/indicator-ip-domain)
- Edge tarayıcısının en son sürümünü çalıştırmayı deneyin. En son sürümü bulmak için [bkz. Sahip Microsoft Edge sürümüne sahip olun.](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb)
- Edge tarayıcısını yeniden başlatın.
- Ayarda bir gösterge bulunan siteye gidin. Site beklendiği gibi görünmüyorsa, 3. Adıma geçin. 

## <a name="step-3-collect-data"></a>3. Adım: Veri toplama

- **MDEClientAnalyzer tanılama** verilerini toplayın. Yönergeler için [bkz. Uç Nokta için Microsoft Defender'a makine ekleme ile ilgili sorunlar.](issues-with-onboarding-machines.md)
- Fiddler izlemesini yükleme ve toplama konusunda sorun görmüyorsanız bkz. [Telerik Fiddler](http://www.telerik.com/fiddler).
- Microsoft Desteği'nin yönlendirmelerini tercih ediyorsanız destek vakalarını açmak için aşağıdaki Destek simgesini seçin.
