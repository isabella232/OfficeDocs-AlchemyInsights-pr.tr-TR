---
title: 0x8004de40 başlatma sırasında hata OneDrive
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
ms.openlocfilehash: 23c57356c8bd94c1cbafb538c9318208429754115a7c4e88abc93d293b5ea6e1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946599"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>0x8004de40 başlatma sırasında hata OneDrive

E-postada oturum **0x8004de40** bir hata iletisi OneDrive, iş veya okul etki alanınıza bağlıyken bilgisayarı yeniden başlatın. Yeniden başlattıktan sonra bu hatayı alırsanız, iş veya okul etki alanınıza bağlıyken bunu deneyin:

1. Başlat'a tıklayın, arama **kutusuna** **cmd** veya komut istemi yazın, komut istemi uygulamasına sağ tıklayın ve Yönetici olarak **çalıştır'ı seçin.** Yönetici parolası veya onay istenirse parolayı yazın veya İzin Ver'e **tıklayın.**  

2. Komut İstemi penceresinde, **dsregcmd /leave**  yazın ve komutun tamamlanacak şekilde beklemelerini bekleyin. Ardından **dsregcmd /join** yazın ve komutun tamamlansın.
3. Bilgisayarınızı yeniden başlatın.
