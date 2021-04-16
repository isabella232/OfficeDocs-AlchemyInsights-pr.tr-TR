---
title: Windows 10'da parmak izi kilidi açma seçeneğini kullanma
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
- "9001689"
- "3765"
ms.openlocfilehash: ba1f2e7b0bb54e89178a320b8579b8d1bfdaff9a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51796697"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a><span data-ttu-id="45ff5-102">Windows 10'da parmak izi kilidi açma seçeneğini kullanma</span><span class="sxs-lookup"><span data-stu-id="45ff5-102">Use fingerprint unlock option in Windows 10</span></span>

<span data-ttu-id="45ff5-103">**Windows Hello Parmak İzi Tanımayı Etkinleştirme**</span><span class="sxs-lookup"><span data-stu-id="45ff5-103">**Enable Windows Hello Fingerprint**</span></span>

<span data-ttu-id="45ff5-104">Windows 10'un kilidini parmak izinizi kullanarak açmak için windows hello parmak izi kilidini en az bir parmağınızı ekleyerek (Windows'un tanımasını öğrenmesine izin vererek) ayarlamanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="45ff5-104">To unlock Windows 10 using your fingerprint, you need to set up Windows Hello Fingerprint by adding (letting Windows learn to recognize) at least one finger.</span></span> 

1. <span data-ttu-id="45ff5-105">Oturum açma **seçenekleri > Hesaplar ve > ayarlar'a gidin (veya** buraya [tıklayın).](ms-settings:signinoptions?activationSource=GetHelp)</span><span class="sxs-lookup"><span data-stu-id="45ff5-105">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="45ff5-106">Kullanılabilir oturum açma seçenekleri listelenir.</span><span class="sxs-lookup"><span data-stu-id="45ff5-106">Available sign-in options will be listed.</span></span> <span data-ttu-id="45ff5-107">Örneğin:</span><span class="sxs-lookup"><span data-stu-id="45ff5-107">For example:</span></span>

    ![Oturum açma seçenekleri.](media/sign-in-options.png)

2. <span data-ttu-id="45ff5-109">Windows Hello Parmak **İzi Tanıma'ya tıklayın veya** dokunun, ardından Ayarla **öğesine tıklayın.**</span><span class="sxs-lookup"><span data-stu-id="45ff5-109">Click or tap **Windows Hello Fingerprint**, then click **Set up**.</span></span> <span data-ttu-id="45ff5-110">Windows Hello kurulum penceresinde, Başla **'ya tıklayın.**</span><span class="sxs-lookup"><span data-stu-id="45ff5-110">In the Windows Hello setup window, click **Get started**.</span></span> <span data-ttu-id="45ff5-111">Parmak izi algılayıcısı etkin hale gelecektir ve parmağınızı algılayıcıya şu şekilde koyabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="45ff5-111">The fingerprint sensor will activate, and you'll be asked to place your finger on the sensor:</span></span>

   ![Parmak izi algılayıcısı.](media/fingerprint-sensor.png)

3. <span data-ttu-id="45ff5-113">Parmağınızı tekrar tekrar taramanızı soracak şekilde yönergeleri izleyin.</span><span class="sxs-lookup"><span data-stu-id="45ff5-113">Follow the instructions, which will ask you to repeatedly scan your finger.</span></span> <span data-ttu-id="45ff5-114">Bu tamamlandığında, oturum açma için kullanmak istediğiniz diğer parmaklarınızı ekleme seçeneğiniz olur.</span><span class="sxs-lookup"><span data-stu-id="45ff5-114">When this is finished, you'll have the option of adding other fingers you may want to use for sign-in.</span></span> <span data-ttu-id="45ff5-115">Windows 10'da bir sonraki oturum açsanız, bu şekilde parmak izinizi kullanma seçeneğiniz olur.</span><span class="sxs-lookup"><span data-stu-id="45ff5-115">Next time you sign in to Windows 10, you will have the option of using your fingerprint to do so.</span></span>

