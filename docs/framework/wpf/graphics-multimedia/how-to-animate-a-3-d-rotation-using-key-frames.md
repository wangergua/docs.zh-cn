---
title: 如何：使用关键帧对三维旋转进行动画处理
ms.date: 03/30/2017
helpviewer_keywords:
- animation [WPF], 3-D translations [WPF], with key frames (Rotation3DAnimation)
- key frames [WPF], Rotation3DAnimation
- 3-D translations [WPF], animating [WPF], with key frames (Rotation3DAnimation)
ms.assetid: 6f671b95-7f30-4836-9a4f-aeb7dc30121f
ms.openlocfilehash: e72ec94f830f0f5001a77e7492aa1326a47b309d
ms.sourcegitcommit: 558d78d2a68acd4c95ef23231c8b4e4c7bac3902
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/09/2019
ms.locfileid: "59297988"
---
# <a name="how-to-animate-a-3-d-rotation-using-key-frames"></a>如何：使用关键帧对三维旋转进行动画处理
在以下示例中，<xref:System.Windows.Media.Animation.Rotation3DAnimationUsingKeyFrames>用于使三维旋转进行动画处理的旋转轴，从而导致"原因"时对象。 此动画使用以下关键帧：  
  
1. <xref:System.Windows.Media.Animation.LinearRotation3DKeyFrame> 用于创建值之间的平滑的线性插值。  
  
2. <xref:System.Windows.Media.Animation.DiscreteRotation3DKeyFrame> 用于之间创建突然"跳跃"的值 （没有内插法）。  
  
3. <xref:System.Windows.Media.Animation.SplineRotation3DKeyFrame> 用于创建具体取决于值之间的变量转换<xref:System.Windows.Media.Animation.SplineRotation3DKeyFrame.KeySpline%2A>属性。 在下面的示例中，此部分动画启动较慢，但是即将结束的时间段，以指数方式加速。  
  
## <a name="example"></a>示例  
 [!code-xaml[Animation3DGallery_snip#Rotation3DAnimationUsingKeyFramesExampleWholePage](~/samples/snippets/csharp/VS_Snippets_Wpf/Animation3DGallery_snip/CS/Rotation3DAnimationUsingKeyFramesExample.xaml#rotation3danimationusingkeyframesexamplewholepage)]  
  
## <a name="see-also"></a>请参阅

- [三维图形概述](3-d-graphics-overview.md)
- [关键帧动画概述](key-frame-animations-overview.md)
- [使用情节提要对三维旋转进行动画处理](how-to-animate-a-3-d-rotation-using-storyboards.md)
- [使用 Rotation3DAnimation 对三维旋转进行动画处理](how-to-animate-a-3-d-rotation-using-rotation3danimation.md)
- [使用四元数对三维旋转进行动画处理](how-to-animate-a-3-d-rotation-using-quaternions.md)
- [使用关键帧对三维旋转进行动画处理 (QuaternionAnimationUsingKeyFrames)](animate-a-3-d-rotation-quaternionanimationusingkeyframes.md)
