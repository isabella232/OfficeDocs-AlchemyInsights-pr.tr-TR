---
title: Koşullu erişim izleme
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 374814f4eabd61433a15876ebf7f351819933c21
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36538798"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Koşullu erişim için Exchange izleme

Kuruluşunuzun erişim gereksinimlerini karşılamıyorsa koşullu erişim ile hedeflenen kullanıcılara bildirim e-posta alacaksınız. Çözmek için aşağıdakilerden birini veya daha fazlasını aşağıdaki çözümleri öneririz:
  
- Aygıt için kaydı kabul edilir, kullanıcı şirket Portal app için gidin ve şirket portalda göründüğünden emin olun önerin. Seçili değilse, kullanıcı aygıtı kaydetmeniz gerekir.
    
- Azure portalda gitmek için **Intune \> aygıt uyumluluğu**. **Aygıt uyumluluğu**altında **İzleyicisi'ni** tıklatın. Kullanıcının aygıt uyumlu olarak işaretlendiğini doğrulamak için aygıt uyumluluğu raporu görüntüleyin. 
    
- Azure portalda gitmek için **Intune \> aygıt uyumluluğu**. **Yönet**altında **ilkeleri**' ni tıklatın. Uyumluluk ilkeler listesinde bir profil, kullanıcının aygıta atanmış olduğunu doğrulayın. Profil atanırsa, Intune aygıtın uyum durumu onaylamak mümkün olmayacak. 
    
- Kullanıcının koşullu erişim atama düzenleyin.
    
1. Azure portalda gitmek için **Intune \> koşullu erişim \> ilkeler**
    
2. Bir ilkeyi listeden seçin.
    
3. **Kullanıcılar ve gruplar'ı** tıklatın.
    
4. Belirli bir ilke birisi olarak hedeflemek için **ekleme** listesine ekleyin. Bir kişinin ilkesinden atlanır sağlamak için **dışlama** listesine ekleyin. 
    
Daha fazla bilgi: [Monitör koşullu erişim aygıtları nasıl](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)
  