<span data-ttu-id="45ff5-116">**Windows Hello Parmak İzi Tanıma oturum açma seçeneği olarak kullanılamıyor**</span><span class="sxs-lookup"><span data-stu-id="45ff5-116">**Windows Hello Fingerprint not available as a sign-in option**</span></span>

<span data-ttu-id="45ff5-117">Oturum açma seçeneklerinde Windows Hello Parmak İzi İşareti seçeneği gösterilmiyorsa, Windows bilgisayarınıza bağlı herhangi bir parmak izi okuyucusu/tarayıcısı farkında değildir veya sistem ilkesi bunun kullanımını engellemektedir (örneğin, bilgisayarınız çalışma alanınız tarafından yönetiliyorsa).</span><span class="sxs-lookup"><span data-stu-id="45ff5-117">If Windows Hello Fingerprint is not shown as an option in **Sign-in options**, it means Windows is not aware of any fingerprint reader/scanner attached to your PC, or that a system policy prevents its use (if for example your PC is managed by your workplace).</span></span> <span data-ttu-id="45ff5-118">Sorun gidermek için:</span><span class="sxs-lookup"><span data-stu-id="45ff5-118">To troubleshoot:</span></span> 

1. <span data-ttu-id="45ff5-119">Görev çubuğunda **Başlangıç** düğmesini seçin ve Cihaz **Yöneticisi'ni arayın.**</span><span class="sxs-lookup"><span data-stu-id="45ff5-119">Select the **Start** button in the Taskbar and search for **Device Manager**.</span></span>

2. <span data-ttu-id="45ff5-120">Cihaz Yöneticisi'ni açmak için **öğesine tıklayın veya dokunun.**</span><span class="sxs-lookup"><span data-stu-id="45ff5-120">Click or tap to open **Device Manager**.</span></span>

3. <span data-ttu-id="45ff5-121">Cihaz Yöneticisi'nde, Biyometrik cihazları köşeli çift ayraçlarına tıklayarak genişletin.</span><span class="sxs-lookup"><span data-stu-id="45ff5-121">In Device Manager, expand Biometric devices by clicking its chevron.</span></span>

   ![Biyometrik cihazlar.](media/biometric-devices.png)

4. <span data-ttu-id="45ff5-123">Parmak izi tarayıcınız Synaptics WBDI tarayıcı gibi biyometrik bir cihaz olarak listelenmiş olmalı:</span><span class="sxs-lookup"><span data-stu-id="45ff5-123">Your fingerprint scanner should be listed as a biometric device, such as the Synaptics WBDI scanner:</span></span>

   ![Biyometrik cihazlar.](media/biometric-devices-expanded.png)

5. <span data-ttu-id="45ff5-125">Parmak izi tarayıcınızın gösterilmezse ve tarayıcı bilgisayarınızla tümleşikse, bilgisayar üreticisinin web sitesine gidin.</span><span class="sxs-lookup"><span data-stu-id="45ff5-125">If your fingerprint scanner is not shown, and the scanner is integrated into your PC, go to the PC manufacturer's website.</span></span> <span data-ttu-id="45ff5-126">Bilgisayar modelinize uygun teknik destek bölümünde, yük makineniz olan bir tarayıcı için Windows 10 sürücüsü aratırsınız.</span><span class="sxs-lookup"><span data-stu-id="45ff5-126">In the technical support section for your PC model, search for a Windows 10 driver for a scanner that you can install.</span></span>

6. <span data-ttu-id="45ff5-127">Tarayıcı pc'den ayrı ise (USB ile takılı) sahip olduğunuz tarayıcı modeline uygun Windows 10 cihaz sürücüsü yazılımını bulmak ve yüklemek için tarayıcı üreticisinin web sitesine gidin.</span><span class="sxs-lookup"><span data-stu-id="45ff5-127">If the scanner is separate from the PC (attached via USB), go to the scanner manufacturer's website to find and install Windows 10 device driver software for the scanner model you have.</span></span>
