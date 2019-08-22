---
title: Dosyayı salt okunur açmak
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 39748581-d319-403c-8501-9b785e4a0ed8
ms.openlocfilehash: 5c28d5f1c6951971aab329060e24b8458e848dd7
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36525691"
---
# <a name="file-open-read-only"></a><span data-ttu-id="a22a2-102">Dosyayı salt okunur açmak</span><span class="sxs-lookup"><span data-stu-id="a22a2-102">File open read-only</span></span>

<span data-ttu-id="a22a2-103">Dosyaları açarken, bunlar salt okunur olarak açmasını bulabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="a22a2-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="a22a2-104">Bazı durumlarda, Internet ve diğer zamanlarda dosyalarını açma, değiştirilebilir bir ayar nedeniyle olabilir gibi daha fazla güvenlik için budur.</span><span class="sxs-lookup"><span data-stu-id="a22a2-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="a22a2-105">Bazı senaryolar nerede salt okunur bir dosyayı açar ve değiştirmek için uygulayabileceğiniz bazı adımlar aşağıdadır.</span><span class="sxs-lookup"><span data-stu-id="a22a2-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="a22a2-106">**Benim antivirus salt okunur açmak onları neden oluyor**</span><span class="sxs-lookup"><span data-stu-id="a22a2-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="a22a2-107">Bazı virüsten koruma programları bunları salt okunur açarak güvenli olmama olasılığı bulunan dosyalardan korumanıza.</span><span class="sxs-lookup"><span data-stu-id="a22a2-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="a22a2-108">Bu ayarları öğrenmek için virüsten koruma programınızın sağlayıcısına denetlemeniz gerekebilir.</span><span class="sxs-lookup"><span data-stu-id="a22a2-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="a22a2-109">BitDefender, örneğin, uygulama dışlamalarını ekleme içerik vardır: [uygulama veya işlem Dışlamalar Bitdefender Control Center'da ekleme](https://www.bitdefender.com/support/how-to-add-application-or-process-exclusions-in-bitdefender-control-center-1119.mdl).</span><span class="sxs-lookup"><span data-stu-id="a22a2-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://www.bitdefender.com/support/how-to-add-application-or-process-exclusions-in-bitdefender-control-center-1119.mdl).</span></span>
  
 <span data-ttu-id="a22a2-110">**Dosya özellikleri salt okunur olarak ayarlanır?**</span><span class="sxs-lookup"><span data-stu-id="a22a2-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="a22a2-111">Dosya özellikleri, dosyayı sağ tıklayıp Özellikler'i seçerek denetleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="a22a2-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="a22a2-112">Salt okunur özniteliği seçili ise, onay işaretini kaldırın ve Tamam'ı tıklatın.</span><span class="sxs-lookup"><span data-stu-id="a22a2-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="a22a2-113">**İçerik korumalı görünümde olur.**</span><span class="sxs-lookup"><span data-stu-id="a22a2-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="a22a2-114">Internet ve diğer güvenli olmama olasılığı bulunan yerlerden gelen dosyaları virüs, solucan veya diğer tür, bilgisayarınıza zarar verebilecek kötü amaçlı yazılım içerebilir.</span><span class="sxs-lookup"><span data-stu-id="a22a2-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="a22a2-115">Bu da genellikle e-posta eklerini veya karşıdan yüklediğiniz dosyaları ile durumdur.</span><span class="sxs-lookup"><span data-stu-id="a22a2-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="a22a2-116">Bilgisayarınızın korunmasına yardımcı olmak için güvenli olmama olasılığı bulunan bu konumlardan dosya Korumalı Görünüm'de açılır.</span><span class="sxs-lookup"><span data-stu-id="a22a2-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="a22a2-117">Korumalı Görünüm'ü kullanarak, bir dosyayı okumasına ve riskleri azaltmanın yanı sıra içeriğine bakın.</span><span class="sxs-lookup"><span data-stu-id="a22a2-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="a22a2-118">Korumalı Görünüm ve ayarlarının nasıl değiştirileceği hakkında daha fazla bilgi için bu makaleye bakın: [Korumalı Görünüm nedir?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="a22a2-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="a22a2-119">**OneDrive dolu mu?**</span><span class="sxs-lookup"><span data-stu-id="a22a2-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="a22a2-120">Dosya OneDrive üzerinde depolanır ve OneDrive depolama alanınızı tam ise, ayrılan alanınızı altında kalana kadar belgeyi kaydedemedi olacaktır.</span><span class="sxs-lookup"><span data-stu-id="a22a2-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="a22a2-121">Bildirim merkezi OneDrive simgesini tıklattıktan sonra Yönet depolama seçerek OneDrive, boş alanı denetleyin veya gidebilirsiniz [http://onedrive.live.com](http://onedrive.live.com), oturum açma ve ekranın sol alt içinde kullanılan alan miktarını not edin.</span><span class="sxs-lookup"><span data-stu-id="a22a2-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [http://onedrive.live.com](http://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="a22a2-122">**Office etkinleştirildi mi?**</span><span class="sxs-lookup"><span data-stu-id="a22a2-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="a22a2-123">Office etkinleştirilmemişse veya aboneliğinizi süresi dolmuşsa, salt okunur sınırlı işlevsellik Modu'nda olabilir.</span><span class="sxs-lookup"><span data-stu-id="a22a2-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="a22a2-124">Office etkinleştirme hakkında daha fazla bilgi için bkz: [Office Etkinleştirme hataları ve lisanssız ürün](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="a22a2-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="a22a2-125">**Hepsi başarısız olursa...**</span><span class="sxs-lookup"><span data-stu-id="a22a2-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="a22a2-126">Bilgisayarı yeniden başlatmayı deneyin.</span><span class="sxs-lookup"><span data-stu-id="a22a2-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="a22a2-127">Office güncelleştirmelerini yükleme</span><span class="sxs-lookup"><span data-stu-id="a22a2-127">Install Office updates</span></span>
    
- <span data-ttu-id="a22a2-128">Office Online bir onarım gerçekleştirin</span><span class="sxs-lookup"><span data-stu-id="a22a2-128">Perform an Online repair of Office</span></span>
    

