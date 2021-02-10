---
title: Etki alanı hizmeti için parola karması eşitlemesi
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8248"
- "9004400"
- "8249"
- "9003245"
ms.openlocfilehash: 7f138837b720926c5b687285a105eb0417ca5b39
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177618"
---
# <a name="password-hash-synchronization-for-domain-service"></a><span data-ttu-id="86bda-102">Etki alanı hizmeti için parola karması eşitlemesi</span><span class="sxs-lookup"><span data-stu-id="86bda-102">Password hash synchronization for domain service</span></span>

<span data-ttu-id="86bda-103">**Azure AD DS örneğiniz parola karma eşitlemesini etkinleştirmenizi istendiğinde**</span><span class="sxs-lookup"><span data-stu-id="86bda-103">**If your Azure AD DS instance is prompting you to enable password hash synchronization**</span></span>

<span data-ttu-id="86bda-104">Karma bir ortamı, şirket içi Azure Active Directory Etki Alanı Hizmetleri (AD DS) ortamından eşitleen kullanıcılarla çalıştırıyorsanız, bir senaryoyla karşılaşırsınız.</span><span class="sxs-lookup"><span data-stu-id="86bda-104">You encounter a scenario in which you are running a hybrid environment with users synchronizing from an on-premises Azure Active Directory Domain Services (AD DS) environment.</span></span> <span data-ttu-id="86bda-105">Şirket içi AD DS'den Azure AD kiracınıza parola karma eşitlemesi olmasına rağmen bu senaryoyla karşılaşıldı.</span><span class="sxs-lookup"><span data-stu-id="86bda-105">This scenario is encountered despite you having password hash synchronization from the on-premises AD DS to your Azure AD tenant.</span></span>

<span data-ttu-id="86bda-106">**Neden**</span><span class="sxs-lookup"><span data-stu-id="86bda-106">**Cause**</span></span>

<span data-ttu-id="86bda-107">Bunun nedeni Azure AD Connect'in varsayılan olarak Azure AD DS için gereken eski Yeni Teknoloji LAN Manager (NTLM) ve Kerberos parola karmalarını eşitlememasıdır.</span><span class="sxs-lookup"><span data-stu-id="86bda-107">This is happening because Azure AD Connect by default does not synchronize legacy New Technology LAN Manager (NTLM) and Kerberos password hashes that are needed for Azure AD DS.</span></span>

<span data-ttu-id="86bda-108">**Geçici Çözüm**</span><span class="sxs-lookup"><span data-stu-id="86bda-108">**Workaround**</span></span> 

<span data-ttu-id="86bda-109">NTLM ve Kerberos kimlik doğrulaması için gereken parola karmalarını eşitlemek için Azure AD Connect'i yapılandırmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="86bda-109">You would need to configure Azure AD Connect to synchronize those password hashes required for NTLM and Kerberos authentication.</span></span>

<span data-ttu-id="86bda-110">Azure AD Connect yapılandırıldığında, şirket içi hesap oluşturma veya parola değiştirme olayı da eski parola karmalarını Azure AD'ye eşitler.</span><span class="sxs-lookup"><span data-stu-id="86bda-110">After Azure AD Connect is configured, an on-premises account creation or password change event also then synchronizes the legacy password hashes to Azure AD.</span></span> <span data-ttu-id="86bda-111">Bu işlem [hakkında](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) daha fazla bilgi ve Azure AD DS karma ortamlarında parola eşitlemesini etkinleştirme hakkında yol gösterici bilgiler için lütfen buraya bakın.</span><span class="sxs-lookup"><span data-stu-id="86bda-111">Please see [here](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) for more information on this and for guidance on how to enable password synchronization in Azure AD DS hybrid environments.</span></span>