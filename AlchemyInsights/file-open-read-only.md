---
title: Dosyayı salt okunur açmak
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 39748581-d319-403c-8501-9b785e4a0ed8
ms.openlocfilehash: 6c4610a133cf4202310bfd166a61ab84ca6ecdbb
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29661807"
---
# <a name="file-open-read-only"></a><span data-ttu-id="e2f51-102">Dosyayı salt okunur açmak</span><span class="sxs-lookup"><span data-stu-id="e2f51-102">File open read-only</span></span>

<span data-ttu-id="e2f51-p101">Dosyaları açarken, bunlar salt okunur olarak açmasını bulabilirsiniz. Bazı durumlarda, Internet ve diğer zamanlarda dosyalarını açma, değiştirilebilir bir ayar nedeniyle olabilir gibi daha fazla güvenlik için budur. Bazı senaryolar nerede salt okunur bir dosyayı açar ve değiştirmek için uygulayabileceğiniz bazı adımlar aşağıdadır.</span><span class="sxs-lookup"><span data-stu-id="e2f51-p101">You may find that when you are opening files, they open as read-only. In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed. Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="e2f51-106">**Benim antivirus salt okunur açmak onları neden oluyor**</span><span class="sxs-lookup"><span data-stu-id="e2f51-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="e2f51-p102">Bazı virüsten koruma programları bunları salt okunur açarak güvenli olmama olasılığı bulunan dosyalardan korumanıza. Bu ayarları öğrenmek için virüsten koruma programınızın sağlayıcısına denetlemeniz gerekebilir. BitDefender, örneğin, uygulama dışlamalarını ekleme içerik vardır: [uygulama veya işlem Dışlamalar Bitdefender Control Center'da ekleme](https://www.bitdefender.com/support/how-to-add-application-or-process-exclusions-in-bitdefender-control-center-1119.mdl).</span><span class="sxs-lookup"><span data-stu-id="e2f51-p102">Some antivirus programs may protect you from potentially unsafe files by opening them read-only. You may need to check with your antivirus provider to learn how to adjust these settings. BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://www.bitdefender.com/support/how-to-add-application-or-process-exclusions-in-bitdefender-control-center-1119.mdl).</span></span>
  
 <span data-ttu-id="e2f51-110">**Dosya özellikleri salt okunur olarak ayarlanır?**</span><span class="sxs-lookup"><span data-stu-id="e2f51-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="e2f51-p103">Dosya özellikleri, dosyayı sağ tıklayıp Özellikler'i seçerek denetleyebilirsiniz. Salt okunur özniteliği seçili ise, onay işaretini kaldırın ve Tamam'ı tıklatın.</span><span class="sxs-lookup"><span data-stu-id="e2f51-p103">You can check the file properties by right-clicking on the file and choosing Properties. If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="e2f51-113">**İçerik korumalı görünümde olur.**</span><span class="sxs-lookup"><span data-stu-id="e2f51-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="e2f51-p104">Internet ve diğer güvenli olmama olasılığı bulunan yerlerden gelen dosyaları virüs, solucan veya diğer tür, bilgisayarınıza zarar verebilecek kötü amaçlı yazılım içerebilir. Bu da genellikle e-posta eklerini veya karşıdan yüklediğiniz dosyaları ile durumdur. Bilgisayarınızın korunmasına yardımcı olmak için güvenli olmama olasılığı bulunan bu konumlardan dosya Korumalı Görünüm'de açılır. Korumalı Görünüm'ü kullanarak, bir dosyayı okumasına ve riskleri azaltmanın yanı sıra içeriğine bakın. Korumalı Görünüm ve ayarlarının nasıl değiştirileceği hakkında daha fazla bilgi için bu makaleye bakın: [Korumalı Görünüm nedir?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="e2f51-p104">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer. This is also commonly the case with email attachments or files you've downloaded. To help protect your computer, files from these potentially unsafe locations are opened in Protected View. By using Protected View, you can read a file and see its contents while reducing the risks. For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="e2f51-119">**OneDrive dolu mu?**</span><span class="sxs-lookup"><span data-stu-id="e2f51-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="e2f51-p105">Dosya OneDrive üzerinde depolanır ve OneDrive depolama alanınızı tam ise, ayrılan alanınızı altında kalana kadar belgeyi kaydedemedi olacaktır. Bildirim merkezi OneDrive simgesini tıklattıktan sonra Yönet depolama seçerek OneDrive, boş alanı denetleyin veya gidebilirsiniz [http://onedrive.live.com](http://onedrive.live.com), oturum açma ve ekranın sol alt içinde kullanılan alan miktarını not edin.</span><span class="sxs-lookup"><span data-stu-id="e2f51-p105">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space. You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [http://onedrive.live.com](http://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="e2f51-122">**Office etkinleştirildi mi?**</span><span class="sxs-lookup"><span data-stu-id="e2f51-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="e2f51-p106">Office etkinleştirilmemişse veya aboneliğinizi süresi dolmuşsa, salt okunur sınırlı işlevsellik Modu'nda olabilir. Office etkinleştirme hakkında daha fazla bilgi için bkz: [Office Etkinleştirme hataları ve lisanssız ürün](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="e2f51-p106">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode. For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="e2f51-125">**Hepsi başarısız olursa...**</span><span class="sxs-lookup"><span data-stu-id="e2f51-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="e2f51-126">Bilgisayarı yeniden başlatmayı deneyin.</span><span class="sxs-lookup"><span data-stu-id="e2f51-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="e2f51-127">Office güncelleştirmelerini yükleme</span><span class="sxs-lookup"><span data-stu-id="e2f51-127">Install Office updates</span></span>
    
- <span data-ttu-id="e2f51-128">Office Online bir onarım gerçekleştirin</span><span class="sxs-lookup"><span data-stu-id="e2f51-128">Perform an Online repair of Office</span></span>
    

