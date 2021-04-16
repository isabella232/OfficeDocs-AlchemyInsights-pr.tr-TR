---
title: Dosya açık salt okunur
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 39748581-d319-403c-8501-9b785e4a0ed8
ms.custom:
- "765"
- "2200014"
ms.openlocfilehash: e478572ea82e5ea11bac9fd7eacafb833253235d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813204"
---
# <a name="file-open-read-only"></a><span data-ttu-id="16436-102">Dosya açık salt okunur</span><span class="sxs-lookup"><span data-stu-id="16436-102">File open read-only</span></span>

<span data-ttu-id="16436-103">Dosyaları a açıyorken bunların salt okunur olarak aç olduğunu bulabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="16436-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="16436-104">Bazı durumlarda, örneğin İnternet'te dosya aken ek güvenlik için bu olabilir ve diğer zamanlarda, değiştiril bir ayardan dolayı söz konusu olabilir.</span><span class="sxs-lookup"><span data-stu-id="16436-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="16436-105">Burada, dosyanın salt okunur aç olduğu bazı senaryolar ve bunu değiştirmek için atabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="16436-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="16436-106">**Virüsten koruma yazılımım salt okunur açılmasına neden oluyor**</span><span class="sxs-lookup"><span data-stu-id="16436-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="16436-107">Bazı virüsten koruma programları, dosyaları salt okunur açarak güvenli olmayabilecek dosyalara karşı sizi koruyabilir.</span><span class="sxs-lookup"><span data-stu-id="16436-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="16436-108">Bu ayarların nasıl ayarla ilgili olduğunu öğrenmek için virüsten koruma sağlayıcınıza danışın.</span><span class="sxs-lookup"><span data-stu-id="16436-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="16436-109">Örneğin BitDefender'ın uygulama dışlamaları ekleme içeriğini burada bulunmaktadır: [Bitdefender Control Center'da](https://aka.ms/AA6098i)uygulama veya işlem dışlamaları ekleme.</span><span class="sxs-lookup"><span data-stu-id="16436-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://aka.ms/AA6098i).</span></span>
  
 <span data-ttu-id="16436-110">**Dosya özellikleri salt okunur olarak mı ayarlanmış?**</span><span class="sxs-lookup"><span data-stu-id="16436-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="16436-111">Dosyaya sağ tık tıklar ve Özellikler'i seçerek dosya özelliklerini kontrol edin.</span><span class="sxs-lookup"><span data-stu-id="16436-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="16436-112">Salt okunur özniteliği işaretli olursa, işaretini kaldırarak Tamam'ı tıklatın.</span><span class="sxs-lookup"><span data-stu-id="16436-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="16436-113">**İçerik korumalı görünümde**</span><span class="sxs-lookup"><span data-stu-id="16436-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="16436-114">İnternet ve güvenli olmayabilecek konumlardan alınan dosyalar virüs, solucan veya bilgisayarınıza zarar verecek başka bir tür kötü amaçlı yazılım içerebilir.</span><span class="sxs-lookup"><span data-stu-id="16436-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="16436-115">E-posta ekleri veya indirdiğiniz dosyalar için de bu durum yaygındır.</span><span class="sxs-lookup"><span data-stu-id="16436-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="16436-116">Bilgisayarınızın korunmasına yardımcı olmak için, güvenli olmayabilecek bu konumlardan gelen dosyalar Korumalı Görünüm'de açılır.</span><span class="sxs-lookup"><span data-stu-id="16436-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="16436-117">Korumalı Görünüm'i kullanarak dosyayı okuyabilir ve içeriğini görebilir ve bu arada riski de azaltabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="16436-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="16436-118">Korumalı görünüm ve ayarları değiştirme hakkında daha fazla bilgi için şu makaleye bakın: [Korumalı Görünüm nedir?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="16436-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="16436-119">**OneDrive dolu mu?**</span><span class="sxs-lookup"><span data-stu-id="16436-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="16436-120">Dosya OneDrive'da depolanıyorsa ve OneDrive depolama alanınız dolu ise, size gereken alan altında olana kadar belgeyi kaydedesiniz.</span><span class="sxs-lookup"><span data-stu-id="16436-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="16436-121">OneDrive'da boş alanlarınızı kontrol etmek için bildirim merkezinde OneDrive simgesine tıklar ve Depolamayı yönet'i seçin veya 'a gidebilir, oturum açın ve ekranın sol alt köşesindeki kullanılan alan miktarını not [https://onedrive.live.com](https://onedrive.live.com) edin.</span><span class="sxs-lookup"><span data-stu-id="16436-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [https://onedrive.live.com](https://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="16436-122">**Office etkinleştirildi mi?**</span><span class="sxs-lookup"><span data-stu-id="16436-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="16436-123">Office etkinleştirilmemişse veya aboneliğinizin süresi dolmuşsa, salt okunur Sınırlı İşlevsellik Modundayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="16436-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="16436-124">Office'i etkinleştirme hakkında bilgi için bkz. [Office'te Lisanssız Ürün ve etkinleştirme hataları.](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)</span><span class="sxs-lookup"><span data-stu-id="16436-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="16436-125">**Diğer her şey başarısız olursa...**</span><span class="sxs-lookup"><span data-stu-id="16436-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="16436-126">Bilgisayarı yeniden başlatmayı deneyin</span><span class="sxs-lookup"><span data-stu-id="16436-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="16436-127">Office güncelleştirmelerini yükleme</span><span class="sxs-lookup"><span data-stu-id="16436-127">Install Office updates</span></span>
    
- <span data-ttu-id="16436-128">Office'in Çevrimiçi onarımını gerçekleştirin</span><span class="sxs-lookup"><span data-stu-id="16436-128">Perform an Online repair of Office</span></span>
    

