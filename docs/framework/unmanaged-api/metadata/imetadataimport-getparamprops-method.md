---
title: IMetaDataImport::GetParamProps 方法
ms.date: 03/30/2017
api_name:
- IMetaDataImport.GetParamProps
api_location:
- mscoree.dll
api_type:
- COM
f1_keywords:
- IMetaDataImport::GetParamProps
helpviewer_keywords:
- IMetaDataImport::GetParamProps method [.NET Framework metadata]
- GetParamProps method [.NET Framework metadata]
ms.assetid: 4d5e5f00-bcab-4f41-b191-176511a186a7
topic_type:
- apiref
author: mairaw
ms.author: mairaw
ms.openlocfilehash: 95850448504fd863f2726a7fb7574436476a6dc5
ms.sourcegitcommit: 3d5d33f384eeba41b2dff79d096f47ccc8d8f03d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/04/2018
---
# <a name="imetadataimportgetparamprops-method"></a>IMetaDataImport::GetParamProps 方法
获取指定的 ParamDef 标记所引用的参数的元数据值。  
  
## <a name="syntax"></a>语法  
  
```  
HRESULT GetParamProps (  
   [in]  mdParamDef      tk,  
   [out] mdMethodDef     *pmd,  
   [out] ULONG           *pulSequence,  
   [out] LPWSTR          szName,  
   [in]  ULONG           cchName,  
   [out] ULONG           *pchName,  
   [out] DWORD           *pdwAttr,  
   [out] DWORD           *pdwCPlusTypeFlag,  
   [out] UVCP_CONSTANT   *ppValue,  
   [out] ULONG           *pcchValue  
);  
```  
  
#### <a name="parameters"></a>参数  
 `tk`  
 [in]表示要返回的元数据的参数的 ParamDef 标记。  
  
 `pmd`  
 [out]指向表示采用参数的方法的 MethodDef 标记的指针。  
  
 `pulSequence`  
 [out]参数的方法自变量列表中的序号位置。  
  
 `szName`  
 [out]一个缓冲区来存放参数的名称。  
  
 `cchName`  
 [in]请求的大小以宽字符为单位`szName`。  
  
 `pchName`  
 [out]在宽字符为单位返回的大小`szName`。  
  
 `pdwAttr`  
 [out]指向任何与参数相关联的属性标志的指针。  
  
 `pdwCPlusTypeFlag`  
 [out]该参数是指向该标志指定的指针<xref:System.ValueType>。  
  
 `ppValue`  
 [out]指向返回由参数的常量字符串的指针。  
  
 `pcchValue`  
 [out]大小`ppValue`以宽字符数或为零`ppValue`不包含一个字符串。  
  
## <a name="requirements"></a>要求  
 **平台：**请参阅[系统要求](../../../../docs/framework/get-started/system-requirements.md)。  
  
 **标头：** Cor.h  
  
 **库：**作为 MsCorEE.dll 中的资源  
  
 **.NET framework 版本：** [!INCLUDE[net_current_v10plus](../../../../includes/net-current-v10plus-md.md)]  
  
## <a name="see-also"></a>请参阅  
 [IMetaDataImport 接口](../../../../docs/framework/unmanaged-api/metadata/imetadataimport-interface.md)  
 [IMetaDataImport2 接口](../../../../docs/framework/unmanaged-api/metadata/imetadataimport2-interface.md)
