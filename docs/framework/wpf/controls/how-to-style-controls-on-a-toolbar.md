---
title: 如何：设置 ToolBar 上的控件的样式
ms.date: 03/30/2017
helpviewer_keywords:
- styling controls on toolbar [WPF]
- toolbars [WPF]
- customizing controls on toolbar [WPF]
ms.assetid: ba6ae056-d6a9-4c24-90f8-467ab0bc0b1a
ms.openlocfilehash: cc5ac9dd64072c34ff999255a27dd92f311cda0f
ms.sourcegitcommit: 3d5d33f384eeba41b2dff79d096f47ccc8d8f03d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/04/2018
---
# <a name="how-to-style-controls-on-a-toolbar"></a>如何：设置 ToolBar 上的控件的样式
<xref:System.Windows.Controls.ToolBar>定义<xref:System.Windows.ResourceKey>对象来指定内的控件的样式<xref:System.Windows.Controls.ToolBar>。  若要在为控件设置样式<xref:System.Windows.Controls.ToolBar>，将其设置`x:key`到样式属性<xref:System.Windows.ResourceKey>中定义<xref:System.Windows.Controls.ToolBar>。  
  
 <xref:System.Windows.Controls.ToolBar>定义了以下<xref:System.Windows.ResourceKey>对象：  
  
-   <xref:System.Windows.Controls.ToolBar.ButtonStyleKey%2A>  
  
-   <xref:System.Windows.Controls.ToolBar.CheckBoxStyleKey%2A>  
  
-   <xref:System.Windows.Controls.ToolBar.ComboBoxStyleKey%2A>  
  
-   <xref:System.Windows.Controls.ToolBar.MenuStyleKey%2A>  
  
-   <xref:System.Windows.Controls.ToolBar.RadioButtonStyleKey%2A>  
  
-   <xref:System.Windows.Controls.ToolBar.SeparatorStyleKey%2A>  
  
-   <xref:System.Windows.Controls.ToolBar.TextBoxStyleKey%2A>  
  
-   <xref:System.Windows.Controls.ToolBar.ToggleButtonStyleKey%2A>  
  
## <a name="example"></a>示例  
 下面的示例定义内的控件的样式<xref:System.Windows.Controls.ToolBar>。  
  
 [!code-xaml[ToolBar_snip#ToolBarAllStyles](../../../../samples/snippets/csharp/VS_Snippets_Wpf/ToolBar_snip/CS/pane1.xaml#toolbarallstyles)]  
[!code-xaml[ToolBar_snip#ToolBar](../../../../samples/snippets/csharp/VS_Snippets_Wpf/ToolBar_snip/CS/pane1.xaml#toolbar)]  
  
## <a name="see-also"></a>请参阅  
 [样式设置和模板化](../../../../docs/framework/wpf/controls/styling-and-templating.md)
