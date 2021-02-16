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
# <a name="group-policy"></a><span data-ttu-id="d3014-102">Grup ilkesi</span><span class="sxs-lookup"><span data-stu-id="d3014-102">Group policy</span></span>

<span data-ttu-id="d3014-103">Azure Active Directory Etki Alanı Hizmetleri'nin (Azure AD DS) kullanıcı ve bilgisayar nesnelerinin ayarları çoğunlukla Grup İlkesi Nesneleri (GPOs) kullanılarak yönetilir.</span><span class="sxs-lookup"><span data-stu-id="d3014-103">Settings for user and computer objects in Azure Active Directory Domain Services (Azure AD DS) are often managed using Group Policy Objects (GPOs).</span></span> <span data-ttu-id="d3014-104">Azure AD DS, AADDC Kullanıcıları ve AADDC Bilgisayarlar kapsayıcıları için yerleşik GPO'lar içerir.</span><span class="sxs-lookup"><span data-stu-id="d3014-104">Azure AD DS includes built-in GPOs for the AADDC Users and AADDC Computers containers.</span></span> <span data-ttu-id="d3014-105">Bu yerleşik GPO'ları, ortamınız için gereken grup ilkesi yapılandıracak şekilde özelleştirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="d3014-105">You can customize these built-in GPOs to configure group policy as needed for your environment.</span></span> <span data-ttu-id="d3014-106">Azure AD DC yönetici grubunun üyeleri, Azure AD DS etki alanında grup ilkesi yönetim ayrıcalıklarına sahip olur ve özel GPOs ve kuruluş birimleri de (OU) oluşturabilir.</span><span class="sxs-lookup"><span data-stu-id="d3014-106">Members of the Azure AD DC administrators group have group policy administration privileges in the Azure AD DS domain, and can also create custom GPOs and organizational units (OUs).</span></span> <span data-ttu-id="d3014-107">Grup ilkesi nedir ve nasıl çalışır hakkında daha fazla bilgi için, Grup İlkesine [genel bakış bilgilerine bakın.](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11))</span><span class="sxs-lookup"><span data-stu-id="d3014-107">For more information on what group policy is and how it works, see [Group Policy overview](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).</span></span>

<span data-ttu-id="d3014-108">Karma bir ortamda, şirket içi AD DS ortamında yapılandırılan grup ilkeleri Azure AD DS ile eşitlenmez.</span><span class="sxs-lookup"><span data-stu-id="d3014-108">In a hybrid environment, group policies configured in an on-premises AD DS environment aren't synchronized to Azure AD DS.</span></span> <span data-ttu-id="d3014-109">Azure AD DS'de kullanıcılara veya bilgisayarlara yönelik yapılandırma ayarlarını tanımlamak için, varsayılan GPO'lardan birini düzenleyin veya özel bir GPO oluşturun.</span><span class="sxs-lookup"><span data-stu-id="d3014-109">To define configuration settings for users or computers in Azure AD DS, edit one of the default GPOs or create a custom GPO.</span></span>

<span data-ttu-id="d3014-110">Bu makalede [Grup](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) İlkesini Yönet, Grup İlkesi Yönetim araçlarının nasıl yüklenemez, yerleşik GPOs'ların tonları nasıl düzenlenemez ve özel GPO'lar nasıl oluşturulacak?</span><span class="sxs-lookup"><span data-stu-id="d3014-110">This article [Manage Group Policy](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) shows you how to install the Group Policy Management tools, how ton edit the built-in GPOs, and how to create custom GPOs.</span></span>



