---
title: Güvenlik gruplarında sorun
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
- "8252"
- "9004397"
ms.openlocfilehash: 1198b79c3301bd2752a7385a6ba6746c8f0c2b5b
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177636"
---
# <a name="issue-with-security-groups"></a><span data-ttu-id="52d80-102">Güvenlik gruplarında sorun</span><span class="sxs-lookup"><span data-stu-id="52d80-102">Issue with security groups</span></span>

<span data-ttu-id="52d80-103">**Ağ Hatası AADDS104 alıyorsanız**</span><span class="sxs-lookup"><span data-stu-id="52d80-103">**If you are getting Network Error AADDS104**</span></span>

<span data-ttu-id="52d80-104">Azure Active Directory Etki Alanı Hizmetleri'nin (AD DS) ağ hatalarının en yaygın nedeni geçersiz ağ güvenlik grubu kurallarıdır.</span><span class="sxs-lookup"><span data-stu-id="52d80-104">Invalid network security group rules are the most common cause of network errors for Azure Active Directory Domain Services (AD DS).</span></span> <span data-ttu-id="52d80-105">Sanal ağın ağ güvenlik grubunun belirli bağlantı noktalarına ve protokollere erişime izin vermesi gerekir.</span><span class="sxs-lookup"><span data-stu-id="52d80-105">The network security group for the virtual network must allow access to specific ports and protocols.</span></span> <span data-ttu-id="52d80-106">Bu bağlantı noktaları engellenmişse, Azure platformu yönetilen etki alanını izleyamaz veya güncelleştiramaz.</span><span class="sxs-lookup"><span data-stu-id="52d80-106">If these ports are blocked, the Azure platform can't monitor or update the managed domain.</span></span> <span data-ttu-id="52d80-107">Azure AD ile Azure AD DS arasındaki eşitleme de etkiyi etkiler.</span><span class="sxs-lookup"><span data-stu-id="52d80-107">The synchronization between the Azure AD and Azure AD DS is also impacted.</span></span> <span data-ttu-id="52d80-108">Hizmette kesinti olmasını önlemek için varsayılan bağlantı noktalarını açık tutabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="52d80-108">Ensure you keep the default ports open to avoid interruption in service.</span></span>

<span data-ttu-id="52d80-109">Ağ güvenliği grubu yapılandırma sorunlarının yaygın uyarılarını anlamak ve çözmek için bkz. Güvenlik Grupları [Ekleme ve Doğrulama.](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules)</span><span class="sxs-lookup"><span data-stu-id="52d80-109">To understand and to resolve common alerts for network security group configuration issues, see [Add and Verify Security Groups](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules).</span></span>
