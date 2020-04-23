---
title: İş akışı e-postası gönderiliyor
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 391d3a2dcc2676a405065115f375c802d2492119
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766153"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="3280d-102">İş akışı e-postası SharePoint listesi veya kitaplık için göndermiyor</span><span class="sxs-lookup"><span data-stu-id="3280d-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="3280d-103">İş akışlarından gelen e-postalar tüm kullanıcılara veya yalnızca belirli kullanıcılara gönderilmez veya **e-posta iletisinin gönderilemeyeceği hatayı görürsünüz. E-postanın geçerli bir alıcıya sahip olduğundan emin olun.**</span><span class="sxs-lookup"><span data-stu-id="3280d-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="3280d-104">Kullanıcının bu site koleksiyonu için **Tüm Kişiler** izinler grubunda (kullanıcı bilgileri listesi) bulunun.</span><span class="sxs-lookup"><span data-stu-id="3280d-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="3280d-105">Örnek doğrudan URL:<tenant><sitename>https:// .sharepoint.com/sites/ /_layouts/15/people.aspx? ÜyelikGroupId=0</span><span class="sxs-lookup"><span data-stu-id="3280d-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="3280d-106">Kullanıcı yoksa, kullanıcının sayfada oturum açmış olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="3280d-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="3280d-107">Harici bir kullanıcıysa, davetlerinin kabul edildiğinden emin olun.</span><span class="sxs-lookup"><span data-stu-id="3280d-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="3280d-108">Kullanıcı izinler grubunda varsa, e-posta adresinin doğru olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="3280d-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="3280d-109">Kullanıcıların e-posta adresi burada ayarlanmıyorsa, o kullanıcı için sharepoint kullanıcı profillerinden bu site koleksiyonuna kullanıcı hesabının eşitlanmasını zorlayan bir örnek uyarı oluşturun.</span><span class="sxs-lookup"><span data-stu-id="3280d-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="3280d-110">İş akışlarından gelen e-postalar site koleksiyonu yöneticilerine gönderilir, ancak diğer kullanıcılara gönderilmez ve **http forbidden to https hatasını görürsünüz: //URL/_vti_bin/client.xvc.sp.utility.utility.SendEmail <span>https:</span>**.</span><span class="sxs-lookup"><span data-stu-id="3280d-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="3280d-111">Bir [SharePoint grubuna e-posta gönderdiğinde Erişim Reddedildi'yi](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups)görün.</span><span class="sxs-lookup"><span data-stu-id="3280d-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="3280d-112">Ayrıca, Sınırlı **erişimli kullanıcı izni kilitleme modu** site koleksiyonu özelliğinin etkin olmadığını doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="3280d-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="3280d-113">İlgili konular</span><span class="sxs-lookup"><span data-stu-id="3280d-113">Related topics</span></span>
<span data-ttu-id="3280d-114">SharePoint Online'da Microsoft Flow'u denemek ister misiniz?</span><span class="sxs-lookup"><span data-stu-id="3280d-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="3280d-115">Akış Oluştur</span><span class="sxs-lookup"><span data-stu-id="3280d-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="3280d-116">SharePoint ve Akış</span><span class="sxs-lookup"><span data-stu-id="3280d-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


