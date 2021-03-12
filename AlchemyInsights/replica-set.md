---
title: Çoğaltma kümesi
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "9004395"
- "8265"
- "9276"
ms.openlocfilehash: 3834696ff59b7e96e90a5b660a489003dfa9729c
ms.sourcegitcommit: 581c696ec108184adae9d4bc8f47cb9247131de8
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714587"
---
# <a name="replica-set"></a><span data-ttu-id="9a18e-102">Çoğaltma kümesi</span><span class="sxs-lookup"><span data-stu-id="9a18e-102">Replica set</span></span>

<span data-ttu-id="9a18e-103">AADDS, yönetilen etki alanı olarak da adlandırılan bir etki alanıdır.</span><span class="sxs-lookup"><span data-stu-id="9a18e-103">AADDS is also called as the managed domain.</span></span> <span data-ttu-id="9a18e-104">Aslında, arka uç tarafından çalıştır ve bakımını yapılan iki etki alanı denetleyicisidir.</span><span class="sxs-lookup"><span data-stu-id="9a18e-104">It is actually two domain controllers that are run and maintained by the backend.</span></span> <span data-ttu-id="9a18e-105">İki DC bir ana DC ve bir çoğaltma DC içerir.</span><span class="sxs-lookup"><span data-stu-id="9a18e-105">The two DCs include one main DC and one replication DC.</span></span> <span data-ttu-id="9a18e-106">AADDS'de (yönetilen etki alanı) yedeklemeler, Azure platformu tarafından yönetilen otomatik bir işlemdir.</span><span class="sxs-lookup"><span data-stu-id="9a18e-106">Backups in AADDS (managed domain) are an automated process managed by the Azure platform.</span></span> <span data-ttu-id="9a18e-107">Yönetilen etki alanınız ile ilgili bir sorun varsa, Azure desteği yedeklemeden geri yüklemede size yardımcı olabilir.</span><span class="sxs-lookup"><span data-stu-id="9a18e-107">In the event of an issue with your managed domain, Azure support can assist you in restoring from backup.</span></span>

<span data-ttu-id="9a18e-108">Sanal bir ağda her çoğaltma kümesi oluşturabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="9a18e-108">You create each replica set in a virtual network.</span></span> <span data-ttu-id="9a18e-109">Her sanal ağ, yönetilen bir etki alanının çoğaltma kümesi barındıran diğer tüm sanal ağlara eş olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="9a18e-109">Each virtual network must be peered to every other virtual network that hosts a managed domain's replica set.</span></span> <span data-ttu-id="9a18e-110">Bu yapılandırma, dizin çoğaltmayı destekleyen bir ağ ağı topolojisi oluşturur.</span><span class="sxs-lookup"><span data-stu-id="9a18e-110">This configuration creates a mesh network topology that supports directory replication.</span></span> <span data-ttu-id="9a18e-111">Her çoğaltma kümesi farklı bir sanal alt ağda yer alan sanal ağ, birden çok çoğaltma kümesini destekleyenin.</span><span class="sxs-lookup"><span data-stu-id="9a18e-111">A virtual network can support multiple replica sets, provided that each replica set is in a different virtual subnet.</span></span>

<span data-ttu-id="9a18e-112">Çoğaltma kümesi hakkında daha fazla ayrıntı için, Kavramlar Çoğaltma [kümelerini gözden geçirin.](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets)</span><span class="sxs-lookup"><span data-stu-id="9a18e-112">For more details on Replica set, see [Concepts Replica sets](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets).</span></span>
