---
title: Parola kullanmadan Windows 10'da oturum açma
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 1c03f00f7b41ea16d3106b19b998edeea6114603
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830566"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="535af-102">Parola kullanmadan Windows 10'da oturum açma</span><span class="sxs-lookup"><span data-stu-id="535af-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="535af-103">Windows başlangıçta parola yazmamak için PIN, yüz tanıma veya parmak izi gibi (varsa) Windows Hello güvenli oturum açma seçeneklerindan birini öneririz.</span><span class="sxs-lookup"><span data-stu-id="535af-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="535af-104">Güvenli oturum açma özelliğini gerçekten devre dışı bırakmak için aşağıdaki "Windows 10'da otomatik olarak oturum açma" yönergelerine bakın.</span><span class="sxs-lookup"><span data-stu-id="535af-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="535af-105">**Hesap parolasının güvenli Windows Hello alternatifleri**</span><span class="sxs-lookup"><span data-stu-id="535af-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="535af-106">Oturum açma **seçenekleri > Hesaplar ve > ayarlar'a gidin (veya** buraya [tıklayın).](ms-settings:signinoptions?activationSource=GetHelp)</span><span class="sxs-lookup"><span data-stu-id="535af-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="535af-107">Kullanılabilir oturum açma seçenekleri listelenir.</span><span class="sxs-lookup"><span data-stu-id="535af-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="535af-108">Örneğin:</span><span class="sxs-lookup"><span data-stu-id="535af-108">For example:</span></span>

![Oturum açma seçenekleri.](media/sign-in-options.png)

<span data-ttu-id="535af-110">Yapılandırmak için seçeneklerden birini tıklatın veya dokunun.</span><span class="sxs-lookup"><span data-stu-id="535af-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="535af-111">Windows'u bir sonraki başlatacak veya kilidini açmayacaksanız, parola yerine yeni seçeneği kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="535af-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="535af-112">**Windows 10'da otomatik olarak oturum açma**</span><span class="sxs-lookup"><span data-stu-id="535af-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="535af-113">**Not:** Otomatik oturum açma kullanışlı bir oturum açmadır, ancak özellikle de bilgisayarınıza birden çok kişi tarafından erişilse bir güvenlik riski getirir.</span><span class="sxs-lookup"><span data-stu-id="535af-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="535af-114">Görev çubuğunda Başlat **düğmesine** tıklayın veya dokunun.</span><span class="sxs-lookup"><span data-stu-id="535af-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="535af-115">Kullanıcı Hesapları penceresini açmak için **netplwiz** yazın ve Enter tuşuna basın.</span><span class="sxs-lookup"><span data-stu-id="535af-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="535af-116">Kullanıcı **Hesapları'nın** altında, Windows başlatıldığında otomatik olarak oturum açmasını istediğiniz hesaba tıklayın.</span><span class="sxs-lookup"><span data-stu-id="535af-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="535af-117">"Kullanıcıların bu bilgisayarı kullanmak için kullanıcı adı ve parola girmeleri gerekir" onay kutusunun işaretini kaldırın.</span><span class="sxs-lookup"><span data-stu-id="535af-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![Kullanıcıların bir kullanıcı adı ve parola seçeneği girmeleri gerekir.](media/users-must-enter-username.png)

5. <span data-ttu-id="535af-119">**Tamam**'a tıklayın.</span><span class="sxs-lookup"><span data-stu-id="535af-119">Click **OK**.</span></span> <span data-ttu-id="535af-120">Seçtiğiniz hesabın parolasını girmeniz ve onaylamanız istenir.</span><span class="sxs-lookup"><span data-stu-id="535af-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="535af-121">Bitirmek **için Tamam'a** tıklayın.</span><span class="sxs-lookup"><span data-stu-id="535af-121">Click **OK** to finish.</span></span> <span data-ttu-id="535af-122">Windows 10 yeniden başlatıldığında, seçtiğiniz hesapta otomatik olarak oturum açılır.</span><span class="sxs-lookup"><span data-stu-id="535af-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
