---
title: Parola kullanmadan Windows 10 ' da oturum açma
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 839b945c457cb007f13605c5b903ded75dadd1d7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47719973"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="af85a-102">Parola kullanmadan Windows 10 ' da oturum açma</span><span class="sxs-lookup"><span data-stu-id="af85a-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="af85a-103">Windows başlangıcında parola yazmak zorunda kalmamak için, varsa, bir PIN, yüz tanıma veya parmak izi gibi Windows Hello güvenli oturum açma seçeneklerinden birini kullanmanızı öneririz.</span><span class="sxs-lookup"><span data-stu-id="af85a-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="af85a-104">Güvenli oturum açmayı gerçekten devre dışı bırakmak istiyorsanız, aşağıdaki "Windows 10 ' da otomatik olarak oturum açma" yönergelerine bakın.</span><span class="sxs-lookup"><span data-stu-id="af85a-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="af85a-105">**Hesap parolasının güvenliğini sağlama**</span><span class="sxs-lookup"><span data-stu-id="af85a-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="af85a-106">**> hesap > oturum açma seçenekleri** 'ne gidin (veya [burayı](ms-settings:signinoptions?activationSource=GetHelp)tıklatın).</span><span class="sxs-lookup"><span data-stu-id="af85a-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="af85a-107">Kullanılabilir oturum açma seçenekleri listelenir.</span><span class="sxs-lookup"><span data-stu-id="af85a-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="af85a-108">Örneğin:</span><span class="sxs-lookup"><span data-stu-id="af85a-108">For example:</span></span>

![Oturum açma seçenekleri.](media/sign-in-options.png)

<span data-ttu-id="af85a-110">Yapılandırmak için seçeneklerden birine tıklayın veya dokunun.</span><span class="sxs-lookup"><span data-stu-id="af85a-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="af85a-111">Windows 'u bir sonraki başlatmanızda veya kilidini açtığınızda, parola yerine yeni seçeneğini kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="af85a-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="af85a-112">**Windows 10 ' da otomatik olarak oturum açma**</span><span class="sxs-lookup"><span data-stu-id="af85a-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="af85a-113">**Not**: otomatik oturum açma kullanışlı bir yöntemdir, ancak özellikle PC 'niz birden çok kişiyle erişilebilir durumdaysa güvenlik riski sunar.</span><span class="sxs-lookup"><span data-stu-id="af85a-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="af85a-114">Görev çubuğundaki **Başlat** düğmesine tıklayın veya dokunun.</span><span class="sxs-lookup"><span data-stu-id="af85a-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="af85a-115">Kullanıcı hesapları penceresini açmak için **Netplwiz** yazın ve ENTER tuşuna basın.</span><span class="sxs-lookup"><span data-stu-id="af85a-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="af85a-116">**Kullanıcı hesaplarında**, Windows başladığında otomatik olarak oturum açmak istediğiniz hesaba tıklayın.</span><span class="sxs-lookup"><span data-stu-id="af85a-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="af85a-117">"Kullanıcıların bu bilgisayarı kullanmak için bir Kullanıcı adı ve parola girmesi gerekir" onay kutusunu temizleyin.</span><span class="sxs-lookup"><span data-stu-id="af85a-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![Kullanıcıların Kullanıcı adı ve parola seçeneğini girmesi gerekir.](media/users-must-enter-username.png)

5. <span data-ttu-id="af85a-119">**Tamam**'a tıklayın.</span><span class="sxs-lookup"><span data-stu-id="af85a-119">Click **OK**.</span></span> <span data-ttu-id="af85a-120">Seçtiğiniz hesabın parolasını girmeniz ve onaylamanız istenecektir.</span><span class="sxs-lookup"><span data-stu-id="af85a-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="af85a-121">**Tamam** 'a tıklayarak işlemi sonlandırın.</span><span class="sxs-lookup"><span data-stu-id="af85a-121">Click **OK** to finish.</span></span> <span data-ttu-id="af85a-122">Windows 10 ' un sonraki başlatılışında, seçtiğiniz hesapta otomatik olarak oturum açılır.</span><span class="sxs-lookup"><span data-stu-id="af85a-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
