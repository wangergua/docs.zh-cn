---
title: <type1>'<typename>必须实现<membername>for interface<interfacename>
ms.date: 07/20/2015
f1_keywords:
- vbc30154
- bc30154
helpviewer_keywords:
- BC30154
ms.assetid: 259afdfa-3608-4760-adcb-88ec0da5020d
ms.openlocfilehash: 86b0d46e0e27b2fd8d1fccb37f4a3c45e95f5f63
ms.sourcegitcommit: 558d78d2a68acd4c95ef23231c8b4e4c7bac3902
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/09/2019
ms.locfileid: "59295323"
---
# <a name="type1typename-must-implement-membername-for-interface-interfacename"></a>\<类型 1 >\<类型名称 > 必须实现\<成员名称 > 接口\<interfacename >
'\<类型名称 > 必须实现\<成员名称 > 接口\<interfacename >。 实现属性必须具有匹配的 ReadOnly / WriteOnly 说明符。  
  
 类或结构声明实现一个接口，但不实现过程、 属性或事件的接口定义。 必须实现该接口的每个成员。  
  
 **错误 ID:** BC30154  
  
## <a name="to-correct-this-error"></a>更正此错误  
  
1. 声明具有相同名称和签名，因为在接口中定义的成员。 请务必包括至少`End Function`， `End Sub`，或`End Property`语句。  
  
2. 添加`Implements`子句的末尾`Function`， `Sub`， `Property`，或`Event`语句。 例如：  
  
    ```  
    Public Event ItHappened() Implements IBaseInterface.ItHappened  
    ```  
  
3. 当实现属性，请确保`ReadOnly`或`WriteOnly`使用如下所示的接口定义的方式相同。  
  
4. 当实现属性，将声明`Get`和`Set`过程，根据需要。  
  
## <a name="see-also"></a>请参阅

- [Implements 语句](../../../visual-basic/language-reference/statements/implements-statement.md)
- [接口](../../../visual-basic/programming-guide/language-features/interfaces/index.md)
