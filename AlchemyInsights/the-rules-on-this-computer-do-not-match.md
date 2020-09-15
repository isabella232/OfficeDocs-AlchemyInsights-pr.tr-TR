---
title: 'Hata: Bu bilgisayardaki kurallar uyuşmuyor'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c2feb6da651d8b3eb7af6a057335b28d26f9e7f6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690983"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="0e394-102">Hata: Bu bilgisayardaki kurallar uyuşmuyor</span><span class="sxs-lookup"><span data-stu-id="0e394-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="0e394-103">Bu bilinen sorunun güncelleştirilmiş durumunu görmek için, [Bu bilgisayardaki kuralların Microsoft Exchange 'deki kurallarla eşleşmediğini](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0) görün</span><span class="sxs-lookup"><span data-stu-id="0e394-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="0e394-104">Outlook ekibi, derleme 12928,10000 ' te bir düzeltme uygulamıştır.</span><span class="sxs-lookup"><span data-stu-id="0e394-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="0e394-105">Düzeltme zaten Insider 'dan hızlıdır ve 2020 Haziran 'da aylık kanala gider.</span><span class="sxs-lookup"><span data-stu-id="0e394-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="0e394-106">Sabit yapıya sahip olduktan sonra "hangi kuralları korumak istiyorsunuz" istemini son kez alabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="0e394-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="0e394-107">İstendiğinde sunucu 'yu seçin ve ardından Outlook 'a geri dönün ve devre dışı bırakılmış kuralları yeniden etkinleştirin.</span><span class="sxs-lookup"><span data-stu-id="0e394-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="0e394-108">Düzeltme mevcut olana kadar aşağıdaki geçici çözümü kullanın:</span><span class="sxs-lookup"><span data-stu-id="0e394-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="0e394-109">**Geçici çözüm**: son raporlarda, sorun yalnızca Outlook masaüstü 'nde istemci kuralları oluşturmuş olanlar için ortaya çıktı.</span><span class="sxs-lookup"><span data-stu-id="0e394-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="0e394-110">Sorun devam ederseniz, kuralları silin ve sonra sorun giderilinceye kadar yalnızca OWA (Outlook Web App) kurallarını oluşturup düzenleyin.</span><span class="sxs-lookup"><span data-stu-id="0e394-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="0e394-111">Kuralları el ile silemsem Outlook 'U başlattığınızda Outlook.exe/cleankurallarını çalıştırarak Outlook komutunu çalıştırabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="0e394-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="0e394-112">Bu, hem istemci hem de sunucu kurallarını silecek.</span><span class="sxs-lookup"><span data-stu-id="0e394-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="0e394-113">Outlook profilindeki tüm hesapların tüm kurallarını silecek.</span><span class="sxs-lookup"><span data-stu-id="0e394-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="0e394-114">Bu komut, komut satırı anahtarları makalesinde daha da belgelenmiştir.</span><span class="sxs-lookup"><span data-stu-id="0e394-114">This command is further documented in the Command-line switches article.</span></span>

