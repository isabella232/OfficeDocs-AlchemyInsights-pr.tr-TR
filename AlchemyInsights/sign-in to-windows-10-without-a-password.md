---
title: Parola kullanmadan Windows 10'da oturum açma
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 1f325eb7afb1e88457296e8187f8ba6dff2ebfe0
ms.sourcegitcommit: 00e4266575438f55bdc18db05ed54aafcb75a3c9
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/11/2020
ms.locfileid: "42588300"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="c4dd2-102">Parola kullanmadan Windows 10'da oturum açma</span><span class="sxs-lookup"><span data-stu-id="c4dd2-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="c4dd2-103">Windows'un başlatılmasında parola yazmak zorunda kalmamak için, varsa PIN, yüz tanıma veya parmak izi gibi Windows Hello güvenli oturum açma seçeneklerinden birini kullanmanızı öneririz.</span><span class="sxs-lookup"><span data-stu-id="c4dd2-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="c4dd2-104">Güvenli oturum açma'yı gerçekten devre dışı kılmış olmak istiyorsanız, aşağıdaki "Windows 10'da otomatik olarak oturum açın" yönergelerine bakın.</span><span class="sxs-lookup"><span data-stu-id="c4dd2-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="c4dd2-105">**Hesap parolasına güvenli Windows Hello alternatifleri**</span><span class="sxs-lookup"><span data-stu-id="c4dd2-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="c4dd2-106">Hesaplar **> Ayarlar>a** gidin (veya [buraya](ms-settings:signinoptions?activationSource=GetHelp)tıklayın).</span><span class="sxs-lookup"><span data-stu-id="c4dd2-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="c4dd2-107">Kullanılabilir oturum açma seçenekleri listelenir.</span><span class="sxs-lookup"><span data-stu-id="c4dd2-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="c4dd2-108">Örneğin:</span><span class="sxs-lookup"><span data-stu-id="c4dd2-108">For example:</span></span>

![Oturum açma seçenekleri.](media/sign-in-options.png)

<span data-ttu-id="c4dd2-110">Yapılandırmak için seçeneklerden birini tıklatın veya dokunun.</span><span class="sxs-lookup"><span data-stu-id="c4dd2-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="c4dd2-111">Windows'u bir sonraki başlattığınızda veya kilidini açtığınızda, parola yerine yeni seçeneği kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="c4dd2-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="c4dd2-112">**Windows 10'da otomatik oturum açma**</span><span class="sxs-lookup"><span data-stu-id="c4dd2-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="c4dd2-113">**Not**: Otomatik oturum açma uygundur, ancak özellikle bilgisayarınıza birden fazla kişi tarafından erişilebiliyorsa, güvenlik riski oluşturur.</span><span class="sxs-lookup"><span data-stu-id="c4dd2-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="c4dd2-114">Görev Çubuğu'ndaki **Başlat** düğmesini tıklatın veya dokunun.</span><span class="sxs-lookup"><span data-stu-id="c4dd2-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="c4dd2-115">**Netplwiz** yazın ve Kullanıcı Hesapları penceresini açmak için Enter tuşuna basın.</span><span class="sxs-lookup"><span data-stu-id="c4dd2-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="c4dd2-116">**Kullanıcı**Hesapları'nda, Windows başladığında otomatik olarak oturum açmanız istediğiniz hesabı tıklatın.</span><span class="sxs-lookup"><span data-stu-id="c4dd2-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="c4dd2-117">"Kullanıcılar bu bilgisayarı kullanmak için bir kullanıcı adı ve parola girmeli" onay kutusunun işaretlerini kaldırın.</span><span class="sxs-lookup"><span data-stu-id="c4dd2-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![Kullanıcıların bir kullanıcı adı ve parola seçeneği girmeleri gerekir.](media/users-must-enter-username.png)

5. <span data-ttu-id="c4dd2-119">**Tamam**'a tıklayın.</span><span class="sxs-lookup"><span data-stu-id="c4dd2-119">Click **OK**.</span></span> <span data-ttu-id="c4dd2-120">Seçtiğiniz hesabın parolasını girmeniz ve onaylamanız istenir.</span><span class="sxs-lookup"><span data-stu-id="c4dd2-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="c4dd2-121">Bitirmek için **Tamam'ı** tıklatın.</span><span class="sxs-lookup"><span data-stu-id="c4dd2-121">Click **OK** to finish.</span></span> <span data-ttu-id="c4dd2-122">Windows 10 bir sonraki başlatılında, seçtiğiniz hesapta otomatik olarak oturum açacaktır.</span><span class="sxs-lookup"><span data-stu-id="c4dd2-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
