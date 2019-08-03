---
title: Sorun giderme sorun - kullanıcı dizinde bulunamadı
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 0909edc581c811fdc4683b004e0df0adbac88d1c
ms.sourcegitcommit: 514ced512d0d7fff485b6fbf236cd27d6b4166e0
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/26/2019
ms.locfileid: "35249933"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="d8712-102">Sorun giderme sorun - kullanıcı dizinde bulunamadı</span><span class="sxs-lookup"><span data-stu-id="d8712-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="d8712-103">Kullanıcı hata iletisi "kullanıcı bulunamadı" dizinde alıyorsanız.</span><span class="sxs-lookup"><span data-stu-id="d8712-103">If users are receiving error message "user can't be found" in the directory.</span></span> <span data-ttu-id="d8712-104">Yeniden burada sorun türü kullanıcı dizininde değil deneyin.</span><span class="sxs-lookup"><span data-stu-id="d8712-104">Please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="d8712-105">Bu sorunu gidermek için aşağıdaki adımları tamamlanabilir.</span><span class="sxs-lookup"><span data-stu-id="d8712-105">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="d8712-106">Daha sonra oturum açmak için kullanılan aynı hesabı e-posta daveti olduğu kabul hesabına emin olun.</span><span class="sxs-lookup"><span data-stu-id="d8712-106">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="d8712-107">Kullanıcı daveti kabul etmek ve siteye imzalamak için aynı hesabı kullandığından emin olun.</span><span class="sxs-lookup"><span data-stu-id="d8712-107">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="d8712-108">Daha fazla bilgi için bkz: [diğer adlar için Microsoft hesabınızı yönetmek nasıl</a> Office 365 oturumu yönetmek için](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="d8712-108">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="d8712-109">Kullanıcı hatayı alıyor her site için göz atın.</span><span class="sxs-lookup"><span data-stu-id="d8712-109">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="d8712-110">Eklemek "/ _layouts/15/people.aspx/membershipgroupid=0" (çift tırnak içinde) site URL'SİNİN sonuna.</span><span class="sxs-lookup"><span data-stu-id="d8712-110">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="d8712-111">Örnek: https://_lT _"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="d8712-111">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="d8712-112">Kullanıcı listeden seçin.</span><span class="sxs-lookup"><span data-stu-id="d8712-112">Select the user from the list.</span></span>

- <span data-ttu-id="d8712-113">Şerit'ten **kullanıcı izinlerini Kaldır** ' ı tıklatın.</span><span class="sxs-lookup"><span data-stu-id="d8712-113">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="d8712-114">Yeniden kullanıcı ekleyin ve davet kullanıcıya yeniden gönderin.</span><span class="sxs-lookup"><span data-stu-id="d8712-114">Add back the User and Resend the invite to the user.</span></span>

