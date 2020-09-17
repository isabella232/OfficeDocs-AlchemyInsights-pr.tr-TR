---
title: Windows 10 ' da parmak izi kilidini kullanma seçeneğini kullanma
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
- "9001689"
- "3765"
ms.openlocfilehash: 99f037f62748c06d77b526e35f67b711885c4a1e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47795264"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a><span data-ttu-id="e58a6-102">Windows 10 ' da parmak izi kilidini kullanma seçeneğini kullanma</span><span class="sxs-lookup"><span data-stu-id="e58a6-102">Use fingerprint unlock option in Windows 10</span></span>

<span data-ttu-id="e58a6-103">**Windows Hello parmak Izini etkinleştirme**</span><span class="sxs-lookup"><span data-stu-id="e58a6-103">**Enable Windows Hello Fingerprint**</span></span>

<span data-ttu-id="e58a6-104">Parmak izinizi kullanarak Windows 10 ' un kilidini açmak için, en az bir parmağınızı ekleyerek (Windows 'un tanıyacağı konusunda izin vererek) Windows Hello parmak Izini ayarlamanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="e58a6-104">To unlock Windows 10 using your fingerprint, you need to set up Windows Hello Fingerprint by adding (letting Windows learn to recognize) at least one finger.</span></span> 

1. <span data-ttu-id="e58a6-105">**> hesap > oturum açma seçenekleri** 'ne gidin (veya [burayı](ms-settings:signinoptions?activationSource=GetHelp)tıklatın).</span><span class="sxs-lookup"><span data-stu-id="e58a6-105">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="e58a6-106">Kullanılabilir oturum açma seçenekleri listelenir.</span><span class="sxs-lookup"><span data-stu-id="e58a6-106">Available sign-in options will be listed.</span></span> <span data-ttu-id="e58a6-107">Örneğin:</span><span class="sxs-lookup"><span data-stu-id="e58a6-107">For example:</span></span>

    ![Oturum açma seçenekleri.](media/sign-in-options.png)

2. <span data-ttu-id="e58a6-109">**Windows Hello parmak izi**'ne tıklayın veya dokunun, ardından **Ayarla**'ya tıklayın.</span><span class="sxs-lookup"><span data-stu-id="e58a6-109">Click or tap **Windows Hello Fingerprint**, then click **Set up**.</span></span> <span data-ttu-id="e58a6-110">Windows Hello kurulumu **penceresinde başlayın 'ı tıklatın.**</span><span class="sxs-lookup"><span data-stu-id="e58a6-110">In the Windows Hello setup window, click **Get started**.</span></span> <span data-ttu-id="e58a6-111">Parmak izi algılayıcısı etkinleştirilir ve parmağınızı algılayıcının üzerine yerleştirmenizi istenecektir:</span><span class="sxs-lookup"><span data-stu-id="e58a6-111">The fingerprint sensor will activate, and you'll be asked to place your finger on the sensor:</span></span>

   ![Parmak izi algılayıcısı.](media/fingerprint-sensor.png)

3. <span data-ttu-id="e58a6-113">Parmağınızı izleyerek parmağınızı sürekli taramanızı ister.</span><span class="sxs-lookup"><span data-stu-id="e58a6-113">Follow the instructions, which will ask you to repeatedly scan your finger.</span></span> <span data-ttu-id="e58a6-114">Bu tamamlandığında, oturum açmak için kullanmak isteyebileceğiniz başka parmağınızı ekleme seçeneğiniz olur.</span><span class="sxs-lookup"><span data-stu-id="e58a6-114">When this is finished, you'll have the option of adding other fingers you may want to use for sign-in.</span></span> <span data-ttu-id="e58a6-115">Windows 10 ' da bir sonraki oturum açışınızda, parmak izinizi kullanarak bunu yapabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="e58a6-115">Next time you sign in to Windows 10, you will have the option of using your fingerprint to do so.</span></span>

