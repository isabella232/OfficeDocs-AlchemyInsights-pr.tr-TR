---
title: Yammer'da görüntü yükleme sorunları giderme
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6000"
- "9003112"
ms.openlocfilehash: 93894eaa5818b591acd1c7b9a90bc1cabbe00450
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148419"
---
# <a name="troubleshoot-image-loading-issues-in-yammer"></a><span data-ttu-id="eec85-102">Yammer'da görüntü yükleme sorunları giderme</span><span class="sxs-lookup"><span data-stu-id="eec85-102">Troubleshoot image loading issues in Yammer</span></span>

<span data-ttu-id="eec85-103">Yammer'da fotoğraf ve dosya önizlemelerinde sorunlar oluştuğunda, sorunun tüm kullanıcılar için oluşup oluşmadığını, mobil cihazlarda oluşup oluşmadığını ve eki yüklerken tekrarlanabilir olup olmadığını denetleyerek sorun giderin.</span><span class="sxs-lookup"><span data-stu-id="eec85-103">When issues occur with photos and file previews in Yammer, troubleshoot by checking whether the issue occurs for all users, whether it occurs on mobile devices, and if it is reproducible when uploading the attachment.</span></span>  

<span data-ttu-id="eec85-104">**Profil fotoğrafı sorunları**</span><span class="sxs-lookup"><span data-stu-id="eec85-104">**Profile photo issues**</span></span>  

<span data-ttu-id="eec85-105">Son kullanıcılar Yammer'da Microsoft 365 üzerinden oturum açsa, profil fotoğraflarını da içeren profillerini değiştirmeleri gerekir.</span><span class="sxs-lookup"><span data-stu-id="eec85-105">If end users sign into Yammer via Microsoft 365, they must change their profile, including their profile photo.</span></span> <span data-ttu-id="eec85-106">Kullanıcıların profil güncelleştirmeleri yapmasına izin verilmiyorsa, bir yönetici güncelleştirmeyi kullanıcı için yapabilir.</span><span class="sxs-lookup"><span data-stu-id="eec85-106">If users are not permitted to make profile updates, an admin can make the update for the user.</span></span> <span data-ttu-id="eec85-107">Daha fazla bilgi için [Office Delve'deki profilinizi görüntüle ve güncelle' ye](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba)bakın.</span><span class="sxs-lookup"><span data-stu-id="eec85-107">For more info, see [View and update your profile in Office Delve](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span></span>

<span data-ttu-id="eec85-108">Profil fotoğrafları da dahil olmak üzere profil düzenleme hakkında daha fazla bilgi için Bkz. [Yammer profilimi ve ayarlarını değiştirin.](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851)</span><span class="sxs-lookup"><span data-stu-id="eec85-108">For info about profile editing, including profile photos, see [Change my Yammer profile and settings](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851).</span></span> 

<span data-ttu-id="eec85-109">Güncelleştirilmiş profil fotoğrafları profil özniteliklerinden farklı olarak eşitlenir.</span><span class="sxs-lookup"><span data-stu-id="eec85-109">Updated profile photos are synced differently than profile attributes.</span></span> <span data-ttu-id="eec85-110">Kullanıcıların profil fotoğraflarının senkronizesini başlatmak için oturum açmaları gerekir.</span><span class="sxs-lookup"><span data-stu-id="eec85-110">Users must sign in to initiate a sync of their profile photo.</span></span> <span data-ttu-id="eec85-111">Daha fazla bilgi için, [Office 365'ten Yammer'a güncellenen kullanıcı profili resimlerine](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer)bakın.</span><span class="sxs-lookup"><span data-stu-id="eec85-111">For info, see [are user profile pictures updated from Office 365 to Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer).</span></span>

<span data-ttu-id="eec85-112">Yammer için kullanıcı yaşam döngüsü hakkında daha fazla bilgi için [Bkz.](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle)</span><span class="sxs-lookup"><span data-stu-id="eec85-112">For info about the user lifecycle for Yammer, see [Manage Yammer users across their lifecycle from Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle).</span></span>  

<span data-ttu-id="eec85-113">Profil resmi eşitlemenin Microsoft 365'te nasıl çalıştığına ilişkin ayrıntılar için Microsoft [365'teki profil resmi eşitleme hakkında bilgi](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a)ye bakın.</span><span class="sxs-lookup"><span data-stu-id="eec85-113">For details on how profile picture sync works in Microsoft 365, see [Information about profile picture synchronization in Microsoft 365](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a).</span></span>  

<span data-ttu-id="eec85-114">**Belge önizlemeleri ve resim küçük resim sorunları**</span><span class="sxs-lookup"><span data-stu-id="eec85-114">**Document previews and image thumbnail issues**</span></span>  

<span data-ttu-id="eec85-115">Dosyalar veya resimler Yammer'a nakledildiğinde, önizlemeler görünmeyebilir çünkü:</span><span class="sxs-lookup"><span data-stu-id="eec85-115">When files or images are posted to Yammer, previews might not appear because:</span></span> 

- <span data-ttu-id="eec85-116">Dosya bozuk ve işlenemez.</span><span class="sxs-lookup"><span data-stu-id="eec85-116">The file is corrupt and cannot be processed.</span></span>
- <span data-ttu-id="eec85-117">Dosya yakın zamanda SharePoint Online'a yüklenmedi veya Yammer'ın başka nedenlerle geçersiz meta verileri var.</span><span class="sxs-lookup"><span data-stu-id="eec85-117">The file has not been recently uploaded to SharePoint Online, or Yammer has invalid metadata for other reasons.</span></span>
- <span data-ttu-id="eec85-118">Önizleme görüntülerinin yüklenmesi için gereken URL'ler engellenir.</span><span class="sxs-lookup"><span data-stu-id="eec85-118">URLs required for loading the preview images are blocked.</span></span>
- <span data-ttu-id="eec85-119">Dosya önizlemesi deftere nakledilmeden önce kullanıcı tarafından kaldırıldı.</span><span class="sxs-lookup"><span data-stu-id="eec85-119">The file preview was removed by the user before posting.</span></span>
- <span data-ttu-id="eec85-120">Hizmet sorunu, önizlemenin oluşturulmasını engelledi.</span><span class="sxs-lookup"><span data-stu-id="eec85-120">A service issue prevented a preview being generated.</span></span>

<span data-ttu-id="eec85-121">**Not** Bağlantılar ve dosya yüklemeleri için önizlemeler farklı davranabilir.</span><span class="sxs-lookup"><span data-stu-id="eec85-121">**Note** Previews for links and file uploads might behave differently.</span></span> <span data-ttu-id="eec85-122">Internet'teki dosyalara bağlantılar veya ek kimlik doğrulaması gerektiren bağlantılar doğru görüntülemeyebilir.</span><span class="sxs-lookup"><span data-stu-id="eec85-122">Links to files on the internet or links that require additional authentication might not display correctly.</span></span>

<span data-ttu-id="eec85-123">Daha fazla bilgi için [bkz.](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf)</span><span class="sxs-lookup"><span data-stu-id="eec85-123">For more info, see [Attach a file or image to a Yammer message](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf).</span></span> 