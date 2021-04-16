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
# <a name="0x8004de40-error-when-launching-onedrive"></a>0x8004de40 başlatma hatası

OneDrive'da **oturum 0x8004de40** bir hata iletisi alırsanız, iş veya okul etki alanınıza bağlıyken bilgisayarı yeniden başlatın. Yeniden başlattıktan sonra bu hatayı alırsanız, iş veya okul etki alanınıza bağlıyken bunu deneyin:

1. Başlat'a tıklayın, arama **kutusuna** **cmd** veya komut istemi yazın, komut istemi uygulamasına sağ tıklayın ve Yönetici olarak **çalıştır'ı seçin.** Yönetici parolası veya onay istenirse parolayı yazın veya İzin Ver'e **tıklayın.**  

2. Komut İstemi penceresinde, **dsregcmd /leave**  yazın ve komutun tamamlanacak şekilde beklemelerini bekleyin. Ardından **dsregcmd /join** yazın ve komutun tamamlansın.
3. Bilgisayarınızı yeniden başlatın.
