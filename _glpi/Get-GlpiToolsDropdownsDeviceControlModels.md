---
title: Get-GlpiToolsDropdownsDeviceControlModels
---

## SYNOPSIS
Function is getting Device Control Models informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsDeviceControlModels [-All] [<CommonParameters>]
```

### DeviceControlModelId
```
Get-GlpiToolsDropdownsDeviceControlModels -DeviceControlModelId <String[]> [-Raw] [<CommonParameters>]
```

### DeviceControlModelName
```
Get-GlpiToolsDropdownsDeviceControlModels -DeviceControlModelName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on DeviceControlModelId which you can find in GLPI website
Returns object with property's of Device Control Models

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsDeviceControlModels -All
```

Example will return all Device Control Models from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsDeviceControlModels
```

Function gets DeviceControlModelId from GLPI from Pipline, and return Device Control Models object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsDeviceControlModels
```

Function gets DeviceControlModelId from GLPI from Pipline (u can pass many ID's like that), and return Device Control Models object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsDeviceControlModels -DeviceControlModelId 326
```

Function gets DeviceControlModelId from GLPI which is provided through -DeviceControlModelId after Function type, and return Device Control Models object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsDeviceControlModels -DeviceControlModelId 326, 321
```

Function gets Device Control Models Id from GLPI which is provided through -DeviceControlModelId keyword after Function type (u can provide many ID's like that), and return Device Control Models object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsDeviceControlModels -DeviceControlModelName Fusion
```

Example will return glpi Device Control Models, but what is the most important, Device Control Models will be shown exactly as you see in glpi dropdown Device Control Models.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Device Control Models from GLPI

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

### -DeviceControlModelId
This parameter can take pipline input, either, you can use this function with -DeviceControlModelId keyword.
Provide to this param DeviceControlModelId from GLPI Device Control Models Bookmark

```yaml
Type: String[]
Parameter Sets: DeviceControlModelId
Aliases: DCMID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with DeviceControlModelId Parameter.
DeviceControlModelId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: DeviceControlModelId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -DeviceControlModelName
This parameter can take pipline input, either, you can use this function with -DeviceControlModelId keyword.
Provide to this param Device Control Models Name from GLPI Device Control Models Bookmark

```yaml
Type: String
Parameter Sets: DeviceControlModelName
Aliases: DCMN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Device Control Models ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Device Control Models from GLPI
## NOTES
PSP 09/2019

## RELATED LINKS
