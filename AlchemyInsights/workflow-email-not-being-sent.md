---
title: İş akışı e-posta gönderme
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 783bf0a5721aa5db7088432c71e06cac6dc90513
ms.sourcegitcommit: 407f6c1e82f1a0be5cf53301fbf03cd25dcbf0ee
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/02/2019
ms.locfileid: "36059623"
---
# <a name="workflow-email-is-not-being-sent"></a><span data-ttu-id="18560-102">İş akışı e-posta gönderme</span><span class="sxs-lookup"><span data-stu-id="18560-102">Workflow email is not being sent</span></span>

1. <span data-ttu-id="18560-103">Tüm kullanıcıları veya yalnızca belirli kullanıcıların iş akışları gelen e-posta gönderilmez veya gördüğünüz hata **e-posta iletisi gönderilemez. Geçerli bir alıcı e-posta olup olmadığını**.</span><span class="sxs-lookup"><span data-stu-id="18560-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

<span data-ttu-id="18560-104">Onay grubundaki **Tüm kişilerin** izinleri (kullanıcı bilgileri listesi) bu site koleksiyonu için varsa.</span><span class="sxs-lookup"><span data-stu-id="18560-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="18560-105">Örnek doğrudan URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MembershipGroupId = 0</span><span class="sxs-lookup"><span data-stu-id="18560-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

- <span data-ttu-id="18560-106">Kullanıcı yoksa, kullanıcı sayfaya oturum emin olun.</span><span class="sxs-lookup"><span data-stu-id="18560-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
- <span data-ttu-id="18560-107">Harici kullanıcı ise, kendi daveti kabul ettiğinden emin olun.</span><span class="sxs-lookup"><span data-stu-id="18560-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
- <span data-ttu-id="18560-108">Kullanıcı grubu izinleri yoksa e-posta adresinin doğru olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="18560-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
- <span data-ttu-id="18560-109">Kullanıcıların e-posta adresi burada ayarlı değilse, daha sonra eşitleme, kullanıcı hesabının bu site koleksiyonu için olan kullanıcı profilleri SharePoint'ten zorlar, bu kullanıcı için bir örnek uyarıyı oluşturun.</span><span class="sxs-lookup"><span data-stu-id="18560-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="18560-110">E-postadan iş akışları site koleksiyonu yöneticileri, ancak diğer kullanıcılara gönderilen ve hata \*\*HTTP Yasak için <spam> <spam> \*\* <spam> <spam>.</span><span class="sxs-lookup"><span data-stu-id="18560-110">Email from Workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <spam><spam>https://URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**<spam><spam>.</span></span>
 

<span data-ttu-id="18560-111">[Gönderilen e-posta grupları, erişim engellendi](https://docs.microsoft.com/sharepoint/support/server-admin/access-denied-when-send-an-email-to-groups)bakın.</span><span class="sxs-lookup"><span data-stu-id="18560-111">See [Access Denied when sent email to groups](https://docs.microsoft.com/sharepoint/support/server-admin/access-denied-when-send-an-email-to-groups).</span></span>

<span data-ttu-id="18560-112">Ayrıca, **sınırlı erişimli kullanıcı izni kilitleme modu** site koleksiyonu özelliği etkin olmadığından emin olun.</span><span class="sxs-lookup"><span data-stu-id="18560-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>

## <a name="related-topics"></a><span data-ttu-id="18560-113">İlgili konular</span><span class="sxs-lookup"><span data-stu-id="18560-113">Related topics</span></span>
- [<span data-ttu-id="18560-114">Akış oluşturma</span><span class="sxs-lookup"><span data-stu-id="18560-114">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="18560-115">SharePoint ve akış</span><span class="sxs-lookup"><span data-stu-id="18560-115">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


