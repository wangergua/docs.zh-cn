---
title: 创建表达式列
ms.date: 03/30/2017
dev_langs:
- csharp
- vb
ms.assetid: 0af3bd64-92a2-4b47-ae62-f5df35f131a6
ms.openlocfilehash: 6e19e4e7cc0ea92e9d93e45c2a50d009e46b78c5
ms.sourcegitcommit: 5b6d778ebb269ee6684fb57ad69a8c28b06235b9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2019
ms.locfileid: "59175495"
---
# <a name="creating-expression-columns"></a>创建表达式列
您可以为列定义表达式，让它能够包含根据同一行中其他列值或根据表中多行的列值计算而得的值。 要定义要计算的表达式，可使用目标列的 <xref:System.Data.DataColumn.Expression%2A> 属性，并使用 <xref:System.Data.DataColumn.ColumnName%2A> 属性在表达式中引用其他列。 用于表达式列的 <xref:System.Data.DataColumn.DataType%2A> 必须适合于表达式将返回的值。  
  
 下表列出了表中表达式列的几种可能用法。  
  
|表达式类型|示例|  
|---------------------|-------------|  
|比较|"总 > = 500"|  
|计算|"UnitPrice * Quantity"|  
|聚合|Sum(Price)|  
  
 可以设置**表达式**上的现有属性**DataColumn**对象，或者您可以将该属性用作第三个参数传递给<xref:System.Data.DataColumn>构造函数，如下面的示例中所示。  
  
```vb  
workTable.Columns.Add("Total",Type.GetType("System.Double"))  
workTable.Columns.Add("SalesTax", Type.GetType("System.Double"), _  
  "Total * 0.086")  
```  
  
```csharp  
workTable.Columns.Add("Total", typeof(Double));  
workTable.Columns.Add("SalesTax", typeof(Double), "Total * 0.086");  
```  
  
 表达式可以引用其他表达式列，但循环引用（其中两个表达式相互引用）将产生异常。 有关编写表达式的规则，请参阅<xref:System.Data.DataColumn.Expression%2A>的属性**DataColumn**类。  
  
## <a name="see-also"></a>请参阅

- <xref:System.Data.DataColumn>
- <xref:System.Data.DataSet>
- <xref:System.Data.DataTable>
- [数据表架构定义](../../../../../docs/framework/data/adonet/dataset-datatable-dataview/datatable-schema-definition.md)
- [DataTables](../../../../../docs/framework/data/adonet/dataset-datatable-dataview/datatables.md)
- [ADO.NET 托管提供程序和 DataSet 开发人员中心](https://go.microsoft.com/fwlink/?LinkId=217917)
