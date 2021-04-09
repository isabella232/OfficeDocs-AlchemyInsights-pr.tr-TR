---
title: OneDrive 0x8004de40 hatasını düzeltme
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 0edb3e19b5dea240c9f2846dc503e65d92113cb7
ms.sourcegitcommit: 477cce131dc4a3c212ab18a8763a50b2f3bb20b1
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/09/2021
ms.locfileid: "51649768"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="b54d0-102">OneDrive 0x8004de40 hatasını düzeltme</span><span class="sxs-lookup"><span data-stu-id="b54d0-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="b54d0-103">Windows 7 çalıştırıyorsanız ve bu hatayı alıyorsanız Windows'ta WinHTTP'da varsayılan güvenli protokol olarak [TLS 1.1 ve TLS 1.2'yi](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)etkinleştirmek için güncelleştirin.</span><span class="sxs-lookup"><span data-stu-id="b54d0-103">If you're running Windows 7 and receive this error, [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).</span></span>

<span data-ttu-id="b54d0-104">Windows 10 çalıştırsanız ve OneDrive ile ilgili bir 0x8004de40 hatası alırsanız:</span><span class="sxs-lookup"><span data-stu-id="b54d0-104">If you're running Windows 10, and you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="b54d0-105">Acitve Dizini etki alanınıza bağlıyken etkilenen bilgisayarı yeniden başlatın.</span><span class="sxs-lookup"><span data-stu-id="b54d0-105">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="b54d0-106">Yeniden başlatma bu sorunu çöze çözeni, cihazınızı Azure AD'den açın ve yeniden başlatın.</span><span class="sxs-lookup"><span data-stu-id="b54d0-106">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="b54d0-107">**Not:** Bu adımları gerçekleştirirken şirket ağınıza bağlanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="b54d0-107">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="b54d0-108">Şirket altyapınıza bağlı değilken (örneğin seyahat ederken) bu adımları gerçekleştirin.</span><span class="sxs-lookup"><span data-stu-id="b54d0-108">Don't perform these steps when you aren't connected to your corporate infrastructure (for example, while traveling).</span></span> 

1. <span data-ttu-id="b54d0-109">Başlat öğesini seçerek yükseltilmiş bir komut istemi  **açın,** Komut İstemi'ne sağ tıklayın ve ardından Yönetici olarak çalıştır **'ı seçin.**</span><span class="sxs-lookup"><span data-stu-id="b54d0-109">Open an elevated command prompt by selecting **Start**, right-click **Command Prompt**, and then select **Run as administrator**.</span></span>

1. <span data-ttu-id="b54d0-110">*dsregcmd /leave yazın ve* Enter tuşuna **basın.**</span><span class="sxs-lookup"><span data-stu-id="b54d0-110">Type *dsregcmd /leave* and press **Enter**.</span></span>

1. <span data-ttu-id="b54d0-111">Tamamlandığında, *dsregcmd /join yazın ve* Enter tuşuna **basın.**</span><span class="sxs-lookup"><span data-stu-id="b54d0-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>

1. <span data-ttu-id="b54d0-112">Tamamlandığında, komut istemini kapatın.</span><span class="sxs-lookup"><span data-stu-id="b54d0-112">When complete, close the command prompt.</span></span>

1. <span data-ttu-id="b54d0-113">Bilgisayarı yeniden başlatın ve OneDrive'da oturum açın.</span><span class="sxs-lookup"><span data-stu-id="b54d0-113">Reboot the computer, and log into OneDrive.</span></span>