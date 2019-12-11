---
title: Get-GlpiToolsDropdownsCartridgeTypes
---

## SYNOPSIS
Function is getting Cartridge Types informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsCartridgeTypes [-All] [<CommonParameters>]
```

### CartridgeTypeId
```
Get-GlpiToolsDropdownsCartridgeTypes -CartridgeTypeId <String[]> [-Raw] [<CommonParameters>]
```

### CartridgeTypeName
```
Get-GlpiToolsDropdownsCartridgeTypes -CartridgeTypeName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on CartridgeTypeId which you can find in GLPI website
Returns object with property's of Cartridge Types

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsCartridgeTypes -All
```

Example will return all Cartridge Types from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsCartridgeTypes
```

Function gets CartridgeTypeId from GLPI from Pipline, and return Cartridge Types object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsCartridgeTypes
```

Function gets CartridgeTypeId from GLPI from Pipline (u can pass many ID's like that), and return Cartridge Types object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsCartridgeTypes -CartridgeTypeId 326
```

Function gets CartridgeTypeId from GLPI which is provided through -CartridgeTypeId after Function type, and return Cartridge Types object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsCartridgeTypes -CartridgeTypeId 326, 321
```

Function gets Cartridge Types Id from GLPI which is provided through -CartridgeTypeId keyword after Function type (u can provide many ID's like that), and return Cartridge Types object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsCartridgeTypes -CartridgeTypeName Fusion
```

Example will return glpi Cartridge Types, but what is the most important, Cartridge Types will be shown exactly as you see in glpi dropdown Cartridge Types.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Cartridge Types from GLPI

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

### -CartridgeTypeId
This parameter can take pipline input, either, you can use this function with -CartridgeTypeId keyword.
Provide to this param CartridgeTypeId from GLPI Cartridge Types Bookmark

```yaml
Type: String[]
Parameter Sets: CartridgeTypeId
Aliases: CTID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with CartridgeTypeId Parameter.
CartridgeTypeId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: CartridgeTypeId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -CartridgeTypeName
This parameter can take pipline input, either, you can use this function with -CartridgeTypeId keyword.
Provide to this param Cartridge Types Name from GLPI Cartridge Types Bookmark

```yaml
Type: String
Parameter Sets: CartridgeTypeName
Aliases: CTN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Cartridge Types ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Cartridge Types from GLPI
## NOTES
PSP 09/2019

## RELATED LINKS
