---
title: Get-GlpiToolsDropdownsDeviceGraphicCardModels
---

## SYNOPSIS
Function is getting Device Graphic Card Models informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsDeviceGraphicCardModels [-All] [<CommonParameters>]
```

### DeviceGraphicCardModelId
```
Get-GlpiToolsDropdownsDeviceGraphicCardModels -DeviceGraphicCardModelId <String[]> [-Raw] [<CommonParameters>]
```

### DeviceGraphicCardModelName
```
Get-GlpiToolsDropdownsDeviceGraphicCardModels -DeviceGraphicCardModelName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on DeviceGraphicCardModelId which you can find in GLPI website
Returns object with property's of Device Graphic Card Models

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsDeviceGraphicCardModels -All
```

Example will return all Device Graphic Card Models from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsDeviceGraphicCardModels
```

Function gets DeviceGraphicCardModelId from GLPI from Pipline, and return Device Graphic Card Models object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsDeviceGraphicCardModels
```

Function gets DeviceGraphicCardModelId from GLPI from Pipline (u can pass many ID's like that), and return Device Graphic Card Models object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsDeviceGraphicCardModels -DeviceGraphicCardModelId 326
```

Function gets DeviceGraphicCardModelId from GLPI which is provided through -DeviceGraphicCardModelId after Function type, and return Device Graphic Card Models object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsDeviceGraphicCardModels -DeviceGraphicCardModelId 326, 321
```

Function gets Device Graphic Card Models Id from GLPI which is provided through -DeviceGraphicCardModelId keyword after Function type (u can provide many ID's like that), and return Device Graphic Card Models object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsDeviceGraphicCardModels -DeviceGraphicCardModelName Fusion
```

Example will return glpi Device Graphic Card Models, but what is the most important, Device Graphic Card Models will be shown exactly as you see in glpi dropdown Device Graphic Card Models.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Device Graphic Card Models from GLPI

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

### -DeviceGraphicCardModelId
This parameter can take pipline input, either, you can use this function with -DeviceGraphicCardModelId keyword.
Provide to this param DeviceGraphicCardModelId from GLPI Device Graphic Card Models Bookmark

```yaml
Type: String[]
Parameter Sets: DeviceGraphicCardModelId
Aliases: DGCMID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with DeviceGraphicCardModelId Parameter.
DeviceGraphicCardModelId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: DeviceGraphicCardModelId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -DeviceGraphicCardModelName
This parameter can take pipline input, either, you can use this function with -DeviceGraphicCardModelId keyword.
Provide to this param Device Graphic Card Models Name from GLPI Device Graphic Card Models Bookmark

```yaml
Type: String
Parameter Sets: DeviceGraphicCardModelName
Aliases: DGCMN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Device Graphic Card Models ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Device Graphic Card Models from GLPI
## NOTES
PSP 09/2019

## RELATED LINKS
