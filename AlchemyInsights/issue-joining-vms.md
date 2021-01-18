---
title: VM 'Lere katılma sorunu
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7924"
- "9004395"
ms.openlocfilehash: 77a889f05d6c4e7b19a1e0a66a99ffc0565c69d8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885658"
---
# <a name="issue-joining-vms"></a><span data-ttu-id="9df5d-102">VM 'Lere katılma sorunu</span><span class="sxs-lookup"><span data-stu-id="9df5d-102">Issue joining VMs</span></span>

<span data-ttu-id="9df5d-103">VM 'Lere katılmaya çalışırken oluşan sorunları çözmek için aşağıdaki adımları uygulayın:</span><span class="sxs-lookup"><span data-stu-id="9df5d-103">To resolve issues that occur while trying to join VMs, perform the following steps:</span></span>

1. <span data-ttu-id="9df5d-104">**SAMAccountName** biçimi yerine **UPN** biçimini (örneğin, ' joeuser@contoso.com ') kullanarak oturum açmayı deneyin (' contoso\joeuser ').</span><span class="sxs-lookup"><span data-stu-id="9df5d-104">Try to sign in using the **UPN** format (for example, 'joeuser@contoso.com') instead of the **SAMAccountName** format ('CONTOSO\joeuser').</span></span>
2. <span data-ttu-id="9df5d-105">*Başlarken* kılavuzunda anlatılan adımlara uygun olarak parola eşitlemesini etkinleştirdiğinizden emin olun.</span><span class="sxs-lookup"><span data-stu-id="9df5d-105">Ensure that you have enabled password synchronization in accordance with the steps outlined in the *Getting Started* guide.</span></span>
3. <span data-ttu-id="9df5d-106">Etkilenen Kullanıcı hesabının Azure AD kiracısında dış hesap olmadığından emin olun.</span><span class="sxs-lookup"><span data-stu-id="9df5d-106">Ensure that the affected user account is not an external account in the Azure AD tenant.</span></span> <span data-ttu-id="9df5d-107">Azure AD etki alanı Hizmetleri bu kullanıcı hesaplarının kimlik bilgilerini içermediğinden, dış kullanıcılar yönetilen etki alanında oturum açamaz.</span><span class="sxs-lookup"><span data-stu-id="9df5d-107">External users cannot sign in to the managed domain since Azure AD Domain Services does not have credentials for such user accounts.</span></span>
4. <span data-ttu-id="9df5d-108">Etkilenen Kullanıcı hesabı yalnızca bulut Kullanıcı hesabandır, Azure AD etki alanı Hizmetleri 'ni etkinleştirdikten sonra kullanıcıların parolasını değiştirmeyeceğinden emin olun.</span><span class="sxs-lookup"><span data-stu-id="9df5d-108">If the affected user account is a cloud-only user account, ensure that users have changed their password after you enabled Azure AD Domain Services.</span></span> <span data-ttu-id="9df5d-109">Bu adım, Azure AD etki alanı Hizmetleri için gereken kimlik bilgilerinin üretilmesine neden olur.</span><span class="sxs-lookup"><span data-stu-id="9df5d-109">This step causes the credential hashes required for Azure AD Domain Services to be generated.</span></span>
5. <span data-ttu-id="9df5d-110">Etkilenen Kullanıcı hesapları şirket içi bir dizinden eşitleniyorsa, önerilen Azure AD Connect sürümünün tam eşitleme yapacak şekilde yapılandırılmış olduğunu doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="9df5d-110">If the affected user accounts are synchronized from an on-premises directory, verify that the recommended release of Azure AD Connect has been configured to perform a full synchronization.</span></span>
6. <span data-ttu-id="9df5d-111">Adım 4 ' ü onayladıktan sonra sorun devam ediyorsa, eşitleme makinenizden aşağıdaki komutları yürütün:</span><span class="sxs-lookup"><span data-stu-id="9df5d-111">If issues persists after confirming Step 4, execute the following commands from your sync machine:</span></span>
 
     `"net stop 'Microsoft Azure AD Sync'"`  
     <span data-ttu-id="9df5d-112">`"net start 'Microsoft Azure AD Sync'"`.</span><span class="sxs-lookup"><span data-stu-id="9df5d-112">`"net start 'Microsoft Azure AD Sync'"`.</span></span>