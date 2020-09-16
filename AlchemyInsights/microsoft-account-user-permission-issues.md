---
title: Sorun giderme-Kullanıcı dizininde bulunamadı
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 512494a69ab274af00962cb9777a3479b4200fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725427"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="40eee-102">Sorun giderme-Kullanıcı dizininde bulunamadı</span><span class="sxs-lookup"><span data-stu-id="40eee-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="40eee-103">Kullanıcılar, dizinde "Kullanıcı bulunamıyor" hata iletisi alıyorsa, lütfen sorun türünün Kullanıcı dizininde olmadığı durumlarda yeniden deneyin.</span><span class="sxs-lookup"><span data-stu-id="40eee-103">If users are receiving error message "user can't be found" in the directory, please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="40eee-104">Sorunu gidermek için aşağıdaki adımlar tamamlanabilir.</span><span class="sxs-lookup"><span data-stu-id="40eee-104">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="40eee-105">E-posta davetini kabul eden hesabın, daha sonra oturum açmak için kullanılan hesapla aynı olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="40eee-105">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="40eee-106">Kullanıcının daveti kabul edip sitede oturum açarken aynı hesabı kullanmasını sağlayın.</span><span class="sxs-lookup"><span data-stu-id="40eee-106">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="40eee-107">Daha fazla bilgi için Microsoft [hesabınızın diğer adlarını nasıl yöneteceğinizi </a> Microsoft 365 oturum açmayı yönetmeye](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases)bakın.</span><span class="sxs-lookup"><span data-stu-id="40eee-107">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Microsoft 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="40eee-108">Kullanıcının hatayı aldığı her siteye göz atın.</span><span class="sxs-lookup"><span data-stu-id="40eee-108">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="40eee-109">"/_Layouts/15/People.aspx/membershipgroupid = 0" (çift tırnak içinde) site URL 'sinin sonuna ekleyin.</span><span class="sxs-lookup"><span data-stu-id="40eee-109">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="40eee-110">Örnek: https://< "contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="40eee-110">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="40eee-111">Listeden kullanıcıyı seçin.</span><span class="sxs-lookup"><span data-stu-id="40eee-111">Select the user from the list.</span></span>

- <span data-ttu-id="40eee-112">Şeritteki **Kullanıcı Izinlerini kaldır** 'ı tıklatın.</span><span class="sxs-lookup"><span data-stu-id="40eee-112">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="40eee-113">Kullanıcıyı geri ekleyin ve daveti kullanıcıya yeniden gönderin.</span><span class="sxs-lookup"><span data-stu-id="40eee-113">Add back the User and Resend the invite to the user.</span></span>

