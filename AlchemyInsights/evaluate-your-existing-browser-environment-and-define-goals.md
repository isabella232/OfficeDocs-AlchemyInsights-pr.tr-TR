---
title: Var olan tarayıcı ortamınızı değerlendirme ve hedefleri tanımlama
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9141"
- "9005291"
ms.openlocfilehash: 5b03d188aa78be83928cf262f1d86f3f933c85ab
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694818"
---
# <a name="evaluate-your-existing-browser-environment-and-define-goals"></a>Var olan tarayıcı ortamınızı değerlendirme ve hedefleri tanımlama

Geçerli tarayıcının durumunu ve proje görüşünü anlamak için zaman almak, tüm proje katılımcılarının uyumlu ve aynı hedefe yönelik çalışmalarına yardımcı olur. Şu adımları izleyin:

1. Geçerli eyaletinizi tanımlayın. Şunları göz önünde bulundurun:
- Şu anda ortamınıza hangi tarayıcılar dağıtılır?
- Hangi tarayıcı varsayılan tarayıcı olarak ayarlanır?
- Uygulamalarınızı bazıları için Internet Explorer'ı kullanmak zorunda mısınız?
- Internet Explorer'ı bugün yapılandırmak için Kurumsal Mod Site Listesi mi kullanıyorsunuz?
- Ortamınız Windows 10 ve macOS gibi hangi işletim sistemi platformlarını destekliyor?
- Tarayıcı yönetimi için hangi yönetim araçlarını kullanırsınız?
- Tarayıcı yapılandırması ve yönetiminden sorumlu olan kimdir?
- Tarayıcı uyumluluğunu doğrulama işlemi nedir?
2. Dağıtımınız için hedefleri tanımlayın. Aşağıdaki şeyleri unutmayın:
- [Microsoft Edge'i varsayılan tarayıcınız olarak ayarlamak istiyor musunuz?](https://docs.microsoft.com/DeployEdge/edge-default-browser)
- Microsoft Edge'in eski sürümünü gizlemek mi yoksa kullanıcıların kullanımına açık bırakmak [mı istiyorsunuz?](https://docs.microsoft.com/DeployEdge/microsoft-edge-sysupdate-access-old-edge)
- [Microsoft Edge'i nasıl yapılandıracaksınız?](https://docs.microsoft.com/DeployEdge/configure-microsoft-edge)
- İlk dağıtımınız kapsamında yapılandırmak için hangi özellikler kritik öneme sahiptir?
- Tanımlanan herhangi bir uyumluluk veya yapılandırma sorununa yönelik işlem nedir?
3. Kullanmak istediğiniz özelliklerin önkoşullarını anlıyoruz, örneğin:
- [Windows Defender Application Guard](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-application-guard/reqs-md-app-guard)
- [Internet Explorer modu](https://docs.microsoft.com/DeployEdge/edge-ie-mode)
- [Kimlik doğrulama ve eşitleme](https://docs.microsoft.com/DeployEdge/microsoft-edge-security-identity)

Bu adımları tamamlandıktan sonra, dağıtım stratejinizi planlamaya başlamaya hazır oluruz.
