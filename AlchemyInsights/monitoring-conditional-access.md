---
title: Koşullu erişimi izleme
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 6083fc427e3791fdb0907198b525337a0c987c4e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47702923"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Exchange için koşullu erişimi izleme

Koşullu erişimle hedeflenen kullanıcılar kuruluşunuzun erişim gereksinimlerini karşılamıyorsa bildirim e-postası alır. Sorunu çözmek için, aşağıdaki çözümlerden bir veya daha fazlasını öneririz:
  
- Cihazın kayıtlı olduğu kabul ediyorsanız, kullanıcının Şirket Portalı uygulamasına gitmesini ve şirket portalında göründüğünü doğrulamasını tavsiye edin. Yoksa, Kullanıcı cihazı kaydetmelidir.
    
- Azure portalında **Intune \> cihaz uyumu**'na gidin. **Monitör** altında **cihaz uyumluluğu**'nı tıklatın. Cihazın uyumluluk raporunuzu görüntülemek için, kullanıcının cihazının uyumlu olduğunu doğrulayın. 
    
- Azure portalında **Intune \> cihaz uyumu**'na gidin. **Yönet**altında, **ilkeler**'e tıklayın. Uyumluluk ilkeleri listesinde, kullanıcının cihazına bir profilin atandığını doğrulayın. Atanmış profil yoksa, Intune cihazın uyumluluk durumunu doğrulayamayacaktır. 
    
- Kullanıcının koşullu erişim atamasını düzenleyin.
    
1. Azure portalında **Intune \> koşullu erişim \> ilkelerine** git
    
2. Listeden bir ilke seçin
    
3. **Kullanıcılar ve gruplar** 'ı tıklatın
    
4. Belirli bir ilkeyi bir başkasından hedeflemek için bunları **ekleme listesine ekleyin** . Bir kişinin ilkeden atlandığından emin olmak için bunları **dışlama** listesine ekleyin. 
    
Daha fazla bilgi: [koşullu erişim aygıtlarını izleme](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)
  

