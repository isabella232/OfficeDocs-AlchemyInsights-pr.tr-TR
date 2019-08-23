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
ms.openlocfilehash: 537b27d06acd17cbb3fe99bcb89e153099e92bb4
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36544883"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="06d26-102">Sorun giderme sorun - kullanıcı dizinde bulunamadı</span><span class="sxs-lookup"><span data-stu-id="06d26-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="06d26-103">Kullanıcı hata iletisi "kullanıcı bulunamadı" dizinde alıyorsanız.</span><span class="sxs-lookup"><span data-stu-id="06d26-103">If users are receiving error message "user can't be found" in the directory.</span></span> <span data-ttu-id="06d26-104">Yeniden burada sorun türü kullanıcı dizininde değil deneyin.</span><span class="sxs-lookup"><span data-stu-id="06d26-104">Please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="06d26-105">Bu sorunu gidermek için aşağıdaki adımları tamamlanabilir.</span><span class="sxs-lookup"><span data-stu-id="06d26-105">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="06d26-106">Daha sonra oturum açmak için kullanılan aynı hesabı e-posta daveti olduğu kabul hesabına emin olun.</span><span class="sxs-lookup"><span data-stu-id="06d26-106">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="06d26-107">Kullanıcı daveti kabul etmek ve siteye imzalamak için aynı hesabı kullandığından emin olun.</span><span class="sxs-lookup"><span data-stu-id="06d26-107">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="06d26-108">Daha fazla bilgi için bkz: [diğer adlar için Microsoft hesabınızı yönetmek nasıl</a> Office 365 oturumu yönetmek için](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="06d26-108">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="06d26-109">Kullanıcı hatayı alıyor her site için göz atın.</span><span class="sxs-lookup"><span data-stu-id="06d26-109">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="06d26-110">Eklemek "/ _layouts/15/people.aspx/membershipgroupid=0" (çift tırnak içinde) site URL'SİNİN sonuna.</span><span class="sxs-lookup"><span data-stu-id="06d26-110">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="06d26-111">Örnek: https://_lT _"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="06d26-111">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="06d26-112">Kullanıcı listeden seçin.</span><span class="sxs-lookup"><span data-stu-id="06d26-112">Select the user from the list.</span></span>

- <span data-ttu-id="06d26-113">Şerit'ten **kullanıcı izinlerini Kaldır** ' ı tıklatın.</span><span class="sxs-lookup"><span data-stu-id="06d26-113">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="06d26-114">Yeniden kullanıcı ekleyin ve davet kullanıcıya yeniden gönderin.</span><span class="sxs-lookup"><span data-stu-id="06d26-114">Add back the User and Resend the invite to the user.</span></span>

