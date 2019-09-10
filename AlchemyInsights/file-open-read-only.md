---
title: Yalnızca okundu'u aç
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 39748581-d319-403c-8501-9b785e4a0ed8
ms.custom:
- "765"
- "2200014"
ms.openlocfilehash: eddd427b159a782abf53adda934de8b15a02ed00
ms.sourcegitcommit: 8864b5789d9905916039081b53530c7e6d8bc529
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/10/2019
ms.locfileid: "36822254"
---
# <a name="file-open-read-only"></a><span data-ttu-id="67867-102">Yalnızca okundu'u aç</span><span class="sxs-lookup"><span data-stu-id="67867-102">File open read-only</span></span>

<span data-ttu-id="67867-103">Dosyaları açarken, yalnızca okunur olarak açılacağını görebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="67867-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="67867-104">Bazı durumlarda, bu, internetten dosyaları açarken olduğu gibi ek güvenlik içindir ve diğer zamanlarda değiştirilebilir bir ayar nedeniyle olabilir.</span><span class="sxs-lookup"><span data-stu-id="67867-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="67867-105">Burada, bir dosyanın salt okunur olarak açıldığı bazı senaryolar ve bunu değiştirmek için atabileceğiniz bazı adımlar verilmiştir.</span><span class="sxs-lookup"><span data-stu-id="67867-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="67867-106">**Antivirüs, yalnızca okunur'u açmalarına neden oluyor**</span><span class="sxs-lookup"><span data-stu-id="67867-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="67867-107">Bazı virüsten koruma programları, yalnızca okunur olarak açarak güvenli olmayan dosyaları korumanızı sağlayabilir.</span><span class="sxs-lookup"><span data-stu-id="67867-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="67867-108">Bu ayarları nasıl ayarladığınızı öğrenmek için virüsten koruma sağlayıcınıza danışabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="67867-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="67867-109">BitDefender, örneğin, burada uygulama dışlamaları ekleyerek içerik vardır: [Nasıl Bitdefender Kontrol Merkezi'nde uygulama veya süreç dışlamalar eklemek için](https://aka.ms/AA6098i).</span><span class="sxs-lookup"><span data-stu-id="67867-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://aka.ms/AA6098i).</span></span>
  
 <span data-ttu-id="67867-110">**Dosya özellikleri salt okunur olarak mı ayarlandı?**</span><span class="sxs-lookup"><span data-stu-id="67867-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="67867-111">Dosyaya sağ tıklayıp Özellikler'i seçerek dosya özelliklerini kontrol edebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="67867-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="67867-112">Salt okunur özniteliği işaretlenirse, bunun denetimini geri alabilir ve Tamam'ı tıklatabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="67867-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="67867-113">**İçerik korumalı görünümde**</span><span class="sxs-lookup"><span data-stu-id="67867-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="67867-114">Internet'ten ve diğer güvenli olmayan konumlardan gelen dosyalar, bilgisayarınıza zarar verebilecek virüsler, solucanlar veya başka türde kötü amaçlı yazılımlar içerebilir.</span><span class="sxs-lookup"><span data-stu-id="67867-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="67867-115">Bu durum, indirdiğiniz e-posta ekleri veya dosyalarda da yaygın olarak geçerlidir.</span><span class="sxs-lookup"><span data-stu-id="67867-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="67867-116">Bilgisayarınızın korunmasına yardımcı olmak için, bu güvenli olmayan konumlardaki dosyalar Korumalı Görünüm'de açılır.</span><span class="sxs-lookup"><span data-stu-id="67867-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="67867-117">Korumalı Görünüm'i kullanarak, riskleri azaltırken bir dosyayı okuyabilir ve içeriğini görebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="67867-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="67867-118">Korumalı görünüm ve ayarları niçin değiştireceğiniz hakkında daha fazla bilgi için şu makaleye bakın: [Korumalı Görünüm nedir?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="67867-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="67867-119">**OneDrive dolu mu?**</span><span class="sxs-lookup"><span data-stu-id="67867-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="67867-120">Dosya OneDrive'da depolanırsa ve OneDrive depolama alanınız doluysa, ayrılan alanın altına gelene kadar belgeyi kaydedemezsiniz.</span><span class="sxs-lookup"><span data-stu-id="67867-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="67867-121">Bildirim merkezindeki OneDrive simgesine tıklayıp depolamayı yönet'i seçerek OneDrive'daki boş alanınızı kontrol edebilir veya [http://onedrive.live.com](http://onedrive.live.com)ekranın sol alt tarafındaki oturum açma ve kullanılan alan miktarına dikkat edebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="67867-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [http://onedrive.live.com](http://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="67867-122">**Office etkinleştirildi mi?**</span><span class="sxs-lookup"><span data-stu-id="67867-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="67867-123">Office etkinleştirilmemişse veya aboneliğinizin süresi dolmuşsa, salt okunur Azaltılmış İşlevsellik Modunda olabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="67867-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="67867-124">Office'i etkinleştirme hakkında daha fazla bilgi için bkz: [Office'te Lisanssız Ürün ve etkinleştirme hataları.](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)</span><span class="sxs-lookup"><span data-stu-id="67867-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="67867-125">**Her şey başarısız olursa...**</span><span class="sxs-lookup"><span data-stu-id="67867-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="67867-126">Bilgisayarı yeniden başlatmayı deneyin</span><span class="sxs-lookup"><span data-stu-id="67867-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="67867-127">Office güncelleştirmelerini yükleme</span><span class="sxs-lookup"><span data-stu-id="67867-127">Install Office updates</span></span>
    
- <span data-ttu-id="67867-128">Office'in Çevrimiçi onarımını gerçekleştirin</span><span class="sxs-lookup"><span data-stu-id="67867-128">Perform an Online repair of Office</span></span>
    

