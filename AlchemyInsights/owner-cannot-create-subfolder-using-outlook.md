---
title: Sahibi Outlook kullanarak alt klasör oluşturamaz
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: 2116bb837e4378ea29d7882df1d3010b3a4e0b1c
ms.sourcegitcommit: 936330b11fec49f6174eadea6c765bdf9e6ba784
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/12/2020
ms.locfileid: "44749236"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="6b378-102">Sahibi Outlook kullanarak alt klasör oluşturamaz</span><span class="sxs-lookup"><span data-stu-id="6b378-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="6b378-103">**Outlook'u kullanarak alt klasörler oluşturan ortak klasör sahiplerinin devam eden bir sorunu var. Sorun yakında giderilecektir.**</span><span class="sxs-lookup"><span data-stu-id="6b378-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="6b378-104">Bu arada, aşağıdaki geçici çözümlerden birini kullanın:</span><span class="sxs-lookup"><span data-stu-id="6b378-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="6b378-105">Sorun yalnızca masaüstü pencereleri için Outlook'u etkilediğiiçin alt klasörü oluşturmak için MAC için Outlook'u kullanın (tüm sürümler)</span><span class="sxs-lookup"><span data-stu-id="6b378-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="6b378-106">Yöneticiexo Shell veya EAC kullanarak alt klasörü oluşturma</span><span class="sxs-lookup"><span data-stu-id="6b378-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="6b378-107">Kullanıcıdaki VarsayılanKamuKlasörPosta Kutusu/EfektifKamuFolderMailbox'ı, soruna neden olan klasör için İçerik Posta Kutusu'ndan başka bir posta kutusuna değiştirme</span><span class="sxs-lookup"><span data-stu-id="6b378-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="6b378-108">*Set-Posta Kutusu Kullanıcı1 VarsayılanKamuKlasörPosta Kutusu PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="6b378-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="6b378-109">Bir saat bekleyin, outlook istemcisini yeniden başlatın</span><span class="sxs-lookup"><span data-stu-id="6b378-109">Wait for an hour, restart outlook client</span></span>