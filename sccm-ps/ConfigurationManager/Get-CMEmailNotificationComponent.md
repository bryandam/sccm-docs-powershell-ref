<<<<<<< HEAD
---
title: Get-CMEmailNotificationComponent
titleSuffix: Configuration Manager
description: Gets an email notification components.
ms.date: 05/02/2019
ms.prod: configuration-manager
ms.technology: configmgr-other
ms.topic: conceptual
author: aczechowski
ms.author: aaroncz
manager: dougeby
=======
﻿---
external help file: AdminUI.PS.HS.dll-Help.xml
ms.assetid: B1E83113-4742-40EC-A78F-EC46C8C50A5E
online version: https://go.microsoft.com/fwlink/?linkid=833672
schema: 2.0.0
>>>>>>> master
---

# Get-CMEmailNotificationComponent

## SYNOPSIS
Gets an email notification components.

## SYNTAX

```
Get-CMEmailNotificationComponent [-SiteSystemServerName <String>] [-SiteCode <String>]
 [-DisableWildcardHandling] [-ForceWildcardHandling] [<CommonParameters>]
```

## DESCRIPTION
The **Get-CMEmailNotificationComponent** cmdlet gets one or more email notification components Microsoft System Center Configuration Manager.

## EXAMPLES

> [!NOTE]
> Configuration Manager CmdLets must be run from the Configuration Manager site drive. For more information, see the [getting started documentation](https://docs.microsoft.com/powershell/sccm/overview).


### Example 1: Get an email notification component by using a site code
```
PS XYZ:\> Get-CMEmailNotificationComponent -SiteCode "CM2"
```

This command gets a notification component for the site that has the site code CM2.

### Example 2: Get an email notification component by using a site system server name
```
PS XYZ:\> Get-CMEmailNotificationComponent -SiteSystemServerName "CMCEN-DIST02.TSQA.CORP.CONTOSCO.COM"
```

This command gets a notification component for the site that has the server that has the specified name.

## PARAMETERS

### -DisableWildcardHandling
DisableWildcardHandling treats wildcard characters as literal character values. Cannot be combined with **ForceWildcardHandling**.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ForceWildcardHandling
ForceWildcardHandling processes wildcard characters and may lead to unexpected behavior (not recommended). Cannot be combined with **DisableWildcardHandling**.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SiteCode
Specifies the three-letter site code of the Configuration Manager site that hosts the site system role.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SiteSystemServerName
Specifies an array of fully qualified domain names (FQDN) of the servers that host the site system role.

```yaml
Type: String
Parameter Sets: (All)
Aliases: Name

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Set-CMEmailNotificationComponent](Set-CMEmailNotificationComponent.md)


