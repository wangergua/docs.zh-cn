---
title: LINQ to DataSet
ms.date: 03/30/2017
ms.assetid: 743e3755-3ecb-45a2-8d9b-9ed41f0dcf17
ms.openlocfilehash: 92be418e38039757437e6e673f39a7baef011528
ms.sourcegitcommit: 5b6d778ebb269ee6684fb57ad69a8c28b06235b9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2019
ms.locfileid: "59221777"
---
# <a name="linq-to-dataset"></a>LINQ to DataSet
[!INCLUDE[linq_dataset](../../../../includes/linq-dataset-md.md)] 可以更轻松、 更快地查询缓存中的数据<xref:System.Data.DataSet>对象。 具体而言，通过使开发人员能够使用编程语言本身而不是通过使用单独的查询语言来编写查询，[!INCLUDE[linq_dataset](../../../../includes/linq-dataset-md.md)] 可以简化查询。 这是非常适合 Visual Studio 开发人员，他们现在可以充分利用编译时语法检查、 静态类型化，并在其查询中的 Visual Studio 提供 IntelliSense 支持。  
  
 [!INCLUDE[linq_dataset](../../../../includes/linq-dataset-md.md)] 此外可对已从一个或多个数据源合并的数据执行查询。 这可以使许多需要灵活表示和处理数据的方案（例如查询本地聚合的数据和 Web 应用程序中的中间层缓存）能够实现。 具体地说，一般报告、分析和业务智能应用程序将需要这种操作方法。  
  
 [!INCLUDE[linq_dataset](../../../../includes/linq-dataset-md.md)]功能主要通过中的扩展方法公开<xref:System.Data.DataRowExtensions>和<xref:System.Data.DataTableExtensions>类。 [!INCLUDE[linq_dataset](../../../../includes/linq-dataset-md.md)] 基于并使用现有[!INCLUDE[ado_whidbey_long](../../../../includes/ado-whidbey-long-md.md)]体系结构，并不是为了替换[!INCLUDE[ado_whidbey_long](../../../../includes/ado-whidbey-long-md.md)]应用程序代码中。 现有的 ADO.NET 2.0 代码将继续在 [!INCLUDE[linq_dataset](../../../../includes/linq-dataset-md.md)] 应用程序中有效。 下图阐释了 [!INCLUDE[linq_dataset](../../../../includes/linq-dataset-md.md)] 与 [!INCLUDE[ado_whidbey_long](../../../../includes/ado-whidbey-long-md.md)] 和数据存储区的关系。  
  
 ![显示 LINQ to DataSet 基于 ADO.NET 提供程序关系图。](./media/linq-to-dataset/linq-dataset-ado-dotnet-provider.gif)  
  
## <a name="in-this-section"></a>本节内容  
 [入门](../../../../docs/framework/data/adonet/getting-started-linq-to-dataset.md)  
  
 [编程指南](../../../../docs/framework/data/adonet/programming-guide-linq-to-dataset.md)  
  
## <a name="reference"></a>参考  
 <xref:System.Data.DataTableExtensions>  
  
 <xref:System.Data.DataRowExtensions>  
  
 <xref:System.Data.DataRowComparer>  
  
## <a name="see-also"></a>请参阅

- [语言集成查询 (LINQ)-C#](../../../csharp/programming-guide/concepts/linq/index.md)
- [语言集成查询 (LINQ) 的 Visual Basic](../../../visual-basic/programming-guide/concepts/linq/index.md)
- [LINQ 和 ADO.NET](../../../../docs/framework/data/adonet/linq-and-ado-net.md)
- [ADO.NET](../../../../docs/framework/data/adonet/index.md)
