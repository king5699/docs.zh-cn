---
title: "如何：从已绑定的目标属性获取绑定对象"
ms.custom: 
ms.date: 03/30/2017
ms.prod: .net-framework
ms.reviewer: 
ms.suite: 
ms.technology: dotnet-wpf
ms.tgt_pltfrm: 
ms.topic: article
helpviewer_keywords:
- data binding [WPF], getting binding objects from bound target properties
- properties [WPF], getting binding objects from
ms.assetid: 87974c5f-136b-4de7-b07d-9285b62ab123
caps.latest.revision: "13"
author: dotnet-bot
ms.author: dotnetcontent
manager: wpickett
ms.workload: dotnet
ms.openlocfilehash: f5369bc770a31aa99f1fb11bfec790eb8fe091d5
ms.sourcegitcommit: 16186c34a957fdd52e5db7294f291f7530ac9d24
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/22/2017
---
# <a name="how-to-get-the-binding-object-from-a-bound-target-property"></a>如何：从已绑定的目标属性获取绑定对象
本示例演示如何从数据绑定的目标属性获取绑定对象。  
  
## <a name="example"></a>示例  
 你可以执行以下操作来获取<xref:System.Windows.Data.Binding>对象：  
  
 [!code-csharp[BindValidation#GetBinding](../../../../samples/snippets/csharp/VS_Snippets_Wpf/BindValidation/CSharp/Window1.xaml.cs#getbinding)]  
  
> [!NOTE]
>  必须为所需的绑定指定依赖属性，因为目标对象的多个属性可能正在使用数据绑定。  
  
 或者，你可以获取<xref:System.Windows.Data.BindingExpression>，然后获取的值<xref:System.Windows.Data.BindingExpression.ParentBinding%2A>属性。  
  
 有关完整示例，请参阅[绑定验证示例](http://go.microsoft.com/fwlink/?LinkID=159972)。  
  
> [!NOTE]
>  如果绑定是<xref:System.Windows.Data.MultiBinding>，使用<xref:System.Windows.Data.BindingOperations>。<xref:System.Windows.Data.BindingOperations.GetMultiBinding%2A>。 如果它是<xref:System.Windows.Data.PriorityBinding>，使用<xref:System.Windows.Data.BindingOperations>。<xref:System.Windows.Data.BindingOperations.GetPriorityBinding%2A>。 如果你不确定是否使用绑定目标属性<xref:System.Windows.Data.Binding>、 <xref:System.Windows.Data.MultiBinding>，或<xref:System.Windows.Data.PriorityBinding>，你可以使用<xref:System.Windows.Data.BindingOperations>。<xref:System.Windows.Data.BindingOperations.GetBindingBase%2A>。  
  
## <a name="see-also"></a>请参阅  
 [在代码中创建绑定](../../../../docs/framework/wpf/data/how-to-create-a-binding-in-code.md)  
 [帮助主题](../../../../docs/framework/wpf/data/data-binding-how-to-topics.md)
