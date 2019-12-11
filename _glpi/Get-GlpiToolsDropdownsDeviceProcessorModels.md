---
title: Get-GlpiToolsDropdownsDeviceProcessorModels
---

## SYNOPSIS
Function is getting Device Processor Models informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsDeviceProcessorModels [-All] [<CommonParameters>]
```

### DeviceProcessorModelId
```
Get-GlpiToolsDropdownsDeviceProcessorModels -DeviceProcessorModelId <String[]> [-Raw] [<CommonParameters>]
```

### DeviceProcessorModelName
```
Get-GlpiToolsDropdownsDeviceProcessorModels -DeviceProcessorModelName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on DeviceProcessorModelId which you can find in GLPI website
Returns object with property's of Device Processor Models

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsDeviceProcessorModels -All
```

Example will return all Device Processor Models from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsDeviceProcessorModels
```

Function gets DeviceProcessorModelId from GLPI from Pipline, and return Device Processor Models object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsDeviceProcessorModels
```

Function gets DeviceProcessorModelId from GLPI from Pipline (u can pass many ID's like that), and return Device Processor Models object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsDeviceProcessorModels -DeviceProcessorModelId 326
```

Function gets DeviceProcessorModelId from GLPI which is provided through -DeviceProcessorModelId after Function type, and return Device Processor Models object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsDeviceProcessorModels -DeviceProcessorModelId 326, 321
```

Function gets Device Processor Models Id from GLPI which is provided through -DeviceProcessorModelId keyword after Function type (u can provide many ID's like that), and return Device Processor Models object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsDeviceProcessorModels -DeviceProcessorModelName Fusion
```

Example will return glpi Device Processor Models, but what is the most important, Device Processor Models will be shown exactly as you see in glpi dropdown Device Processor Models.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Device Processor Models from GLPI

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

### -DeviceProcessorModelId
This parameter can take pipline input, either, you can use this function with -DeviceProcessorModelId keyword.
Provide to this param DeviceProcessorModelId from GLPI Device Processor Models Bookmark

```yaml
Type: String[]
Parameter Sets: DeviceProcessorModelId
Aliases: DPMID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with DeviceProcessorModelId Parameter.
DeviceProcessorModelId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: DeviceProcessorModelId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -DeviceProcessorModelName
This parameter can take pipline input, either, you can use this function with -DeviceProcessorModelId keyword.
Provide to this param Device Processor Models Name from GLPI Device Processor Models Bookmark

```yaml
Type: String
Parameter Sets: DeviceProcessorModelName
Aliases: DPMN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Device Processor Models ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Device Processor Models from GLPI
## NOTES
PSP 09/2019

## RELATED LINKS
