---
title: Sanal Office'OneDrive'Windows yükleme
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: 226bd24a955f6165969102c8cf00cf45da537ee05a5363c74f1dfd055d922e1d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028636"
---
# <a name="install-office-and-onedrive-on-windows-virtual-desktop"></a>Sanal Office'OneDrive'Windows yükleme

1. [Asıl VHD görüntüsünü hazırlama ve özelleştirme.](https://docs.microsoft.com/azure/virtual-desktop/set-up-customize-master-image) Henüz oluşturulmamışsa bir sanal makine (VM) oluşturun.

1. [Paylaşılan Office etkinleştirme modunda yükleme](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-office-in-shared-computer-activation-mode). Paylaşılan bilgisayar etkinleştirmesi, birden çok kullanıcının postanıza erişmelerine Office.

1. [Makine OneDrive modunda yükleme .](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-onedrive-in-per-machine-mode) Genellikle OneDrive kullanıcı başına yüklenir, ancak burada her makineye yüklenmiş olması gerekir.