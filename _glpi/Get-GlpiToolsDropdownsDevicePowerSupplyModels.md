---
title: Get-GlpiToolsDropdownsDevicePowerSupplyModels
---

## SYNOPSIS
Function is getting Device Power Supply Models informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsDevicePowerSupplyModels [-All] [<CommonParameters>]
```

### DevicePowerSupplyModelId
```
Get-GlpiToolsDropdownsDevicePowerSupplyModels -DevicePowerSupplyModelId <String[]> [-Raw] [<CommonParameters>]
```

### DevicePowerSupplyModelName
```
Get-GlpiToolsDropdownsDevicePowerSupplyModels -DevicePowerSupplyModelName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on DevicePowerSupplyModelId which you can find in GLPI website
Returns object with property's of Device Power Supply Models

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsDevicePowerSupplyModels -All
```

Example will return all Device Power Supply Models from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsDevicePowerSupplyModels
```

Function gets DevicePowerSupplyModelId from GLPI from Pipline, and return Device Power Supply Models object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsDevicePowerSupplyModels
```

Function gets DevicePowerSupplyModelId from GLPI from Pipline (u can pass many ID's like that), and return Device Power Supply Models object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsDevicePowerSupplyModels -DevicePowerSupplyModelId 326
```

Function gets DevicePowerSupplyModelId from GLPI which is provided through -DevicePowerSupplyModelId after Function type, and return Device Power Supply Models object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsDevicePowerSupplyModels -DevicePowerSupplyModelId 326, 321
```

Function gets Device Power Supply Models Id from GLPI which is provided through -DevicePowerSupplyModelId keyword after Function type (u can provide many ID's like that), and return Device Power Supply Models object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsDevicePowerSupplyModels -DevicePowerSupplyModelName Fusion
```

Example will return glpi Device Power Supply Models, but what is the most important, Device Power Supply Models will be shown exactly as you see in glpi dropdown Device Power Supply Models.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Device Power Supply Models from GLPI

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

### -DevicePowerSupplyModelId
This parameter can take pipline input, either, you can use this function with -DevicePowerSupplyModelId keyword.
Provide to this param DevicePowerSupplyModelId from GLPI Device Power Supply Models Bookmark

```yaml
Type: String[]
Parameter Sets: DevicePowerSupplyModelId
Aliases: DPSMID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with DevicePowerSupplyModelId Parameter.
DevicePowerSupplyModelId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: DevicePowerSupplyModelId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -DevicePowerSupplyModelName
This parameter can take pipline input, either, you can use this function with -DevicePowerSupplyModelId keyword.
Provide to this param Device Power Supply Models Name from GLPI Device Power Supply Models Bookmark

```yaml
Type: String
Parameter Sets: DevicePowerSupplyModelName
Aliases: DPSMN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Device Power Supply Models ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Device Power Supply Models from GLPI
## NOTES
PSP 09/2019

## RELATED LINKS
