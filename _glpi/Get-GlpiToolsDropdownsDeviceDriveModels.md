---
title: Get-GlpiToolsDropdownsDeviceDriveModels
---

## SYNOPSIS
Function is getting Device Drive Models informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsDeviceDriveModels [-All] [<CommonParameters>]
```

### DeviceDriveModelId
```
Get-GlpiToolsDropdownsDeviceDriveModels -DeviceDriveModelId <String[]> [-Raw] [<CommonParameters>]
```

### DeviceDriveModelName
```
Get-GlpiToolsDropdownsDeviceDriveModels -DeviceDriveModelName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on DeviceDriveModelId which you can find in GLPI website
Returns object with property's of Device Drive Models

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsDeviceDriveModels -All
```

Example will return all Device Drive Models from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsDeviceDriveModels
```

Function gets DeviceDriveModelId from GLPI from Pipline, and return Device Drive Models object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsDeviceDriveModels
```

Function gets DeviceDriveModelId from GLPI from Pipline (u can pass many ID's like that), and return Device Drive Models object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsDeviceDriveModels -DeviceDriveModelId 326
```

Function gets DeviceDriveModelId from GLPI which is provided through -DeviceDriveModelId after Function type, and return Device Drive Models object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsDeviceDriveModels -DeviceDriveModelId 326, 321
```

Function gets Device Drive Models Id from GLPI which is provided through -DeviceDriveModelId keyword after Function type (u can provide many ID's like that), and return Device Drive Models object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsDeviceDriveModels -DeviceDriveModelName Fusion
```

Example will return glpi Device Drive Models, but what is the most important, Device Drive Models will be shown exactly as you see in glpi dropdown Device Drive Models.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Device Drive Models from GLPI

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

### -DeviceDriveModelId
This parameter can take pipline input, either, you can use this function with -DeviceDriveModelId keyword.
Provide to this param DeviceDriveModelId from GLPI Device Drive Models Bookmark

```yaml
Type: String[]
Parameter Sets: DeviceDriveModelId
Aliases: DDMID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with DeviceDriveModelId Parameter.
DeviceDriveModelId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: DeviceDriveModelId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -DeviceDriveModelName
This parameter can take pipline input, either, you can use this function with -DeviceDriveModelId keyword.
Provide to this param Device Drive Models Name from GLPI Device Drive Models Bookmark

```yaml
Type: String
Parameter Sets: DeviceDriveModelName
Aliases: DDMN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Device Drive Models ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Device Drive Models from GLPI
## NOTES
PSP 09/2019

## RELATED LINKS
