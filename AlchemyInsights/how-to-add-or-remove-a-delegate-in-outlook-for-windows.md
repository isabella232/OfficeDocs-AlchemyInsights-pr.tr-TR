---
title: Windows için Outlook 'ta temsilci ekleme veya kaldırma
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800004"
- "7334"
ms.openlocfilehash: fcbd6082c104f0e1bca022a23cbbeb6e3363a6c5
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573809"
---
# <a name="how-to-add-or-remove-a-delegate-in-outlook-for-windows"></a><span data-ttu-id="0baf9-102">Windows için Outlook 'ta temsilci ekleme veya kaldırma</span><span class="sxs-lookup"><span data-stu-id="0baf9-102">How to add or remove a Delegate in Outlook for Windows</span></span>

<span data-ttu-id="0baf9-103">Windows için Outlook 'ta temsilci eklemek için:</span><span class="sxs-lookup"><span data-stu-id="0baf9-103">To add a Delegate in Outlook for Windows:</span></span> 

1. <span data-ttu-id="0baf9-104">**Dosya** sekmesini ve ardından **Hesap ayarları**'nı tıklatın ve sonra da **temsilci erişimi**'ni seçin.</span><span class="sxs-lookup"><span data-stu-id="0baf9-104">Click on the **File** tab followed by **Account Settings**, and then choose **Delegate Access**.</span></span>
2. <span data-ttu-id="0baf9-105">**Ekle**'ye tıklayın.</span><span class="sxs-lookup"><span data-stu-id="0baf9-105">Click on **Add**.</span></span> <span data-ttu-id="0baf9-106">**Ekle** görünmüyorsa, Outlook ve Exchange arasında etkin bir bağlantı bulunmayabilir.</span><span class="sxs-lookup"><span data-stu-id="0baf9-106">If **Add** doesn’t appear, an active connection might not exist between Outlook and Exchange.</span></span> <span data-ttu-id="0baf9-107">Outlook durum çubuğunda bağlantı durumu görüntülenir.</span><span class="sxs-lookup"><span data-stu-id="0baf9-107">The Outlook status bar displays the connection status.</span></span>
3. <span data-ttu-id="0baf9-108">Temsilciniz olarak atamak istediğiniz kişinin adını yazın veya arama sonuçları listesinde adı bulup seçin.</span><span class="sxs-lookup"><span data-stu-id="0baf9-108">Type the name of the person you want to designate as your delegate, or search and choose the name in the search results list.</span></span>

    > [!NOTE]
    > <span data-ttu-id="0baf9-109">Temsilcinin, kuruluşunuzun Exchange genel adres listesindeki (GAL) bir kişi olması gerekir.</span><span class="sxs-lookup"><span data-stu-id="0baf9-109">The delegate must be a person in your organization's Exchange Global Address List (GAL).</span></span>
4. <span data-ttu-id="0baf9-110">**Ekle** 'ye tıklayın ve ardından **Tamam 'a** tıklayın.</span><span class="sxs-lookup"><span data-stu-id="0baf9-110">Click on **Add** followed by **OK**.</span></span>
5. <span data-ttu-id="0baf9-111">**Temsilci izinleri** iletişim kutusunda varsayılan izin ayarlarını kabul edin veya Exchange klasörleri için özel erişim düzeylerini seçin.</span><span class="sxs-lookup"><span data-stu-id="0baf9-111">In the **Delegate Permissions** dialog box, accept the default permission settings or select custom access levels for Exchange folders.</span></span>

    - <span data-ttu-id="0baf9-112">Bir temsilcinin yalnızca Toplantı istekleri ve yanıtları ile çalışma izni olması gerekiyorsa, temsilci gibi varsayılan izin ayarları, **bana gönderilen toplantı ile ilgili gelen iletilerin kopyalarını alır** .</span><span class="sxs-lookup"><span data-stu-id="0baf9-112">If a delegate needs permission to work only with meeting requests and responses, the default permission settings such as **Delegate receives copies of meeting-related messages sent to me** are sufficient.</span></span> <span data-ttu-id="0baf9-113">**Gelen kutusu** Izin ayarını **yok** olarak bırakabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="0baf9-113">You can leave the **Inbox** permission setting at **None**.</span></span> <span data-ttu-id="0baf9-114">Toplantı istekleri ve yanıtları doğrudan temsilcinin gelen kutusuna gidecek.</span><span class="sxs-lookup"><span data-stu-id="0baf9-114">Meeting requests and responses will go directly to the delegate's inbox.</span></span>

    > [!NOTE]
    > <span data-ttu-id="0baf9-115">Varsayılan olarak, temsilcinin **Takvim** klasörünüze **Düzenleyici (öğeleri okuyabilir, oluşturabilir ve değiştirebilir)** izni verilir.</span><span class="sxs-lookup"><span data-stu-id="0baf9-115">By default, the delegate is granted **Editor (can read, create, and modify items)** permission to your **Calendar** folder.</span></span> <span data-ttu-id="0baf9-116">Temsilci sizin adınıza bir toplantıya cevap verdiğinde, **Takvim** klasörünüze otomatik olarak eklenir.</span><span class="sxs-lookup"><span data-stu-id="0baf9-116">When the delegate responds to a meeting on your behalf, it is automatically added to your **Calendar** folder.</span></span>

