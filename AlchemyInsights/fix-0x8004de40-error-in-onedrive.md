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
# <a name="fix-0x8004de40-error-in-onedrive"></a>OneDrive 0x8004de40 hatasını düzeltme

Windows 7 çalıştırıyorsanız ve bu hatayı alıyorsanız Windows'ta WinHTTP'da varsayılan güvenli protokol olarak [TLS 1.1 ve TLS 1.2'yi](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)etkinleştirmek için güncelleştirin.

Windows 10 çalıştırsanız ve OneDrive ile ilgili bir 0x8004de40 hatası alırsanız:

- Acitve Dizini etki alanınıza bağlıyken etkilenen bilgisayarı yeniden başlatın.
- Yeniden başlatma bu sorunu çöze çözeni, cihazınızı Azure AD'den açın ve yeniden başlatın. 

**Not:** Bu adımları gerçekleştirirken şirket ağınıza bağlanabilirsiniz. Şirket altyapınıza bağlı değilken (örneğin seyahat ederken) bu adımları gerçekleştirin. 

1. Başlat öğesini seçerek yükseltilmiş bir komut istemi  **açın,** Komut İstemi'ne sağ tıklayın ve ardından Yönetici olarak çalıştır **'ı seçin.**

1. *dsregcmd /leave yazın ve* Enter tuşuna **basın.**

1. Tamamlandığında, *dsregcmd /join yazın ve* Enter tuşuna **basın.**

1. Tamamlandığında, komut istemini kapatın.

1. Bilgisayarı yeniden başlatın ve OneDrive'da oturum açın.