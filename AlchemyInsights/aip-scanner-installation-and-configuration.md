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
# <a name="aip-scanner-installation-and-configuration"></a>AIP tarayıcı: yükleme ve yapılandırma

**AIP tarayıcısını yüklemek için önerilen yönergeleri izleyin:**

1. Yükseltme yapıyorsanız ve temiz bir yükleme gerçekleştire değilken, [Azure Information Protection tarayıcısını](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) ve birleşik etiket istemcisini yükseltme yönergelerini takip ediyorsanız, bkz. Azure Information Protection [tarayıcısını yükseltme](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).
2. Tüm Güvenlik Duvarları ve ağ [altyapısı ayarları gereksinimlerine uyarak uyumlu olduğunu doğrulayın.](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure)
3. İlkelerinizin [otomatik etiketlemeye](https://docs.microsoft.com/azure/information-protection/configure-policy) ayar olduğundan veya ilkede varsayılan bir etiketin olduğundan emin olun.
4. Azure Information Protection istemcisi tarafından desteklenen Dosya türleri konusunda açıklandığı gibi, ilgili dosya türünün etiket/koruma [için yapılandırıldığından emin olun.](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection) Ayrıca, varsayılan davranışı değiştirmek de istemiyorsanız şu yönergeleri izleyin: [Dosyaların varsayılan koruma düzeyini değiştirme](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).
5. Tarayıcı hizmetini çalıştıracak şekilde yapılandırılmış kullanıcı hesabının, yapılandırılmış tüm depolara erişim izinleri olduğunu doğrulayın.
6. Sorun halen devam ediyorsanız, lütfen tarayıcı günlüklerini dışarı aktarın ve bunları destek biletinize ekleyin.

**Azure Information Protection Tarayıcı günlüklerini dışarı aktarma**

1. Tarayıcı hizmetini çalıştıran kullanıcı bağlamının altında %localappdata%\Microsoft\MSIP klasörüne gidin.
2. MSIP klasörünün altındaki tüm içeriği sıkıştırın.
3. Günlükleri tercih konumunuzla kaydedin ve hizmet isteğinize iliştirin.
4. [Export-AIPLogs -OnBehalfOf da kullanabilirsiniz.](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps)

**Ek bilgi için bkz:**
- [Dosyaları otomatik olarak sınıflandırmak ve korumak için Azure Information Protection tarayıcısını dağıtma](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [Set-AIPAuthentication için Token parametresini belirtme ve kullanma](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [Tarayıcı için bir keşif döngüsü çalıştırma ve raporları görüntüleme](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [Azure Information Protection belgelerini gözden geçirme](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Azure Information Protection gereksinimleri](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Azure Information Protection istemcisini indirin](https://www.microsoft.com/download/details.aspx?id=53018)
