---
title: Grup ilkesi
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8303"
- "9003234"
ms.openlocfilehash: a829a78bbe947300b6dabb9fdb36088c17809742
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256909"
---
# <a name="group-policy"></a>Grup ilkesi

Azure Active Directory Etki Alanı Hizmetleri'nin (Azure AD DS) kullanıcı ve bilgisayar nesnelerinin ayarları çoğunlukla Grup İlkesi Nesneleri (GPOs) kullanılarak yönetilir. Azure AD DS, AADDC Kullanıcıları ve AADDC Bilgisayarlar kapsayıcıları için yerleşik GPO'lar içerir. Bu yerleşik GPO'ları, ortamınız için gereken grup ilkesi yapılandıracak şekilde özelleştirebilirsiniz. Azure AD DC yönetici grubunun üyeleri, Azure AD DS etki alanında grup ilkesi yönetim ayrıcalıklarına sahip olur ve özel GPOs ve kuruluş birimleri de (OU) oluşturabilir. Grup ilkesi nedir ve nasıl çalışır hakkında daha fazla bilgi için, Grup İlkesine [genel bakış bilgilerine bakın.](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11))

Karma bir ortamda, şirket içi AD DS ortamında yapılandırılan grup ilkeleri Azure AD DS ile eşitlenmez. Azure AD DS'de kullanıcılara veya bilgisayarlara yönelik yapılandırma ayarlarını tanımlamak için, varsayılan GPO'lardan birini düzenleyin veya özel bir GPO oluşturun.

Bu makalede [Grup](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) İlkesini Yönet, Grup İlkesi Yönetim araçlarının nasıl yüklenemez, yerleşik GPOs'ların tonları nasıl düzenlenemez ve özel GPO'lar nasıl oluşturulacak?



