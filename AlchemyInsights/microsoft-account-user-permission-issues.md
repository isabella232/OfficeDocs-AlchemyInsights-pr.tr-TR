---
title: Sorun giderme sorunu - Kullanıcı dizinde bulunamadı
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 81b9dafe8e27e5f73fe232c51ff56fed3fec29b4
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36754212"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="e55d5-102">Sorun giderme sorunu - Kullanıcı dizinde bulunamadı</span><span class="sxs-lookup"><span data-stu-id="e55d5-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="e55d5-103">Kullanıcılar dizinde "kullanıcı bulunamıyor" hata iletisi alıyorsanız.</span><span class="sxs-lookup"><span data-stu-id="e55d5-103">If users are receiving error message "user can't be found" in the directory.</span></span> <span data-ttu-id="e55d5-104">Lütfen Sorun Türü Kullanıcı dizininde olmadığı yerde yeniden deneyin.</span><span class="sxs-lookup"><span data-stu-id="e55d5-104">Please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="e55d5-105">Sorunu gidermek için aşağıdaki adımlar tamamlanabilir.</span><span class="sxs-lookup"><span data-stu-id="e55d5-105">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="e55d5-106">E-posta davetini kabul eden hesabın daha sonra oturum açmada kullanılan hesapla aynı olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="e55d5-106">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="e55d5-107">Daveti kabul etmek ve sitede oturum açmak için kullanıcının aynı hesabı kullandığından emin olun.</span><span class="sxs-lookup"><span data-stu-id="e55d5-107">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="e55d5-108">Daha fazla bilgi için, [Office 365</a> oturumunu yönetmek için Microsoft hesabınıza takma](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases)adlar nasıl yönetilir' e bakın.</span><span class="sxs-lookup"><span data-stu-id="e55d5-108">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="e55d5-109">Kullanıcının hata aldığı her siteye göz atın.</span><span class="sxs-lookup"><span data-stu-id="e55d5-109">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="e55d5-110">Site URL'sinin sonuna "/_layouts/15/people.aspx/membershipgroupid=0" (çift tırnak içinde) ekleyin.</span><span class="sxs-lookup"><span data-stu-id="e55d5-110">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="e55d5-111">Örnek: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="e55d5-111">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="e55d5-112">Listeden kullanıcıyı seçin.</span><span class="sxs-lookup"><span data-stu-id="e55d5-112">Select the user from the list.</span></span>

- <span data-ttu-id="e55d5-113">**Kullanıcı İzinlerini** Şeritten Kaldır'ı tıklatın.</span><span class="sxs-lookup"><span data-stu-id="e55d5-113">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="e55d5-114">Kullanıcıyı geri ekleyin ve daveti kullanıcıya yeniden gönderin.</span><span class="sxs-lookup"><span data-stu-id="e55d5-114">Add back the User and Resend the invite to the user.</span></span>

