---
title: 如何：在渐变中使用系统颜色
ms.date: 03/30/2017
helpviewer_keywords:
- gradients [WPF], system colors in
- system colors in gradients [WPF]
ms.assetid: 11942e7e-6300-4b50-8ed1-f50e8d20e7d2
ms.openlocfilehash: 55c99640907a0c372f8c7bbc50b9b45c9f15ef3c
ms.sourcegitcommit: 5b6d778ebb269ee6684fb57ad69a8c28b06235b9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2019
ms.locfileid: "59229435"
---
# <a name="how-to-use-system-colors-in-a-gradient"></a>如何：在渐变中使用系统颜色
若要在渐变中使用系统颜色，请使用 *\<SystemColor >* 颜色和 *\<SystemColor >* ColorKey 静态属性<xref:System.Windows.SystemColors>类来获取对颜色，引用其中 *\<SystemColor >* 是所需的系统颜色的名称。 使用 *\<SystemColor >* ColorKey 属性时想要创建的动态引用，随着系统主题变化而自动更新。 否则，请使用 *\<SystemColor >* Color 属性。  
  
## <a name="example"></a>示例  
 以下示例使用动态系统颜色资源创建渐变。  
  
 [!code-xaml[brushsamples_snip#GraphicsMMDynamicSystemColorGradientExampleWholePage](~/samples/snippets/csharp/VS_Snippets_Wpf/brushsamples_snip/CS/DynamicSystemColorExample.xaml#graphicsmmdynamicsystemcolorgradientexamplewholepage)]  
  
 下一个示例使用静态系统颜色资源创建渐变。  
  
 [!code-xaml[brushsamples_snip#GraphicsMMStaticSystemColorGradientExampleWholePage](~/samples/snippets/csharp/VS_Snippets_Wpf/brushsamples_snip/CS/StaticSystemColorExample.xaml#graphicsmmstaticsystemcolorgradientexamplewholepage)]  
  
## <a name="see-also"></a>请参阅

- <xref:System.Windows.SystemColors>
- [使用系统画笔绘制区域](how-to-paint-an-area-with-a-system-brush.md)
- [使用纯色和渐变进行绘制概述](painting-with-solid-colors-and-gradients-overview.md)
