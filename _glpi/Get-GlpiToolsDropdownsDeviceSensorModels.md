---
title: Get-GlpiToolsDropdownsDeviceSensorModels
---

## SYNOPSIS
Function is getting Device Sensor Models informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsDeviceSensorModels [-All] [<CommonParameters>]
```

### DeviceSensorModelId
```
Get-GlpiToolsDropdownsDeviceSensorModels -DeviceSensorModelId <String[]> [-Raw] [<CommonParameters>]
```

### DeviceSensorModelName
```
Get-GlpiToolsDropdownsDeviceSensorModels -DeviceSensorModelName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on DeviceSensorModelId which you can find in GLPI website
Returns object with property's of Device Sensor Models

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsDeviceSensorModels -All
```

Example will return all Device Sensor Models from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsDeviceSensorModels
```

Function gets DeviceSensorModelId from GLPI from Pipline, and return Device Sensor Models object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsDeviceSensorModels
```

Function gets DeviceSensorModelId from GLPI from Pipline (u can pass many ID's like that), and return Device Sensor Models object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsDeviceSensorModels -DeviceSensorModelId 326
```

Function gets DeviceSensorModelId from GLPI which is provided through -DeviceSensorModelId after Function type, and return Device Sensor Models object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsDeviceSensorModels -DeviceSensorModelId 326, 321
```

Function gets Device Sensor Models Id from GLPI which is provided through -DeviceSensorModelId keyword after Function type (u can provide many ID's like that), and return Device Sensor Models object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsDeviceSensorModels -DeviceSensorModelName Fusion
```

Example will return glpi Device Sensor Models, but what is the most important, Device Sensor Models will be shown exactly as you see in glpi dropdown Device Sensor Models.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Device Sensor Models from GLPI

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

### -DeviceSensorModelId
This parameter can take pipline input, either, you can use this function with -DeviceSensorModelId keyword.
Provide to this param DeviceSensorModelId from GLPI Device Sensor Models Bookmark

```yaml
Type: String[]
Parameter Sets: DeviceSensorModelId
Aliases: DSMID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with DeviceSensorModelId Parameter.
DeviceSensorModelId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: DeviceSensorModelId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -DeviceSensorModelName
This parameter can take pipline input, either, you can use this function with -DeviceSensorModelId keyword.
Provide to this param Device Sensor Models Name from GLPI Device Sensor Models Bookmark

```yaml
Type: String
Parameter Sets: DeviceSensorModelName
Aliases: DSMN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Device Sensor Models ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Device Sensor Models from GLPI
## NOTES
PSP 09/2019

## RELATED LINKS
