---
ms.openlocfilehash: 3f553f95941eaf36cf335e9765a670a05bd157f4
ms.sourcegitcommit: 5b6d778ebb269ee6684fb57ad69a8c28b06235b9
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2019
ms.locfileid: "59234110"
---
### <a name="appdomainsetupdynamicbase-is-no-longer-randomized-by-userandomizedstringhashalgorithm"></a>UseRandomizedStringHashAlgorithm 不再由 AppDomainSetup.DynamicBase 进行随机化

|   |   |
|---|---|
|详细信息|在 .NET Framework 4.6 之前，如果在应用的配置文件中启用了 UseRandomizedStringHashAlgorithm，那么 <xref:System.AppDomainSetup.DynamicBase> 的值会在应用程序域或者进程之间进行随机化。 自 .NET Framework 4.6 起，<xref:System.AppDomainSetup.DynamicBase> 将在运行的应用的不同实例之间，以及在不同的应用域之间返回一个稳定的结果。 不同应用的动态基各不相同；此更改仅删除相同应用的不同实例的随机命名元素。|
|建议|请注意，启用 <code>UseRandomizedStringHashAlgorithm</code> 不会导致随机化 <xref:System.AppDomainSetup.DynamicBase>。 如果需要随机基，则必须在应用代码中生成它，而不是通过此 API 生成。|
|范围|边缘|
|版本|4.6|
|类型|运行时|
|受影响的 API|<ul><li><xref:System.AppDomainSetup.DynamicBase?displayProperty=nameWithType></li></ul>|
