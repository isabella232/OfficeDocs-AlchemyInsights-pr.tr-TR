---
title: 'Hata: Bu bilgisayarınızın kuralları eş eşşş değil'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c46eb856baafbef9bc3b7fa34a0258ef16923fb8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51782972"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="4fec1-102">Hata: Bu bilgisayarınızın kuralları eş eşşş değil</span><span class="sxs-lookup"><span data-stu-id="4fec1-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="4fec1-103">Bu bilinen sorunun güncelleştirilmiş durumunu görmek için bkz. Bu bilgisayarda kuralların [Microsoft Exchange'in kurallarıyla eşleşmedi](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span><span class="sxs-lookup"><span data-stu-id="4fec1-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="4fec1-104">Outlook Ekibi Derleme 12928.10000'de bir düzeltme uygulamaya başladı.</span><span class="sxs-lookup"><span data-stu-id="4fec1-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="4fec1-105">Düzeltme zaten Insider Hızlı için ve Haziran 2020'nin sonlarında Aylık Kanala geç gelecektir.</span><span class="sxs-lookup"><span data-stu-id="4fec1-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="4fec1-106">Düzeltilen derlemeyi elde ettiyken son kez "Hangi kuralları tutmak istediğiniz" istemini alabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="4fec1-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="4fec1-107">Sorulsa Sunucu'ya gidin, Outlook'a geri gidin ve devre dışı bırakılmış olan tüm kuralları yeniden etkinleştirin.</span><span class="sxs-lookup"><span data-stu-id="4fec1-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="4fec1-108">Düzeltme kullanılabilir olana kadar lütfen aşağıdaki geçici çözümü kullanın:</span><span class="sxs-lookup"><span data-stu-id="4fec1-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="4fec1-109">**Geçici** çözüm : Son raporlarda, bu sorun yalnızca Outlook masaüstünde istemci kuralı oluşturanların ortaya çıktı.</span><span class="sxs-lookup"><span data-stu-id="4fec1-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="4fec1-110">Soruna neden olmaya devam ediyorsanız, kuralları silmeyi ve sonra sorun çözülene kadar yalnızca OWA'da (Outlook Web App) kural oluşturma ve düzenlemeyi göz önünde bulundurabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="4fec1-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="4fec1-111">Kuralları el ile silemezsiniz, Outlook'u başlatmak için /cleanrules komutunu Outlook.exe Outlook komutunu çalıştırabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="4fec1-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="4fec1-112">Bu hem istemci hem de sunucu kurallarını siler.</span><span class="sxs-lookup"><span data-stu-id="4fec1-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="4fec1-113">Outlook Profilinde yer alan tüm hesaplar için kuralların hepsini siler.</span><span class="sxs-lookup"><span data-stu-id="4fec1-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="4fec1-114">Bu komut, Komut satırı anahtarları makalesinde daha ayrıntılı belgelanmıştır.</span><span class="sxs-lookup"><span data-stu-id="4fec1-114">This command is further documented in the Command-line switches article.</span></span>

