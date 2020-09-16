---
title: 'Hata: önbelleğe alınan kimlik bilgilerinizin süresi dolduğundan değişikliklerinizi karşıya yükleyemiyoruz veya indiremiyoruz'
ms.author: v-miegge
author: v-miegge
manager: v-cojank
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: ''
ms.custom:
- "3534"
- "9001489"
ms.openlocfilehash: 8105fa7b311bc932f95c8bff4d6b58ed9aabe74a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734499"
---
# <a name="error-we-cant-upload-or-download-your-changes-because-your-cached-credentials-have-expired"></a><span data-ttu-id="f89f3-102">Hata: önbelleğe alınan kimlik bilgilerinizin süresi dolduğundan değişikliklerinizi karşıya yükleyemiyoruz veya indiremiyoruz</span><span class="sxs-lookup"><span data-stu-id="f89f3-102">Error: We can't upload or download your changes because your cached credentials have expired</span></span>

<span data-ttu-id="f89f3-103">Dosyaları OneDrive uygulamasına kaydederken, **"önbelleğe alınmış kimlik bilgileriniz süresi doldu"** ifadesini içeren bir hata alırsanız aşağıdaki adımları uygulayın:</span><span class="sxs-lookup"><span data-stu-id="f89f3-103">When saving files to the OneDrive app, if you receive an error that contains the phrase **"your cached credentials have expired"**, perform the following steps:</span></span>

1. <span data-ttu-id="f89f3-104">Tüm Office uygulamalarını kapatın.</span><span class="sxs-lookup"><span data-stu-id="f89f3-104">Close all Office applications.</span></span>
1. <span data-ttu-id="f89f3-105">Kimlik bilgileri Yöneticisi 'ni açın ve görev çubuğundaki arama kutusuna **kimlik bilgileri Yöneticisi** yazın, ardından **kimlik bilgileri Yöneticisi Denetim Masası**'nı seçin.</span><span class="sxs-lookup"><span data-stu-id="f89f3-105">Open Credential Manager, and type **credential manager** in the search box on the taskbar, then select **Credential Manager Control panel**.</span></span>
1. <span data-ttu-id="f89f3-106">**Windows kimlik bilgileri**'ni seçin.</span><span class="sxs-lookup"><span data-stu-id="f89f3-106">Select **Windows Credentials**.</span></span>
1. <span data-ttu-id="f89f3-107">**OneDrive**Word ile başlayan herhangi bir girişi bulun.</span><span class="sxs-lookup"><span data-stu-id="f89f3-107">Find any entry that starts with the word **OneDrive**.</span></span>
1. <span data-ttu-id="f89f3-108">Girdiyi seçip **Kaldır**'a basın.</span><span class="sxs-lookup"><span data-stu-id="f89f3-108">Select the entry, then press **Remove**.</span></span>
1. <span data-ttu-id="f89f3-109">Kimlik bilgileri Yöneticisi 'ni kapatın, ardından syıseçtiğiniz mavi buluta sağ tıklayın ve **OneDrive 'ı kapat**'ı seçin.</span><span class="sxs-lookup"><span data-stu-id="f89f3-109">Close Credential Manager, then right click on the blue cloud in your systray, and select **Close OneDrive**.</span></span>
1. <span data-ttu-id="f89f3-110">Görev çubuğundaki arama kutusuna **OneDrive** yazın ve OneDrive 'ı başlatmak Için **OneDrive uygulamasını** seçin.</span><span class="sxs-lookup"><span data-stu-id="f89f3-110">Type **OneDrive** into the search box on the taskbar and select **OneDrive App** to launch OneDrive.</span></span>
1. <span data-ttu-id="f89f3-111">OneDrive 'da oturum açın ve dosyayı OneDrive 'a kaydetmeyi deneyin.</span><span class="sxs-lookup"><span data-stu-id="f89f3-111">Sign into OneDrive, then try to save the file to OneDrive.</span></span>