<span data-ttu-id="e58a6-116">**Windows Hello Parmak Izi oturum açma seçeneği olarak kullanılamaz**</span><span class="sxs-lookup"><span data-stu-id="e58a6-116">**Windows Hello Fingerprint not available as a sign-in option**</span></span>

<span data-ttu-id="e58a6-117">Windows Hello Parmak Izi **oturum açma seçeneklerinde**bir seçenek olarak gösterilmiyorsa, Windows 'un bilgisayarınıza bağlı parmak izi okuyucusunun/tarayıcısının farkında olmadığı veya sistem ilkesinin kullanımını engellediğini (ÖRNEĞIN, PC 'niz iş yeriniz tarafından yönetiliyorsa).</span><span class="sxs-lookup"><span data-stu-id="e58a6-117">If Windows Hello Fingerprint is not shown as an option in **Sign-in options**, it means Windows is not aware of any fingerprint reader/scanner attached to your PC, or that a system policy prevents its use (if for example your PC is managed by your workplace).</span></span> <span data-ttu-id="e58a6-118">Sorun gidermek için:</span><span class="sxs-lookup"><span data-stu-id="e58a6-118">To troubleshoot:</span></span> 

1. <span data-ttu-id="e58a6-119">Görev çubuğundaki **Başlat** düğmesini seçin ve **Cihaz Yöneticisi 'ni**arayın.</span><span class="sxs-lookup"><span data-stu-id="e58a6-119">Select the **Start** button in the Taskbar and search for **Device Manager**.</span></span>

2. <span data-ttu-id="e58a6-120">**Aygıt Yöneticisi 'ni**açmak için tıklayın veya dokunun.</span><span class="sxs-lookup"><span data-stu-id="e58a6-120">Click or tap to open **Device Manager**.</span></span>

3. <span data-ttu-id="e58a6-121">Aygıt Yöneticisi 'nde, Çift Ayraca tıklayarak biyometrik cihazları genişletin.</span><span class="sxs-lookup"><span data-stu-id="e58a6-121">In Device Manager, expand Biometric devices by clicking its chevron.</span></span>

   ![Biyometrik cihazlar.](media/biometric-devices.png)

4. <span data-ttu-id="e58a6-123">Parmak izi tarayıcınız, Synaptics ILEDI tarayıcısı gibi bir biyometrik aygıt olarak listelenmelidir:</span><span class="sxs-lookup"><span data-stu-id="e58a6-123">Your fingerprint scanner should be listed as a biometric device, such as the Synaptics WBDI scanner:</span></span>

   ![Biyometrik cihazlar.](media/biometric-devices-expanded.png)

5. <span data-ttu-id="e58a6-125">Parmak izi tarayıcınız gösterilmiyorsa ve tarayıcı bilgisayarınızla tümleşikse, bılgısayar üreticisinin Web sitesine gidin.</span><span class="sxs-lookup"><span data-stu-id="e58a6-125">If your fingerprint scanner is not shown, and the scanner is integrated into your PC, go to the PC manufacturer's website.</span></span> <span data-ttu-id="e58a6-126">PC modelinizin teknik destek bölümünde, yükleyebileceğiniz bir tarayıcı için Windows 10 sürücüsü arayın.</span><span class="sxs-lookup"><span data-stu-id="e58a6-126">In the technical support section for your PC model, search for a Windows 10 driver for a scanner that you can install.</span></span>

6. <span data-ttu-id="e58a6-127">Tarayıcı PC 'den ayrıdır (USB ile bağlı), sahip olduğunuz tarayıcı modeli için Windows 10 cihaz sürücüsü yazılımını bulmak için tarayıcı üreticisinin Web sitesine gidin.</span><span class="sxs-lookup"><span data-stu-id="e58a6-127">If the scanner is separate from the PC (attached via USB), go to the scanner manufacturer's website to find and install Windows 10 device driver software for the scanner model you have.</span></span>
