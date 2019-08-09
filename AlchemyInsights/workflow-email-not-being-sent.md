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
ms.openlocfilehash: 49c510668f4c73a71495b89ee9f810d4e7244da3
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270692"
---
# <a name="workflow-email-is-not-being-sent"></a><span data-ttu-id="1f394-102">İş akışı e-posta gönderme</span><span class="sxs-lookup"><span data-stu-id="1f394-102">Workflow email is not being sent</span></span>

1. <span data-ttu-id="1f394-103">Tüm kullanıcıları veya yalnızca belirli kullanıcıların iş akışları gelen e-posta gönderilmez veya gördüğünüz hata **e-posta iletisi gönderilemez. Geçerli bir alıcı e-posta olup olmadığını**.</span><span class="sxs-lookup"><span data-stu-id="1f394-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="1f394-104">Onay grubundaki **Tüm kişilerin** izinleri (kullanıcı bilgileri listesi) bu site koleksiyonu için varsa.</span><span class="sxs-lookup"><span data-stu-id="1f394-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="1f394-105">Örnek doğrudan URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MembershipGroupId = 0</span><span class="sxs-lookup"><span data-stu-id="1f394-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="1f394-106">Kullanıcı yoksa, kullanıcı sayfaya oturum emin olun.</span><span class="sxs-lookup"><span data-stu-id="1f394-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="1f394-107">Harici kullanıcı ise, kendi daveti kabul ettiğinden emin olun.</span><span class="sxs-lookup"><span data-stu-id="1f394-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="1f394-108">Kullanıcı grubu izinleri yoksa e-posta adresinin doğru olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="1f394-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="1f394-109">Kullanıcıların e-posta adresi burada ayarlı değilse, daha sonra eşitleme, kullanıcı hesabının bu site koleksiyonu için olan kullanıcı profilleri SharePoint'ten zorlar, bu kullanıcı için bir örnek uyarıyı oluşturun.</span><span class="sxs-lookup"><span data-stu-id="1f394-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="1f394-110">E-postadan iş akışları site koleksiyonu yöneticileri, ancak diğer kullanıcılara gönderilen ve hata \*\*HTTP Yasak için <spam> <spam> \*\* <spam> <spam>.</span><span class="sxs-lookup"><span data-stu-id="1f394-110">Email from Workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <spam><spam>https://URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**<spam><spam>.</span></span>
 

    <span data-ttu-id="1f394-111">[Gönderilen e-posta grupları, erişim engellendi](https://docs.microsoft.com/sharepoint/support/server-admin/access-denied-when-send-an-email-to-groups)bakın.</span><span class="sxs-lookup"><span data-stu-id="1f394-111">See [Access Denied when sent email to groups](https://docs.microsoft.com/sharepoint/support/server-admin/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="1f394-112">Ayrıca, **sınırlı erişimli kullanıcı izni kilitleme modu** site koleksiyonu özelliği etkin olmadığından emin olun.</span><span class="sxs-lookup"><span data-stu-id="1f394-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="1f394-113">İlgili konular</span><span class="sxs-lookup"><span data-stu-id="1f394-113">Related topics</span></span>
<span data-ttu-id="1f394-114">SharePoint çevrimiçi Microsoft Flow denemek istiyor?</span><span class="sxs-lookup"><span data-stu-id="1f394-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="1f394-115">Akış oluşturma</span><span class="sxs-lookup"><span data-stu-id="1f394-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="1f394-116">SharePoint ve akış</span><span class="sxs-lookup"><span data-stu-id="1f394-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


