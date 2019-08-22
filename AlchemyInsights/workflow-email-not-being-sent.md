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
ms.openlocfilehash: 261fe1b1bc815dd4ad568051cfefad1e214b957e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36530911"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="395fd-102">İş akışı e-posta bir SharePoint listesi veya kitaplığı için gönderiliyor.</span><span class="sxs-lookup"><span data-stu-id="395fd-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="395fd-103">Tüm kullanıcıları veya yalnızca belirli kullanıcıların iş akışları gelen e-posta gönderilmez veya gördüğünüz hata **e-posta iletisi gönderilemez. Geçerli bir alıcı e-posta olup olmadığını**.</span><span class="sxs-lookup"><span data-stu-id="395fd-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="395fd-104">Onay grubundaki **Tüm kişilerin** izinleri (kullanıcı bilgileri listesi) bu site koleksiyonu için varsa.</span><span class="sxs-lookup"><span data-stu-id="395fd-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="395fd-105">Örnek doğrudan URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MembershipGroupId = 0</span><span class="sxs-lookup"><span data-stu-id="395fd-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="395fd-106">Kullanıcı yoksa, kullanıcı sayfaya oturum emin olun.</span><span class="sxs-lookup"><span data-stu-id="395fd-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="395fd-107">Harici kullanıcı ise, kendi daveti kabul ettiğinden emin olun.</span><span class="sxs-lookup"><span data-stu-id="395fd-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="395fd-108">Kullanıcı grubu izinleri yoksa e-posta adresinin doğru olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="395fd-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="395fd-109">Kullanıcıların e-posta adresi burada ayarlı değilse, daha sonra eşitleme, kullanıcı hesabının bu site koleksiyonu için olan kullanıcı profilleri SharePoint'ten zorlar, bu kullanıcı için bir örnek uyarıyı oluşturun.</span><span class="sxs-lookup"><span data-stu-id="395fd-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="395fd-110">E-postadan iş akışları site koleksiyonu yöneticileri, ancak diğer kullanıcılara gönderilen ve hata **için HTTP Yasak <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span><span class="sxs-lookup"><span data-stu-id="395fd-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="395fd-111">[SharePoint grubuna bir e-posta gönderdiğinizde, erişim engellendi](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups)bakın.</span><span class="sxs-lookup"><span data-stu-id="395fd-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="395fd-112">Ayrıca, **sınırlı erişimli kullanıcı izni kilitleme modu** site koleksiyonu özelliği etkin olmadığından emin olun.</span><span class="sxs-lookup"><span data-stu-id="395fd-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="395fd-113">İlgili konular</span><span class="sxs-lookup"><span data-stu-id="395fd-113">Related topics</span></span>
<span data-ttu-id="395fd-114">SharePoint çevrimiçi Microsoft Flow denemek istiyor?</span><span class="sxs-lookup"><span data-stu-id="395fd-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="395fd-115">Akış oluşturma</span><span class="sxs-lookup"><span data-stu-id="395fd-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="395fd-116">SharePoint ve akış</span><span class="sxs-lookup"><span data-stu-id="395fd-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


