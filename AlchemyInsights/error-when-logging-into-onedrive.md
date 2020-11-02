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
# <a name="0x8004de40-error-when-launching-onedrive"></a>OneDrive başlatılırken 0x8004de40 hatası

OneDrive 'da oturum açarken bir hata **0x8004de40** alırsanız, iş veya okul etki alanınıza bağlıyken bilgisayarı yeniden başlatın. Yeniden başlattıktan sonra bu hatayı alıyorsanız, iş veya okul etki alanınıza bağlıyken bunu deneyin:

1. Başlat 'a tıklayın, arama kutusuna **cmd** veya **komut istemi**  yazın, komut istemi uygulamasına sağ tıklayın ve  **yönetici olarak çalıştır** 'ı seçin. Yönetici parolası veya onaylamanız istenirse, parolayı yazın veya **Izin ver** 'i tıklatın.  

2. Komut Istemi penceresinde **dsregcmd/Leave**  yazın ve komutun tamamlanmasını bekleyin. Ardından **dsregcmd/Join** yazın ve komutun tamamlanmasını bekleyin.
3. Bilgisayarınızı yeniden başlatın.
