---
title: 在 ASP.NET Core 中授权简介
author: rick-anderson
description: 了解授权以及授权 ASP.NET Core 应用中的工作方式的基础知识。
ms.author: riande
ms.date: 10/14/2016
uid: security/authorization/introduction
ms.openlocfilehash: b5e60b3c256941fff5e54e1a02e077c34c535902
ms.sourcegitcommit: 79850db9e79b1705b89f466c6f2c961ff15485de
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/07/2020
ms.locfileid: "75693864"
---
# <a name="introduction-to-authorization-in-aspnet-core"></a>在 ASP.NET Core 中授权简介

<a name="security-authorization-introduction"></a>

授权是指确定用户可执行的操作的过程。 例如，允许管理用户创建文档库、添加文档、编辑文档和删除文档。 使用库的非管理用户仅获得读取文档的权限。

授权与身份验证相互独立。 但是，授权需要一种身份验证机制。 身份验证是认定用户的过程。 身份验证可为当前用户创建一个或多个标识。

有关 ASP.NET Core 中的身份验证的详细信息，请参阅 <xref:security/authentication/index>。

## <a name="authorization-types"></a>授权类型

ASP.NET Core 授权提供一个简单、 声明性[角色](xref:security/authorization/roles)以及丰富[基于策略的](xref:security/authorization/policies)模型。 授权在要求中表示，而处理程序根据要求评估用户的声明。 命令式检查可以基于简单的策略或策略，这些策略可评估用户尝试访问的资源的用户标识和属性。

## <a name="namespaces"></a>命名空间

授权组件（包括 `AuthorizeAttribute` 和 `AllowAnonymousAttribute` 属性）位于 `Microsoft.AspNetCore.Authorization` 命名空间中。

请查阅有关[简单授权](xref:security/authorization/simple)的文档。
