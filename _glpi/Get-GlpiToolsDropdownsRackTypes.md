---
title: Get-GlpiToolsDropdownsRackTypes
---

## SYNOPSIS
Function is getting Rack Types informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsRackTypes [-All] [<CommonParameters>]
```

### RackTypeId
```
Get-GlpiToolsDropdownsRackTypes -RackTypeId <String[]> [-Raw] [<CommonParameters>]
```

### RackTypeName
```
Get-GlpiToolsDropdownsRackTypes -RackTypeName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on RackTypeId which you can find in GLPI website
Returns object with property's of Rack Types

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsRackTypes -All
```

Example will return all Rack Types from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsRackTypes
```

Function gets RackTypeId from GLPI from pipeline, and return Rack Types object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsRackTypes
```

Function gets RackTypeId from GLPI from pipeline (u can pass many ID's like that), and return Rack Types object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsRackTypes -RackTypeId 326
```

Function gets RackTypeId from GLPI which is provided through -RackTypeId after Function type, and return Rack Types object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsRackTypes -RackTypeId 326, 321
```

Function gets Rack Types Id from GLPI which is provided through -RackTypeId keyword after Function type (u can provide many ID's like that), and return Rack Types object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsRackTypes -RackTypeName Fusion
```

Example will return glpi Rack Types, but what is the most important, Rack Types will be shown exactly as you see in glpi dropdown Rack Types.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Rack Types from GLPI

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

### -RackTypeId
This parameter can take pipeline input, either, you can use this function with -RackTypeId keyword.
Provide to this param RackTypeId from GLPI Rack Types Bookmark

```yaml
Type: String[]
Parameter Sets: RackTypeId
Aliases: RTID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with RackTypeId Parameter.
RackTypeId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: RackTypeId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -RackTypeName
This parameter can take pipeline input, either, you can use this function with -RackTypeId keyword.
Provide to this param Rack Types Name from GLPI Rack Types Bookmark

```yaml
Type: String
Parameter Sets: RackTypeName
Aliases: RTN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Rack Types ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Rack Types from GLPI
## NOTES
PSP 09/2019

## RELATED LINKS