5. <span data-ttu-id="0baf9-117">İzin verilmesini bildirmek üzere bir ileti göndermek için, **Bu izinleri özetleyen temsilciye otomatik olarak bir ileti gönder** seçeneğini işaretleyin.</span><span class="sxs-lookup"><span data-stu-id="0baf9-117">To send a message to notify the delegate of the changed permissions, select the **Automatically send a message to delegate summarizing these permissions** check box.</span></span>
6. <span data-ttu-id="0baf9-118">İsterseniz, **temsilci özel öğelerimi görebilir** kutusunu seçin.</span><span class="sxs-lookup"><span data-stu-id="0baf9-118">If you want, select the **Delegate can see my private items** check box.</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="0baf9-119">Bu ayar tüm Exchange klasörlerini etkiler.</span><span class="sxs-lookup"><span data-stu-id="0baf9-119">This setting affects all Exchange folders.</span></span> <span data-ttu-id="0baf9-120">Bu, tüm posta, kişiler, takvim, görevler, notlar ve günlük klasörlerini içerir.</span><span class="sxs-lookup"><span data-stu-id="0baf9-120">This includes all Mail, Contacts, Calendar, Tasks, Notes, and Journal folders.</span></span> <span data-ttu-id="0baf9-121">Yalnızca belirtilen klasörlerdeki özel öğelere erişim izni vermemenizin bir yolu yoktur.</span><span class="sxs-lookup"><span data-stu-id="0baf9-121">There is no way to grant access to private items in only specified folders.</span></span>

7. <span data-ttu-id="0baf9-122">**Tamam**'ı seçin.</span><span class="sxs-lookup"><span data-stu-id="0baf9-122">Choose **OK**.</span></span>

    > [!NOTE]
    >
    > - <span data-ttu-id="0baf9-123">Adına Gönder izinleriyle gönderilen mesajlar hem temsilcinin hem de **Kimden** adlarınızın yanında yer alır.</span><span class="sxs-lookup"><span data-stu-id="0baf9-123">Messages sent with Send on Behalf permissions include both the delegate's and your names next to **From**.</span></span> <span data-ttu-id="0baf9-124">Farklı Gönder izinleriyle bir ileti gönderildiğinde, yalnızca adınız görüntülenir.</span><span class="sxs-lookup"><span data-stu-id="0baf9-124">When a message is sent with Send As permissions, only your name appears.</span></span>
    > - <span data-ttu-id="0baf9-125">Bir kullanıcıyı temsilci olarak eklediğinizde, Exchange posta kutunuzu Outlook profilinize ekleyebilirler.</span><span class="sxs-lookup"><span data-stu-id="0baf9-125">Once you add someone as a delegate, they can add your Exchange mailbox to their Outlook profile.</span></span> <span data-ttu-id="0baf9-126">Yönergeler için, [başka birinin posta ve takvim öğelerini yönetme](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5)bölümüne bakın.</span><span class="sxs-lookup"><span data-stu-id="0baf9-126">For instructions, see [Manage another person's mail and calendar items](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5).</span></span>

<span data-ttu-id="0baf9-127">Windows için Outlook 'ta temsilciyi kaldırmak için:</span><span class="sxs-lookup"><span data-stu-id="0baf9-127">To remove a Delegate in Outlook for Windows:</span></span>

1. <span data-ttu-id="0baf9-128">**Dosya** sekmesini tıklatın.</span><span class="sxs-lookup"><span data-stu-id="0baf9-128">Click on the **File** tab.</span></span>
2. <span data-ttu-id="0baf9-129">**Hesap ayarları** 'nı ve ardından **temsilci erişimi**'ni tıklatın.</span><span class="sxs-lookup"><span data-stu-id="0baf9-129">Click on **Account Settings** followed by **Delegate Access**.</span></span>
3. <span data-ttu-id="0baf9-130">İzinlerini değiştirmek istediğiniz temsilcinin adını seçin **ve ardından** **Tamam 'a** tıklayın.</span><span class="sxs-lookup"><span data-stu-id="0baf9-130">Choose the name of the delegate for whom you want to change permissions, and then click on **Remove** followed by **OK**.</span></span>
