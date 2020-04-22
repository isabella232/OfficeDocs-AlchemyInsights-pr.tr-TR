---
title: Koşullu Erişimin İzlenmesi
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 8b76d58791408037b5704b421d7afa166e3ea0be
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713738"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Değişim için Koşullu Erişimin İzlenmesi

Koşullu erişim le hedeflenen kullanıcılar, kuruluşunuzun erişim gereksinimlerini karşılamadıkları takdirde bir bildirim e-postası alır. Çözmek için, aşağıdaki çözümlerden birini veya birkaçını öneririz:
  
- Cihazın kayıtlı olduğu varsayılsa, kullanıcıya Şirket Portalı uygulamasına gitmesini ve Şirket Portalı'nda göründüğünü doğrulamasını tavsiye edin. Değilse, kullanıcı aygıtı kaydetmelidir.
    
- Azure portalında **Intune \> Aygıt uyumluluğu'na**gidin. **Monitör** altında **Aygıt uyumluluğu'na**tıklayın. Kullanıcının aygıtının uyumlu olarak işaretlendiğini doğrulamak için cihazınızın uyumluluk raporunu görüntüleyin. 
    
- Azure portalında **Intune \> Aygıt uyumluluğu'na**gidin. **Yönet**altında, **İlkeler'i**tıklatın. Uyumluluk ilkeleri listesinde, kullanıcınızın cihazına bir profil atandığını doğrulayın. Profil atanmamışsa, Intune aygıtın uyumluluk durumunu onaylayamayacaktır. 
    
- Kullanıcının koşullu erişim atamasını edin.
    
1. Azure portalında **Intune \> Koşullu \> erişim İlkeleri'ne** gidin
    
2. Listeden bir ilke seçin
    
3. **Kullanıcılar ve gruplar'ı** tıklatın
    
4. Belirli bir ilkeyi birine hedeflemek için, bu politikayı **Ekle** listesine ekleyin. Bir kişinin ilkeden çıkarıldığından emin olmak için, bunları **Dışlayın** listesine ekleyin. 
    
Daha fazla bilgi: [Koşullu Erişim aygıtları nasıl izlenir?](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)
  

