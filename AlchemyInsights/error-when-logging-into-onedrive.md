---
title: 0x8004de40 başlatma hatası
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
- "6886"
- "9003837"
ms.openlocfilehash: e329d7fe881a0fc9514584e06aa2d6e8ebab5b11
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813672"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a><span data-ttu-id="7133d-102">0x8004de40 başlatma hatası</span><span class="sxs-lookup"><span data-stu-id="7133d-102">0x8004de40 error when launching OneDrive</span></span>

<span data-ttu-id="7133d-103">OneDrive'da **oturum 0x8004de40** bir hata iletisi alırsanız, iş veya okul etki alanınıza bağlıyken bilgisayarı yeniden başlatın.</span><span class="sxs-lookup"><span data-stu-id="7133d-103">If you receive an error **0x8004de40** when  logging into OneDrive, reboot the computer while connected to your work or school domain.</span></span> <span data-ttu-id="7133d-104">Yeniden başlattıktan sonra bu hatayı alırsanız, iş veya okul etki alanınıza bağlıyken bunu deneyin:</span><span class="sxs-lookup"><span data-stu-id="7133d-104">If you receive this error after rebooting, try this while connected to your work or school domain:</span></span>

1. <span data-ttu-id="7133d-105">Başlat'a tıklayın, arama **kutusuna** **cmd** veya komut istemi yazın, komut istemi uygulamasına sağ tıklayın ve Yönetici olarak **çalıştır'ı seçin.**</span><span class="sxs-lookup"><span data-stu-id="7133d-105">Click Start, and type **cmd** or **command prompt**  in the search  box, right-click on the command prompt app, and select  **Run as administrator**.</span></span> <span data-ttu-id="7133d-106">Yönetici parolası veya onay istenirse parolayı yazın veya İzin Ver'e **tıklayın.**</span><span class="sxs-lookup"><span data-stu-id="7133d-106">If you are prompted for an administrator password or for a confirmation, type the password, or click **Allow**.</span></span>  

2. <span data-ttu-id="7133d-107">Komut İstemi penceresinde, **dsregcmd /leave**  yazın ve komutun tamamlanacak şekilde beklemelerini bekleyin.</span><span class="sxs-lookup"><span data-stu-id="7133d-107">In the Command Prompt window, type **dsregcmd /leave**  and wait for the command to complete.</span></span> <span data-ttu-id="7133d-108">Ardından **dsregcmd /join** yazın ve komutun tamamlansın.</span><span class="sxs-lookup"><span data-stu-id="7133d-108">Then type **dsregcmd /join** and wait for the command to complete.</span></span>
3. <span data-ttu-id="7133d-109">Bilgisayarınızı yeniden başlatın.</span><span class="sxs-lookup"><span data-stu-id="7133d-109">Reboot your computer.</span></span>
