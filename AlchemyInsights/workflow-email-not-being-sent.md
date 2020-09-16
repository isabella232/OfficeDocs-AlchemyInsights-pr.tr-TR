---
title: İş akışı e-postası gönderilmiyor
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 7efb8895ac7e2816a2c6055ec3c08d6f7029d39d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47749029"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="6b2f9-102">SharePoint listesi veya kitaplığı için iş akışı e-postası gönderilmiyor</span><span class="sxs-lookup"><span data-stu-id="6b2f9-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="6b2f9-103">İş akışlarından gelen e-posta tüm kullanıcılara veya yalnızca belirli kullanıcılara gönderilmez veya **e-posta iletisinin gönderilemediği hatayı görürsünüz. e-postanın geçerli bir alıcısı olduğundan emin olun**.</span><span class="sxs-lookup"><span data-stu-id="6b2f9-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="6b2f9-104">Kullanıcının söz konusu site koleksiyonu için **tüm insan** izinleri grubunda (Kullanıcı bilgileri listesi) bulunup bulunmadığını denetleyin.</span><span class="sxs-lookup"><span data-stu-id="6b2f9-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="6b2f9-105">Örnek doğrudan URL: https:// <tenant> . SharePoint.com/sites/ <sitename> /_layouts/15/People.aspx? MembershipGroupId = 0</span><span class="sxs-lookup"><span data-stu-id="6b2f9-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="6b2f9-106">Kullanıcı yoksa, kullanıcının sayfada oturum açıldığından emin olun.</span><span class="sxs-lookup"><span data-stu-id="6b2f9-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="6b2f9-107">Bu bir dış kullanıcıysanız, davetinin kabul edilmiş olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="6b2f9-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="6b2f9-108">Kullanıcı izinler grubunda varsa, e-posta adresinin doğru olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="6b2f9-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="6b2f9-109">Kullanıcıların e-posta adresi burada ayarlanmamışsa, bu kullanıcı hesabının SharePoint 'in Kullanıcı profillerinden bu site koleksiyonuna eşitlenmesini zorlayan bir örnek uyarı oluşturun.</span><span class="sxs-lookup"><span data-stu-id="6b2f9-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="6b2f9-110">İş akışlarından gelen e-posta, site koleksiyonu yöneticilerine gönderilir, ancak diğer kullanıcılara değil **http <span>:</span>//_vti_bin/Client.XVC.Sp.Utilities.Utility.SendEmail**.</span><span class="sxs-lookup"><span data-stu-id="6b2f9-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="6b2f9-111">[Bir SharePoint grubuna e-posta gönderdiğinizde erişim engellendi](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups)bölümüne bakın.</span><span class="sxs-lookup"><span data-stu-id="6b2f9-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="6b2f9-112">Ayrıca, **sınırlı erişimli kullanıcı izni kilitleme modu** site koleksiyonu özelliğinin etkin olmadığını doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="6b2f9-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="6b2f9-113">İlgili konular</span><span class="sxs-lookup"><span data-stu-id="6b2f9-113">Related topics</span></span>
<span data-ttu-id="6b2f9-114">SharePoint Online 'da Microsoft akışını denemek mi istiyorsunuz?</span><span class="sxs-lookup"><span data-stu-id="6b2f9-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="6b2f9-115">Akış oluştur</span><span class="sxs-lookup"><span data-stu-id="6b2f9-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="6b2f9-116">SharePoint ve akış</span><span class="sxs-lookup"><span data-stu-id="6b2f9-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


