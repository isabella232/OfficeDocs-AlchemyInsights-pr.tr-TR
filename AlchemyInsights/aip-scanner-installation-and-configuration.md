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
# <a name="aip-scanner-installation-and-configuration"></a>AIP tarayıcı: kurulum ve yapılandırma

**AIP tarayıcısını yüklemek için önerilen yönergeleri izleyin:**

1. Yükseltme yapıyorsanız ve temiz bir yükleme gerçekleştirmiyorsanız, lütfen Azure [Bilgi Koruması tarayıcısını yükseltme](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) yönergelerini izlediğinizi ve birleşik etiketleme [istemcisi için Azure Bilgi Koruması tarayıcısını yükseltmeye](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner)bakın.
2. Tüm Güvenlik Duvarları [ve ağ altyapısı ayarları gereksinimlerine](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure)uyduğunuzdan doğrulayın.
3. [İlkelerinizin](https://docs.microsoft.com/azure/information-protection/configure-policy) otomatik etiketlemeye ayarlandıktan veya ilkede varsayılan etiket olduğundan emin olun.
4. Azure [Bilgi Koruması istemcisi tarafından desteklenen Dosya türlerinde](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection)açıklandığı şekilde ilgili dosya türünün etiket/koruma için yapılandırıldığından emin olun. Ayrıca, varsayılan davranışı değiştirmek istiyorsanız, şu yönergeleri izleyin: [Dosyaların varsayılan koruma düzeyini değiştirme.](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files)
5. Tarayıcı hizmetini çalıştırmak üzere yapılandırılan kullanıcı hesabının, yapılandırılan tüm depolara erişmek için izinlere sahip olduğunu doğrulayın.
6. Hala sorunlarla karşılaşırsanız, lütfen tarayıcı günlüklerini dışa aktarın ve destek biletinize ekleyin.

**Azure Bilgi Koruma Tarayıcı günlüklerini dışa aktarma**

1. Tarayıcı hizmetini çalıştıran kullanıcı bağlamı altında %localappdata%\Microsoft\MSIP'e gidin.
2. MSIP klasörünün altındaki tüm içeriği zip.
3. Günlükleri seçtiğiniz konuma kaydedin ve servis isteğinize takın.
4. [Ayrıca Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps)kullanabilirsiniz.

**Daha fazla bilgi için bkz:**
- [Dosyaları otomatik olarak sınıflandırmak ve korumak için Azure Bilgi Koruma tarayıcısını dağıtma](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [Set-AIPAuthentication için Belirtin ve Belirtin](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [Tarayıcı için bir keşif döngüsü çalıştırma ve raporları görüntüleme](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [Azure Bilgi Koruması belgelerini gözden geçirin](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Azure Bilgi Koruması Gereksinimleri](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Azure Bilgi Koruması istemcisi indirin](https://www.microsoft.com/download/details.aspx?id=53018)
