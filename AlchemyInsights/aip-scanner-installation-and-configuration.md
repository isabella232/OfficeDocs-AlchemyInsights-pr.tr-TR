---
title: 'AIP tarayıcı: yükleme ve yapılandırma'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5119"
ms.openlocfilehash: c32f3f10e2e17cf67e73ec8404be293eeefb68a3
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821683"
---
# <a name="aip-scanner-installation-and-configuration"></a><span data-ttu-id="530c7-102">AIP tarayıcı: yükleme ve yapılandırma</span><span class="sxs-lookup"><span data-stu-id="530c7-102">AIP scanner: installation and configuration</span></span>

<span data-ttu-id="530c7-103">**AIP tarayıcısını yüklemek için önerilen yönergeleri izleyin:**</span><span class="sxs-lookup"><span data-stu-id="530c7-103">**To install the AIP scanner, follow the recommended guidelines**:</span></span>

1. <span data-ttu-id="530c7-104">Yükseltme yapıyorsanız ve temiz bir yükleme gerçekleştire değilken, [Azure Information Protection tarayıcısını](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) ve birleşik etiket istemcisini yükseltme yönergelerini takip ediyorsanız, bkz. Azure Information Protection [tarayıcısını yükseltme](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span><span class="sxs-lookup"><span data-stu-id="530c7-104">If you are upgrading and not performing a clean installation, please make sure you have followed the guidelines for [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) and for unified labeling client, see [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span></span>
2. <span data-ttu-id="530c7-105">Tüm Güvenlik Duvarları ve ağ [altyapısı ayarları gereksinimlerine uyarak uyumlu olduğunu doğrulayın.](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure)</span><span class="sxs-lookup"><span data-stu-id="530c7-105">Verify that you comply with all [Firewalls and network infrastructure settings requirements](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).</span></span>
3. <span data-ttu-id="530c7-106">İlkelerinizin [otomatik etiketlemeye](https://docs.microsoft.com/azure/information-protection/configure-policy) ayar olduğundan veya ilkede varsayılan bir etiketin olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="530c7-106">Make sure your [policies are set](https://docs.microsoft.com/azure/information-protection/configure-policy) to automatic labeling or have a default label in the policy.</span></span>
4. <span data-ttu-id="530c7-107">Azure Information Protection istemcisi tarafından desteklenen Dosya türleri konusunda açıklandığı gibi, ilgili dosya türünün etiket/koruma [için yapılandırıldığından emin olun.](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection)</span><span class="sxs-lookup"><span data-stu-id="530c7-107">Make sure that the relevant file type is configured for label/protection as described in [File types supported by the Azure Information Protection client](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection).</span></span> <span data-ttu-id="530c7-108">Ayrıca, varsayılan davranışı değiştirmek de istemiyorsanız şu yönergeleri izleyin: [Dosyaların varsayılan koruma düzeyini değiştirme](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span><span class="sxs-lookup"><span data-stu-id="530c7-108">In addition, if you want to change the default behavior, follow these guidelines: [Changing the default protection level of files](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span></span>
5. <span data-ttu-id="530c7-109">Tarayıcı hizmetini çalıştıracak şekilde yapılandırılmış kullanıcı hesabının, yapılandırılmış tüm depolara erişim izinleri olduğunu doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="530c7-109">Verify that the user account configured to run the scanner service has permissions to access all the configured repositories.</span></span>
6. <span data-ttu-id="530c7-110">Sorun halen devam ediyorsanız, lütfen tarayıcı günlüklerini dışarı aktarın ve bunları destek biletinize ekleyin.</span><span class="sxs-lookup"><span data-stu-id="530c7-110">If you still experience issues, please export the scanner logs and add them to your support ticket.</span></span>

<span data-ttu-id="530c7-111">**Azure Information Protection Tarayıcı günlüklerini dışarı aktarma**</span><span class="sxs-lookup"><span data-stu-id="530c7-111">**Export Azure Information Protection Scanner logs**</span></span>

1. <span data-ttu-id="530c7-112">Tarayıcı hizmetini çalıştıran kullanıcı bağlamının altında %localappdata%\Microsoft\MSIP klasörüne gidin.</span><span class="sxs-lookup"><span data-stu-id="530c7-112">Navigate to %localappdata%\Microsoft\MSIP under the user context running the scanner service.</span></span>
2. <span data-ttu-id="530c7-113">MSIP klasörünün altındaki tüm içeriği sıkıştırın.</span><span class="sxs-lookup"><span data-stu-id="530c7-113">Zip all the contents under the MSIP folder.</span></span>
3. <span data-ttu-id="530c7-114">Günlükleri tercih konumunuzla kaydedin ve hizmet isteğinize iliştirin.</span><span class="sxs-lookup"><span data-stu-id="530c7-114">Save the logs to your choice of location, and attach them to your service request.</span></span>
4. <span data-ttu-id="530c7-115">[Export-AIPLogs -OnBehalfOf da kullanabilirsiniz.](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps)</span><span class="sxs-lookup"><span data-stu-id="530c7-115">You can also use [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span></span>

<span data-ttu-id="530c7-116">**Ek bilgi için bkz:**</span><span class="sxs-lookup"><span data-stu-id="530c7-116">**For additional information, see**:</span></span>
- [<span data-ttu-id="530c7-117">Dosyaları otomatik olarak sınıflandırmak ve korumak için Azure Information Protection tarayıcısını dağıtma</span><span class="sxs-lookup"><span data-stu-id="530c7-117">Deploying the Azure Information Protection scanner to automatically classify and protect files</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [<span data-ttu-id="530c7-118">Set-AIPAuthentication için Token parametresini belirtme ve kullanma</span><span class="sxs-lookup"><span data-stu-id="530c7-118">Specify and use the Token parameter for Set-AIPAuthentication</span></span>](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [<span data-ttu-id="530c7-119">Tarayıcı için bir keşif döngüsü çalıştırma ve raporları görüntüleme</span><span class="sxs-lookup"><span data-stu-id="530c7-119">Run a discovery cycle and view reports for the scanner</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [<span data-ttu-id="530c7-120">Azure Information Protection belgelerini gözden geçirme</span><span class="sxs-lookup"><span data-stu-id="530c7-120">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="530c7-121">Azure Information Protection gereksinimleri</span><span class="sxs-lookup"><span data-stu-id="530c7-121">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [<span data-ttu-id="530c7-122">Azure Information Protection istemcisini indirin</span><span class="sxs-lookup"><span data-stu-id="530c7-122">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)
