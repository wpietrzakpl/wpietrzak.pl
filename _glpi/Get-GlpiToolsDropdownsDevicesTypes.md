---
title: Get-GlpiToolsDropdownsDevicesTypes
---

## SYNOPSIS
Function is getting Devices Types informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsDevicesTypes [-All] [<CommonParameters>]
```

### DeviceTypeId
```
Get-GlpiToolsDropdownsDevicesTypes -DeviceTypeId <String[]> [-Raw] [<CommonParameters>]
```

### DeviceTypeName
```
Get-GlpiToolsDropdownsDevicesTypes -DeviceTypeName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on DeviceTypeId which you can find in GLPI website
Returns object with property's of Devices Types

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsDevicesTypes -All
```

Example will return all Devices Types from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsDevicesTypes
```

Function gets DeviceTypeId from GLPI from Pipline, and return Devices Types object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsDevicesTypes
```

Function gets DeviceTypeId from GLPI from Pipline (u can pass many ID's like that), and return Devices Types object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsDevicesTypes -DeviceTypeId 326
```

Function gets DeviceTypeId from GLPI which is provided through -DeviceTypeId after Function type, and return Devices Types object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsDevicesTypes -DeviceTypeId 326, 321
```

Function gets Devices Types Id from GLPI which is provided through -DeviceTypeId keyword after Function type (u can provide many ID's like that), and return Devices Types object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsDevicesTypes -DeviceTypeName Fusion
```

Example will return glpi Devices Types, but what is the most important, Devices Types will be shown exactly as you see in glpi dropdown Devices Types.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Devices Types from GLPI

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

### -DeviceTypeId
This parameter can take pipline input, either, you can use this function with -DeviceTypeId keyword.
Provide to this param DeviceTypeId from GLPI Devices Types Bookmark

```yaml
Type: String[]
Parameter Sets: DeviceTypeId
Aliases: DTID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with DeviceTypeId Parameter.
DeviceTypeId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: DeviceTypeId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -DeviceTypeName
This parameter can take pipline input, either, you can use this function with -DeviceTypeId keyword.
Provide to this param Devices Types Name from GLPI Devices Types Bookmark

```yaml
Type: String
Parameter Sets: DeviceTypeName
Aliases: DTN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Devices Types ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Devices Types from GLPI
## NOTES
PSP 09/2019

## RELATED LINKS
