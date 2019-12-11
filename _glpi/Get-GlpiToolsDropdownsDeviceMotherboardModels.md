---
title: Get-GlpiToolsDropdownsDeviceMotherboardModels
---

## SYNOPSIS
Function is getting Device Motherboard Models informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsDeviceMotherboardModels [-All] [<CommonParameters>]
```

### DeviceMotherboardModelId
```
Get-GlpiToolsDropdownsDeviceMotherboardModels -DeviceMotherboardModelId <String[]> [-Raw] [<CommonParameters>]
```

### DeviceMotherboardModelName
```
Get-GlpiToolsDropdownsDeviceMotherboardModels -DeviceMotherboardModelName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on DeviceMotherboardModelId which you can find in GLPI website
Returns object with property's of Device Motherboard Models

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsDeviceMotherboardModels -All
```

Example will return all Device Motherboard Models from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsDeviceMotherboardModels
```

Function gets DeviceMotherboardModelId from GLPI from Pipline, and return Device Motherboard Models object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsDeviceMotherboardModels
```

Function gets DeviceMotherboardModelId from GLPI from Pipline (u can pass many ID's like that), and return Device Motherboard Models object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsDeviceMotherboardModels -DeviceMotherboardModelId 326
```

Function gets DeviceMotherboardModelId from GLPI which is provided through -DeviceMotherboardModelId after Function type, and return Device Motherboard Models object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsDeviceMotherboardModels -DeviceMotherboardModelId 326, 321
```

Function gets Device Motherboard Models Id from GLPI which is provided through -DeviceMotherboardModelId keyword after Function type (u can provide many ID's like that), and return Device Motherboard Models object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsDeviceMotherboardModels -DeviceMotherboardModelName Fusion
```

Example will return glpi Device Motherboard Models, but what is the most important, Device Motherboard Models will be shown exactly as you see in glpi dropdown Device Motherboard Models.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Device Motherboard Models from GLPI

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

### -DeviceMotherboardModelId
This parameter can take pipline input, either, you can use this function with -DeviceMotherboardModelId keyword.
Provide to this param DeviceMotherboardModelId from GLPI Device Motherboard Models Bookmark

```yaml
Type: String[]
Parameter Sets: DeviceMotherboardModelId
Aliases: DMMID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with DeviceMotherboardModelId Parameter.
DeviceMotherboardModelId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: DeviceMotherboardModelId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -DeviceMotherboardModelName
This parameter can take pipline input, either, you can use this function with -DeviceMotherboardModelId keyword.
Provide to this param Device Motherboard Models Name from GLPI Device Motherboard Models Bookmark

```yaml
Type: String
Parameter Sets: DeviceMotherboardModelName
Aliases: DMMN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Device Motherboard Models ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Device Motherboard Models from GLPI
## NOTES
PSP 09/2019

## RELATED LINKS
