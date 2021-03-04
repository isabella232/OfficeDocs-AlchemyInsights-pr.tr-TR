---
title: GPO Dağıtımı
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "8602"
ms.openlocfilehash: d31f77e70e8456a4076a8146025f1f8ada977a06
ms.sourcegitcommit: 969219d6dff18d86d679d4d8741d1e39e4ce9539
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/03/2021
ms.locfileid: "50428049"
---
# <a name="gpo-deployment"></a>GPO Dağıtımı

Azure Active Directory Etki Alanı Hizmetleri'nden (Azure AD DS) kullanıcı ve bilgisayar nesnelerinin ayarları çoğunlukla Grup İlkesi Nesneleri (GPOS) kullanılarak yönetilir. Azure AD DS, AADDC Kullanıcıları ve AADDC Bilgisayarlar kapsayıcıları için yerleşik GPO'lar içerir. Bu yerleşik GPO'ları, ortamınız için gereken grup ilkesi yapılandıracak şekilde özelleştirebilirsiniz. Azure AD DC yönetici grubunun üyeleri, Azure AD DS etki alanında grup ilkesi yönetimi ayrıcalıklarına sahiptir ve özel GPO'lar ve kuruluş birimleri de (OU) oluşturabilirler. Grup ilkesi nedir ve nasıl çalışır hakkında daha fazla bilgi için, Grup İlkesine [Genel Bakış'a bakın.](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11))

Karma bir ortamda, şirket içi AD DS ortamında yapılandırılan grup ilkeleri Azure AD DS ile eşitlenmez. Azure AD DS'de kullanıcılara veya bilgisayarlara yönelik yapılandırma ayarlarını tanımlamak için varsayılan GPOS'lardan birini düzenleyin veya özel bir GPO oluşturun.

Bu makalede [Grup](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) İlkesiNi yönet, Grup İlkesi Yönetim araçlarının nasıl yüklenemez, yerleşik GPO'ların tonları nasıl düzenlenemez ve özel GPO'lar nasıl oluşturulacak?
