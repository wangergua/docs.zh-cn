---
title: 使用 SerializationBinder 控制序列化和反序列化
ms.date: 03/30/2017
ms.assetid: ba8dcecf-acc7-467c-939d-021bbac797d4
ms.openlocfilehash: cb2476b55a965e326e492c3c0b77f0be65b2b290
ms.sourcegitcommit: 5b6d778ebb269ee6684fb57ad69a8c28b06235b9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2019
ms.locfileid: "59198525"
---
# <a name="controlling-serialization-and-deserialization-with-serializationbinder"></a>使用 SerializationBinder 控制序列化和反序列化
在序列化过程中，格式化程序传输创建正确类型和版本的对象实例时所需的信息。 此信息通常包括对象的完整类型名称和程序集名称。 默认情况下，反序列化可使用此信息创建相同对象的实例。 由于原始类可能在执行反序列化的计算机上不存在，原始类已在程序集之间移动，或者服务器和客户端要求使用不同的类版本，因此有些用户可能需要控制要序列化和反序列化哪个类。 有关详细信息，请参阅[序列化联编程序使用情况](../../../../docs/framework/wcf/samples/usage-of-serialization-binder.md)。  
  
> [!WARNING]
>  此功能仅在使用 <xref:System.Runtime.Serialization.Formatters.Binary.BinaryFormatter> 或 <xref:System.Runtime.Serialization.NetDataContractSerializer> 时可用。  
  
## <a name="using-serializationbinder"></a>使用 SerializationBinder  
 <xref:System.Runtime.Serialization.SerializationBinder> 是一个抽象类，用于控制在序列化和反序列化过程中使用的实际类型。 若要控制在序列化和反序列化期间使用的类型，请从 <xref:System.Runtime.Serialization.SerializationBinder> 派生一个类，并重写 <xref:System.Runtime.Serialization.SerializationBinder.BindToName(System.Type,System.String@,System.String@)> 和 <xref:System.Runtime.Serialization.SerializationBinder.BindToType(System.String,System.String)> 方法。 <xref:System.Runtime.Serialization.SerializationBinder.BindToName(System.Type,System.String@,System.String@)> 方法采用 <xref:System.Type>，并返回程序集名称和类型名称。 <xref:System.Runtime.Serialization.SerializationBinder.BindToType(System.String,System.String)> 方法采用程序集名称和类型名称，并返回 <xref:System.Type>。  
  
## <a name="see-also"></a>请参阅

- [序列化和反序列化](../../../../docs/framework/wcf/feature-details/serialization-and-deserialization.md)
- [序列化联编程序的用法](../../../../docs/framework/wcf/samples/usage-of-serialization-binder.md)
