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
ms.openlocfilehash: 6f9e164713ce36023de954d45031fd4414780e174bf5c7741c4aec274a65b32e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54067860"
---
# <a name="gpo-deployment"></a>GPO Dağıtımı

Ayarlar Alanı Hizmetleri'Azure Active Directory (Azure AD DS) kullanan kullanıcı ve bilgisayar nesneleri için kimlik bilgileri çoğunlukla Grup İlkesi Nesneleri (GPOS) kullanılarak yönetilir. Azure AD DS, AADDC Kullanıcıları ve AADDC Bilgisayarlar kapsayıcıları için yerleşik GPOS içerir. Ortamınız için gereken grup ilkesi yapılandırmak için bu yerleşik GPOS'ları özelleştirebilirsiniz. Azure AD DC yönetici grubunun üyelerinin Azure AD DS etki alanında grup ilkesi yönetim ayrıcalıkları vardır ve özel GPOS ve kuruluş birimleri (OU'lar) da oluşturabilirler. Grup ilkesi nedir ve nasıl çalışır? hakkında daha fazla bilgi için bkz. Grup [İlkesine Genel Bakış.](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11))

Karma bir ortamda, şirket içi AD DS ortamında yapılandırılan grup ilkeleri Azure AD DS ile eşitlenmez. Azure AD DS'de kullanıcılara veya bilgisayarlara yönelik yapılandırma ayarlarını tanımlamak için varsayılan GPOS'lardan birini düzenleyin veya özel bir GPO oluşturun.

Bu makalede [Grup İlkesini](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) Yönet, Grup İlkesi Yönetim araçlarını yükleme, yerleşik GPOS'ları düzenleme ve özel GPOS oluşturma hakkında bilgi sağlar.
