---
title: OneDrive başlatılırken 0x8004de40 hatası
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
- "6886"
- "9003837"
ms.openlocfilehash: f689fcf9432e9b356843efe73ed0f79a32735e6f
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/30/2020
ms.locfileid: "48823121"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a><span data-ttu-id="6b85e-102">OneDrive başlatılırken 0x8004de40 hatası</span><span class="sxs-lookup"><span data-stu-id="6b85e-102">0x8004de40 error when launching OneDrive</span></span>

<span data-ttu-id="6b85e-103">OneDrive 'da oturum açarken bir hata **0x8004de40** alırsanız, iş veya okul etki alanınıza bağlıyken bilgisayarı yeniden başlatın.</span><span class="sxs-lookup"><span data-stu-id="6b85e-103">If you receive an error **0x8004de40** when  logging into OneDrive, reboot the computer while connected to your work or school domain.</span></span> <span data-ttu-id="6b85e-104">Yeniden başlattıktan sonra bu hatayı alıyorsanız, iş veya okul etki alanınıza bağlıyken bunu deneyin:</span><span class="sxs-lookup"><span data-stu-id="6b85e-104">If you receive this error after rebooting, try this while connected to your work or school domain:</span></span>

1. <span data-ttu-id="6b85e-105">Başlat 'a tıklayın, arama kutusuna **cmd** veya **komut istemi**  yazın, komut istemi uygulamasına sağ tıklayın ve  **yönetici olarak çalıştır** 'ı seçin.</span><span class="sxs-lookup"><span data-stu-id="6b85e-105">Click Start, and type **cmd** or **command prompt**  in the search  box, right-click on the command prompt app, and select  **Run as administrator** .</span></span> <span data-ttu-id="6b85e-106">Yönetici parolası veya onaylamanız istenirse, parolayı yazın veya **Izin ver** 'i tıklatın.</span><span class="sxs-lookup"><span data-stu-id="6b85e-106">If you are prompted for an administrator password or for a confirmation, type the password, or click **Allow** .</span></span>  

2. <span data-ttu-id="6b85e-107">Komut Istemi penceresinde **dsregcmd/Leave**  yazın ve komutun tamamlanmasını bekleyin.</span><span class="sxs-lookup"><span data-stu-id="6b85e-107">In the Command Prompt window, type **dsregcmd /leave**  and wait for the command to complete.</span></span> <span data-ttu-id="6b85e-108">Ardından **dsregcmd/Join** yazın ve komutun tamamlanmasını bekleyin.</span><span class="sxs-lookup"><span data-stu-id="6b85e-108">Then type **dsregcmd /join** and wait for the command to complete.</span></span>
3. <span data-ttu-id="6b85e-109">Bilgisayarınızı yeniden başlatın.</span><span class="sxs-lookup"><span data-stu-id="6b85e-109">Reboot your computer.</span></span>
