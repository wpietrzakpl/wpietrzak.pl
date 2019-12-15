---
title: Get-GlpiToolsDropdownsManufacturers
---

## SYNOPSIS
Function is getting Manufacturer informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsManufacturers [-All] [<CommonParameters>]
```

### ManufacturerId
```
Get-GlpiToolsDropdownsManufacturers -ManufacturerId <String[]> [-Raw] [<CommonParameters>]
```

### ManufacturerName
```
Get-GlpiToolsDropdownsManufacturers -ManufacturerName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on ManufacturerID which you can find in GLPI website
Returns object with property's of Manufacturer

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsManufacturers -All
```

Example will return all Manufacturer from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsManufacturers
```

Function gets ManufacturerId from GLPI from Pipline, and return Manufacturer object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsManufacturers
```

Function gets ManufacturerId from GLPI from Pipline (u can pass many ID's like that), and return Manufacturer object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsManufacturers -ManufacturerId 326
```

Function gets ManufacturerId from GLPI which is provided through -ManufacturerId after Function type, and return Manufacturer object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsManufacturers -ManufacturerId 326, 321
```

Function gets ManufacturerId from GLPI which is provided through -ManufacturerId keyword after Function type (u can provide many ID's like that), and return Manufacturer object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsManufacturers -Manufacturer Fusion
```

Example will return glpi Manufacturer, but what is the most important, Manufacturer will be shown exactly as you see in glpi dropdown Manufacturer.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Manufacturer from GLPI

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

### -ManufacturerId
This parameter can take pipline input, either, you can use this function with -ManufacturerId keyword.
Provide to this param Manufacturer ID from GLPI Manufacturer Bookmark

```yaml
Type: String[]
Parameter Sets: ManufacturerId
Aliases: MID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with ManufacturerId Parameter.
ManufacturerId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: ManufacturerId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -ManufacturerName

```yaml
Type: String
Parameter Sets: ManufacturerName
Aliases: MN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Manufacturer ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Manufacturer from GLPI
## NOTES
PSP 06/2019

## RELATED LINKS
