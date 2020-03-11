---
title: Windows 10'da parmak izi kilidini açma seçeneğini kullanma
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001689"
- "3765"
ms.openlocfilehash: 8a5059c722c306ad79811140062cec7f52f31766
ms.sourcegitcommit: 00e4266575438f55bdc18db05ed54aafcb75a3c9
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/11/2020
ms.locfileid: "42588335"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a><span data-ttu-id="55d71-102">Windows 10'da parmak izi kilidini açma seçeneğini kullanma</span><span class="sxs-lookup"><span data-stu-id="55d71-102">Use fingerprint unlock option in Windows 10</span></span>

<span data-ttu-id="55d71-103">**Windows Hello Parmak İzini Etkinleştir**</span><span class="sxs-lookup"><span data-stu-id="55d71-103">**Enable Windows Hello Fingerprint**</span></span>

<span data-ttu-id="55d71-104">Parmak izinizi kullanarak Windows 10'un kilidini açmak için en az bir parmak ekleyerek (Windows'un tanımayı öğrenmesine izin vererek) Windows Hello Parmak İzi'ni ayarlamanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="55d71-104">To unlock Windows 10 using your fingerprint, you need to set up Windows Hello Fingerprint by adding (letting Windows learn to recognize) at least one finger.</span></span> 

1. <span data-ttu-id="55d71-105">Hesaplar **> Ayarlar>a** gidin (veya [buraya](ms-settings:signinoptions?activationSource=GetHelp)tıklayın).</span><span class="sxs-lookup"><span data-stu-id="55d71-105">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="55d71-106">Kullanılabilir oturum açma seçenekleri listelenir.</span><span class="sxs-lookup"><span data-stu-id="55d71-106">Available sign-in options will be listed.</span></span> <span data-ttu-id="55d71-107">Örneğin:</span><span class="sxs-lookup"><span data-stu-id="55d71-107">For example:</span></span>

    ![Oturum açma seçenekleri.](media/sign-in-options.png)

2. <span data-ttu-id="55d71-109">**Windows Hello Parmak İzi'ni**tıklatın veya dokunun, ardından **Ayarla'yı**tıklatın.</span><span class="sxs-lookup"><span data-stu-id="55d71-109">Click or tap **Windows Hello Fingerprint**, then click **Set up**.</span></span> <span data-ttu-id="55d71-110">Windows Hello kurulum **penceresinde, Başlat'ı**tıklatın.</span><span class="sxs-lookup"><span data-stu-id="55d71-110">In the Windows Hello setup window, click **Get started**.</span></span> <span data-ttu-id="55d71-111">Parmak izi sensörü devreye girer ve parmağınızı sensörün üzerine yerleştirmeniz istenir:</span><span class="sxs-lookup"><span data-stu-id="55d71-111">The fingerprint sensor will activate, and you'll be asked to place your finger on the sensor:</span></span>

   ![Parmak izi sensörü.](media/fingerprint-sensor.png)

3. <span data-ttu-id="55d71-113">Parmağınızı tekrar tekrar tetmenizi isteyecek olan talimatları uygulayın.</span><span class="sxs-lookup"><span data-stu-id="55d71-113">Follow the instructions, which will ask you to repeatedly scan your finger.</span></span> <span data-ttu-id="55d71-114">Bu işlem tamamlandığında, oturum açma için kullanmak isteyebileceğin diğer parmakları ekleme seçeneğiniz olur.</span><span class="sxs-lookup"><span data-stu-id="55d71-114">When this is finished, you'll have the option of adding other fingers you may want to use for sign-in.</span></span> <span data-ttu-id="55d71-115">Windows 10'da bir daha oturum açtığınızda, bunu yapmak için parmak izinizi kullanma seçeneğiniz olacaktır.</span><span class="sxs-lookup"><span data-stu-id="55d71-115">Next time you sign in to Windows 10, you will have the option of using your fingerprint to do so.</span></span>

