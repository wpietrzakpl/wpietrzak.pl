---
title: Get-GlpiToolsDropdownsPeripheralModels
---

## SYNOPSIS
Function is getting Peripheral Models informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsPeripheralModels [-All] [<CommonParameters>]
```

### PeripheralModelId
```
Get-GlpiToolsDropdownsPeripheralModels -PeripheralModelId <String[]> [-Raw] [<CommonParameters>]
```

### PeripheralModelName
```
Get-GlpiToolsDropdownsPeripheralModels -PeripheralModelName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on PeripheralModelId which you can find in GLPI website
Returns object with property's of Peripheral Models

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsPeripheralModels -All
```

Example will return all Peripheral Models from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsPeripheralModels
```

Function gets PeripheralModelId from GLPI from Pipline, and return Peripheral Models object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsPeripheralModels
```

Function gets PeripheralModelId from GLPI from Pipline (u can pass many ID's like that), and return Peripheral Models object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsPeripheralModels -PeripheralModelId 326
```

Function gets PeripheralModelId from GLPI which is provided through -PeripheralModelId after Function type, and return Peripheral Models object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsPeripheralModels -PeripheralModelId 326, 321
```

Function gets Peripheral Models Id from GLPI which is provided through -PeripheralModelId keyword after Function type (u can provide many ID's like that), and return Peripheral Models object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsPeripheralModels -PeripheralModelName Fusion
```

Example will return glpi Peripheral Models, but what is the most important, Peripheral Models will be shown exactly as you see in glpi dropdown Peripheral Models.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Peripheral Models from GLPI

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

### -PeripheralModelId
This parameter can take pipline input, either, you can use this function with -PeripheralModelId keyword.
Provide to this param PeripheralModelId from GLPI Peripheral Models Bookmark

```yaml
Type: String[]
Parameter Sets: PeripheralModelId
Aliases: PMID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with PeripheralModelId Parameter.
PeripheralModelId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: PeripheralModelId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -PeripheralModelName
This parameter can take pipline input, either, you can use this function with -PeripheralModelId keyword.
Provide to this param Peripheral Models Name from GLPI Peripheral Models Bookmark

```yaml
Type: String
Parameter Sets: PeripheralModelName
Aliases: PMN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Peripheral Models ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Peripheral Models from GLPI
## NOTES
PSP 09/2019

## RELATED LINKS
