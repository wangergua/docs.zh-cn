---
title: 发生错误，因为无法获得单个实例启动所需的操作系统资源
ms.date: 07/20/2015
f1_keywords:
- vbrAppModel_CantGetMemoryMappedFile
ms.assetid: 0d9f2a30-ff72-4355-8060-744f22339359
ms.openlocfilehash: 9aa7ba0babe0a89942e320a76e07c05162b31700
ms.sourcegitcommit: 558d78d2a68acd4c95ef23231c8b4e4c7bac3902
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/09/2019
ms.locfileid: "59313601"
---
# <a name="an-unexpected-error-has-occurred-because-an-operating-system-resource-required-for-single-instance-startup-cannot-be-acquired"></a>发生错误，因为无法获得单个实例启动所需的操作系统资源
应用程序未能获取所需的操作系统资源。 一些可能导致此问题的原因是：  
  
-   应用程序不具备创建命名操作系统对象的权限。  
  
-   公共语言运行时不具备创建内存映射文件的权限。  
  
-   应用程序需要访问某个操作系统对象，但另一个进程正在使用该对象。  
  
## <a name="to-correct-this-error"></a>更正此错误  
  
1. 检查该应用程序具有创建命名操作系统对象的足够权限。  
  
2. 检查公共语言运行时具有创建内存映射文件的足够权限。  
  
3. 重新启动计算机以清除可能正使用连接到原始实例应用程序所需的资源的任何进程。  
  
4. 记录发生错误的环境，并与 Microsoft 产品支持服务联系  
  
## <a name="see-also"></a>请参阅

- [Application Page, Project Designer (Visual Basic)](/visualstudio/ide/reference/application-page-project-designer-visual-basic)
- [调试器基础知识](/visualstudio/debugger/debugger-basics)
- [Talk to Us](/visualstudio/ide/talk-to-us)