<span data-ttu-id="55d71-116">**Windows Hello Parmak İzi oturum açma seçeneği olarak kullanılamıyor**</span><span class="sxs-lookup"><span data-stu-id="55d71-116">**Windows Hello Fingerprint not available as a sign-in option**</span></span>

<span data-ttu-id="55d71-117">Windows Hello Parmak İzi Oturum **Açma seçeneklerinde**bir seçenek olarak gösterilmiyorsa, Bu, Windows'un bilgisayarınıza bağlı herhangi bir parmak izi okuyucusunun/tarayıcısının farkında olmadığı veya bir sistem ilkesinin kullanımını engellediği anlamına gelir (örneğin bilgisayarınız işyeriniz tarafından yönetiliyorsa).</span><span class="sxs-lookup"><span data-stu-id="55d71-117">If Windows Hello Fingerprint is not shown as an option in **Sign-in options**, it means Windows is not aware of any fingerprint reader/scanner attached to your PC, or that a system policy prevents its use (if for example your PC is managed by your workplace).</span></span> <span data-ttu-id="55d71-118">Sorun gidermek için:</span><span class="sxs-lookup"><span data-stu-id="55d71-118">To troubleshoot:</span></span> 

1. <span data-ttu-id="55d71-119">Görev Çubuğu'ndaki **Başlat** düğmesini seçin ve **Aygıt Yöneticisi'ni**arayın.</span><span class="sxs-lookup"><span data-stu-id="55d71-119">Select the **Start** button in the Taskbar and search for **Device Manager**.</span></span>

2. <span data-ttu-id="55d71-120">**Aygıt Yöneticisi'ni**açmak için tıklatın veya dokunun.</span><span class="sxs-lookup"><span data-stu-id="55d71-120">Click or tap to open **Device Manager**.</span></span>

3. <span data-ttu-id="55d71-121">Device Manager'da, köşeli ayraçlarını tıklatarak Biyometrik aygıtları genişletin.</span><span class="sxs-lookup"><span data-stu-id="55d71-121">In Device Manager, expand Biometric devices by clicking its chevron.</span></span>

   ![Biyometrik cihazlar.](media/biometric-devices.png)

4. <span data-ttu-id="55d71-123">Parmak izi tarayıcınız Synaptics WBDI tarayıcısı gibi biyometrik bir aygıt olarak listelenmelidir:</span><span class="sxs-lookup"><span data-stu-id="55d71-123">Your fingerprint scanner should be listed as a biometric device, such as the Synaptics WBDI scanner:</span></span>

   ![Biyometrik cihazlar.](media/biometric-devices-expanded.png)

5. <span data-ttu-id="55d71-125">Parmak izi tarayıcınız gösterinmiyorsa ve tarayıcı bilgisayarınıza entegre edilmişse, BILGISAYAR üreticisinin web sitesine gidin.</span><span class="sxs-lookup"><span data-stu-id="55d71-125">If your fingerprint scanner is not shown, and the scanner is integrated into your PC, go to the PC manufacturer's website.</span></span> <span data-ttu-id="55d71-126">PC modelinizin teknik destek bölümünde, yükleyebileceğiniz bir tarayıcı için Windows 10 sürücüsü arayın.</span><span class="sxs-lookup"><span data-stu-id="55d71-126">In the technical support section for your PC model, search for a Windows 10 driver for a scanner that you can install.</span></span>

6. <span data-ttu-id="55d71-127">Tarayıcı bilgisayardan ayrıysa (USB üzerinden bağlıysa), sahip olduğunuz tarayıcı modeli için Windows 10 aygıt sürücüsü yazılımını bulmak ve yüklemek için tarayıcı üreticisinin web sitesine gidin.</span><span class="sxs-lookup"><span data-stu-id="55d71-127">If the scanner is separate from the PC (attached via USB), go to the scanner manufacturer's website to find and install Windows 10 device driver software for the scanner model you have.</span></span>
