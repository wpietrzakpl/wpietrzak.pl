---
title: Get-GlpiToolsDropdownsDeviceHardDriveModels
---

## SYNOPSIS
Function is getting Device Hard Drive Models informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsDeviceHardDriveModels [-All] [<CommonParameters>]
```

### DeviceHardDriveModelId
```
Get-GlpiToolsDropdownsDeviceHardDriveModels -DeviceHardDriveModelId <String[]> [-Raw] [<CommonParameters>]
```

### DeviceHardDriveModelName
```
Get-GlpiToolsDropdownsDeviceHardDriveModels -DeviceHardDriveModelName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on DeviceHardDriveModelId which you can find in GLPI website
Returns object with property's of Device Hard Drive Models

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsDeviceHardDriveModels -All
```

Example will return all Device Hard Drive Models from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsDeviceHardDriveModels
```

Function gets DeviceHardDriveModelId from GLPI from Pipline, and return Device Hard Drive Models object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsDeviceHardDriveModels
```

Function gets DeviceHardDriveModelId from GLPI from Pipline (u can pass many ID's like that), and return Device Hard Drive Models object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsDeviceHardDriveModels -DeviceHardDriveModelId 326
```

Function gets DeviceHardDriveModelId from GLPI which is provided through -DeviceHardDriveModelId after Function type, and return Device Hard Drive Models object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsDeviceHardDriveModels -DeviceHardDriveModelId 326, 321
```

Function gets Device Hard Drive Models Id from GLPI which is provided through -DeviceHardDriveModelId keyword after Function type (u can provide many ID's like that), and return Device Hard Drive Models object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsDeviceHardDriveModels -DeviceHardDriveModelName Fusion
```

Example will return glpi Device Hard Drive Models, but what is the most important, Device Hard Drive Models will be shown exactly as you see in glpi dropdown Device Hard Drive Models.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Device Hard Drive Models from GLPI

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

### -DeviceHardDriveModelId
This parameter can take pipline input, either, you can use this function with -DeviceHardDriveModelId keyword.
Provide to this param DeviceHardDriveModelId from GLPI Device Hard Drive Models Bookmark

```yaml
Type: String[]
Parameter Sets: DeviceHardDriveModelId
Aliases: DHDMID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with DeviceHardDriveModelId Parameter.
DeviceHardDriveModelId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: DeviceHardDriveModelId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -DeviceHardDriveModelName
This parameter can take pipline input, either, you can use this function with -DeviceHardDriveModelId keyword.
Provide to this param Device Hard Drive Models Name from GLPI Device Hard Drive Models Bookmark

```yaml
Type: String
Parameter Sets: DeviceHardDriveModelName
Aliases: DHDMN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Device Hard Drive Models ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Device Hard Drive Models from GLPI
## NOTES
PSP 09/2019

## RELATED LINKS
