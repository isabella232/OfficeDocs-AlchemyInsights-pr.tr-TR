---
title: 'AIP tarayıcı: kurulum ve yapılandırma'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5119"
ms.openlocfilehash: d059d411aef03ca57662b71fbd7d27aecd3e0e57
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/23/2020
ms.locfileid: "44358569"
---
# <a name="aip-scanner-installation-and-configuration"></a><span data-ttu-id="887cc-102">AIP tarayıcı: kurulum ve yapılandırma</span><span class="sxs-lookup"><span data-stu-id="887cc-102">AIP scanner: installation and configuration</span></span>

<span data-ttu-id="887cc-103">**AIP tarayıcısını yüklemek için önerilen yönergeleri izleyin:**</span><span class="sxs-lookup"><span data-stu-id="887cc-103">**To install the AIP scanner, follow the recommended guidelines**:</span></span>

1. <span data-ttu-id="887cc-104">Yükseltme yapıyorsanız ve temiz bir yükleme gerçekleştirmiyorsanız, lütfen Azure [Bilgi Koruması tarayıcısını yükseltme](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) yönergelerini izlediğinizi ve birleşik etiketleme [istemcisi için Azure Bilgi Koruması tarayıcısını yükseltmeye](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner)bakın.</span><span class="sxs-lookup"><span data-stu-id="887cc-104">If you are upgrading and not performing a clean installation, please make sure you have followed the guidelines for [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) and for unified labeling client, see [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span></span>
2. <span data-ttu-id="887cc-105">Tüm Güvenlik Duvarları [ve ağ altyapısı ayarları gereksinimlerine](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure)uyduğunuzdan doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="887cc-105">Verify that you comply with all [Firewalls and network infrastructure settings requirements](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).</span></span>
3. <span data-ttu-id="887cc-106">[İlkelerinizin](https://docs.microsoft.com/azure/information-protection/configure-policy) otomatik etiketlemeye ayarlandıktan veya ilkede varsayılan etiket olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="887cc-106">Make sure your [policies are set](https://docs.microsoft.com/azure/information-protection/configure-policy) to automatic labeling or have a default label in the policy.</span></span>
4. <span data-ttu-id="887cc-107">Azure [Bilgi Koruması istemcisi tarafından desteklenen Dosya türlerinde](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection)açıklandığı şekilde ilgili dosya türünün etiket/koruma için yapılandırıldığından emin olun.</span><span class="sxs-lookup"><span data-stu-id="887cc-107">Make sure that the relevant file type is configured for label/protection as described in [File types supported by the Azure Information Protection client](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection).</span></span> <span data-ttu-id="887cc-108">Ayrıca, varsayılan davranışı değiştirmek istiyorsanız, şu yönergeleri izleyin: [Dosyaların varsayılan koruma düzeyini değiştirme.](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files)</span><span class="sxs-lookup"><span data-stu-id="887cc-108">In addition, if you want to change the default behavior, follow these guidelines: [Changing the default protection level of files](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span></span>
5. <span data-ttu-id="887cc-109">Tarayıcı hizmetini çalıştırmak üzere yapılandırılan kullanıcı hesabının, yapılandırılan tüm depolara erişmek için izinlere sahip olduğunu doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="887cc-109">Verify that the user account configured to run the scanner service has permissions to access all the configured repositories.</span></span>
6. <span data-ttu-id="887cc-110">Hala sorunlarla karşılaşırsanız, lütfen tarayıcı günlüklerini dışa aktarın ve destek biletinize ekleyin.</span><span class="sxs-lookup"><span data-stu-id="887cc-110">If you still experience issues, please export the scanner logs and add them to your support ticket.</span></span>

<span data-ttu-id="887cc-111">**Azure Bilgi Koruma Tarayıcı günlüklerini dışa aktarma**</span><span class="sxs-lookup"><span data-stu-id="887cc-111">**Export Azure Information Protection Scanner logs**</span></span>

1. <span data-ttu-id="887cc-112">Tarayıcı hizmetini çalıştıran kullanıcı bağlamı altında %localappdata%\Microsoft\MSIP'e gidin.</span><span class="sxs-lookup"><span data-stu-id="887cc-112">Navigate to %localappdata%\Microsoft\MSIP under the user context running the scanner service.</span></span>
2. <span data-ttu-id="887cc-113">MSIP klasörünün altındaki tüm içeriği zip.</span><span class="sxs-lookup"><span data-stu-id="887cc-113">Zip all the contents under the MSIP folder.</span></span>
3. <span data-ttu-id="887cc-114">Günlükleri seçtiğiniz konuma kaydedin ve servis isteğinize takın.</span><span class="sxs-lookup"><span data-stu-id="887cc-114">Save the logs to your choice of location, and attach them to your service request.</span></span>
4. <span data-ttu-id="887cc-115">[Ayrıca Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps)kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="887cc-115">You can also use [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span></span>

<span data-ttu-id="887cc-116">**Daha fazla bilgi için bkz:**</span><span class="sxs-lookup"><span data-stu-id="887cc-116">**For additional information, see**:</span></span>
- [<span data-ttu-id="887cc-117">Dosyaları otomatik olarak sınıflandırmak ve korumak için Azure Bilgi Koruma tarayıcısını dağıtma</span><span class="sxs-lookup"><span data-stu-id="887cc-117">Deploying the Azure Information Protection scanner to automatically classify and protect files</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [<span data-ttu-id="887cc-118">Set-AIPAuthentication için Belirtin ve Belirtin</span><span class="sxs-lookup"><span data-stu-id="887cc-118">Specify and use the Token parameter for Set-AIPAuthentication</span></span>](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [<span data-ttu-id="887cc-119">Tarayıcı için bir keşif döngüsü çalıştırma ve raporları görüntüleme</span><span class="sxs-lookup"><span data-stu-id="887cc-119">Run a discovery cycle and view reports for the scanner</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [<span data-ttu-id="887cc-120">Azure Bilgi Koruması belgelerini gözden geçirin</span><span class="sxs-lookup"><span data-stu-id="887cc-120">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="887cc-121">Azure Bilgi Koruması Gereksinimleri</span><span class="sxs-lookup"><span data-stu-id="887cc-121">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [<span data-ttu-id="887cc-122">Azure Bilgi Koruması istemcisi indirin</span><span class="sxs-lookup"><span data-stu-id="887cc-122">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)
