---
title: Add-CMDeploymentTypeSupersedence
titleSuffix: Configuration Manager
description: Adds a deployment type supersedence in Configuration Manager.
ms.date: 01/02/2019
ms.prod: configuration-manager
ms.technology: configmgr-other
ms.topic: reference
author: mumian
ms.author: jgao
manager: dougeby
---

# Add-CMDeploymentTypeSupersedence

## SYNOPSIS

Adds a deployment type supersedence in Configuration Manager.

## SYNTAX

```powershell
Add-CMDeploymentTypeSupersedence [-SupersedingDeploymentType] <IResultObject>
 [-SupersededDeploymentType] <IResultObject> [-IsUninstall <Boolean>] [-DisableWildcardHandling]
 [-ForceWildcardHandling] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION

The **Add-CMDeploymentTypeSupersedence** cmdlet sets one deployment type to supersede another. Required input is a superseding type from [Get-CMDeploymentType](./Get-CMDeploymentType.md) and superseded deployment type from [Get-CMDeploymentType](./Get-CMDeploymentType.md).

## EXAMPLES

> [!NOTE]
> Configuration Manager CmdLets must be run from the Configuration Manager site drive. For more information, see the [getting started documentation](https://docs.microsoft.com/powershell/sccm/overview).


### Example 1

```
PS XYZ:\>  Get-CMDeploymentType -ApplicationName MyApp | Add-CMDeploymentTypeSupersedence -SupersedingDeploymentType (Get-CMDeploymentType -ApplicationName MySupersedingApp)
```

## PARAMETERS

### -Confirm

Prompts you for confirmation before running the cmdlet.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: cf

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

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

### -IsUninstall

```yaml
Type: Boolean
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SupersededDeploymentType

Specifies a superseded deployment type object.

```yaml
Type: IResultObject
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SupersedingDeploymentType

Specifies a superseding deployment type object.

```yaml
Type: IResultObject
Parameter Sets: (All)
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WhatIf

Shows what would happen if the cmdlet runs.
The cmdlet is not run.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: wi

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters

This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### None

## OUTPUTS

### System.Object

## RELATED LINKS

[Get-CMDeploymentTypeSupersedence](./Get-CMDeploymentTypeSupersedence.md)

[Set-CMDeploymentTypeSupersedence](./Set-CMDeploymentTypeSupersedence.md)

[Remove-CMDeploymentTypeSupersedence](./Remove-CMDeploymentTypeSupersedence.md)
