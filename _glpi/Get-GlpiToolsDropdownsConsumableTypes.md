---
title: Get-GlpiToolsDropdownsConsumableTypes
---

## SYNOPSIS
Function is getting Consumable Types informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsConsumableTypes [-All] [<CommonParameters>]
```

### ConsumableTypeId
```
Get-GlpiToolsDropdownsConsumableTypes -ConsumableTypeId <String[]> [-Raw] [<CommonParameters>]
```

### ConsumableTypeName
```
Get-GlpiToolsDropdownsConsumableTypes -ConsumableTypeName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on ConsumableTypeId which you can find in GLPI website
Returns object with property's of Consumable Types

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsConsumableTypes -All
```

Example will return all Consumable Types from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsConsumableTypes
```

Function gets ConsumableTypeId from GLPI from Pipline, and return Consumable Types object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsConsumableTypes
```

Function gets ConsumableTypeId from GLPI from Pipline (u can pass many ID's like that), and return Consumable Types object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsConsumableTypes -ConsumableTypeId 326
```

Function gets ConsumableTypeId from GLPI which is provided through -ConsumableTypeId after Function type, and return Consumable Types object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsConsumableTypes -ConsumableTypeId 326, 321
```

Function gets Consumable Types Id from GLPI which is provided through -ConsumableTypeId keyword after Function type (u can provide many ID's like that), and return Consumable Types object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsConsumableTypes -ConsumableTypeName Fusion
```

Example will return glpi Consumable Types, but what is the most important, Consumable Types will be shown exactly as you see in glpi dropdown Consumable Types.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Consumable Types from GLPI

```yaml
Type: SwitchParameter
Parameter Sets: All
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -ConsumableTypeId
This parameter can take pipline input, either, you can use this function with -ConsumableTypeId keyword.
Provide to this param ConsumableTypeId from GLPI Consumable Types Bookmark

```yaml
Type: String[]
Parameter Sets: ConsumableTypeId
Aliases: CTID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with ConsumableTypeId Parameter.
ConsumableTypeId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: ConsumableTypeId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -ConsumableTypeName
This parameter can take pipline input, either, you can use this function with -ConsumableTypeId keyword.
Provide to this param Consumable Types Name from GLPI Consumable Types Bookmark

```yaml
Type: String
Parameter Sets: ConsumableTypeName
Aliases: CTN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Consumable Types ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Consumable Types from GLPI
## NOTES
PSP 09/2019

## RELATED LINKS
