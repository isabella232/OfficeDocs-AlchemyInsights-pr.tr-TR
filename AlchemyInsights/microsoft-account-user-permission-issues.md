---
title: Sorun giderme sorunu - Kullanıcı dizinde bulunamadı
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 3b863c5e9962dd29ca2ed41d113041d74830f615
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43702758"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="ef0e4-102">Sorun giderme sorunu - Kullanıcı dizinde bulunamadı</span><span class="sxs-lookup"><span data-stu-id="ef0e4-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="ef0e4-103">Kullanıcılar dizinde "kullanıcı bulunamıyor" hata iletisi alıyorsa, lütfen Sorun Türü Kullanıcı'nın dizinde olmadığı yerlerde yeniden deneyin.</span><span class="sxs-lookup"><span data-stu-id="ef0e4-103">If users are receiving error message "user can't be found" in the directory, please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="ef0e4-104">Sorunu gidermek için aşağıdaki adımlar tamamlanabilir.</span><span class="sxs-lookup"><span data-stu-id="ef0e4-104">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="ef0e4-105">E-posta davetini kabul eden hesabın daha sonra oturum açmada kullanılan hesapla aynı olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="ef0e4-105">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="ef0e4-106">Daveti kabul etmek ve sitede oturum açmak için kullanıcının aynı hesabı kullandığından emin olun.</span><span class="sxs-lookup"><span data-stu-id="ef0e4-106">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="ef0e4-107">Daha fazla bilgi için, [Microsoft 365</a> oturumunu yönetmek için Microsoft hesabınıziçin takma adları nasıl yönetebilirsiniz'](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases)e bakın.</span><span class="sxs-lookup"><span data-stu-id="ef0e4-107">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Microsoft 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="ef0e4-108">Kullanıcının hata aldığı her siteye göz atın.</span><span class="sxs-lookup"><span data-stu-id="ef0e4-108">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="ef0e4-109">Site URL'sinin sonuna "/_layouts/15/people.aspx/membershipgroupid=0" (çift tırnak içinde) ekleyin.</span><span class="sxs-lookup"><span data-stu-id="ef0e4-109">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="ef0e4-110">Örnek: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="ef0e4-110">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="ef0e4-111">Listeden kullanıcıyı seçin.</span><span class="sxs-lookup"><span data-stu-id="ef0e4-111">Select the user from the list.</span></span>

- <span data-ttu-id="ef0e4-112">**Kullanıcı İzinlerini** Şeritten Kaldır'ı tıklatın.</span><span class="sxs-lookup"><span data-stu-id="ef0e4-112">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="ef0e4-113">Kullanıcıyı geri ekleyin ve daveti kullanıcıya yeniden gönderin.</span><span class="sxs-lookup"><span data-stu-id="ef0e4-113">Add back the User and Resend the invite to the user.</span></span>

