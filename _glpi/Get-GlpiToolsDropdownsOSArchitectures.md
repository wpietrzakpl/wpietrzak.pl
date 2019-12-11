---
title: Get-GlpiToolsDropdownsOSArchitectures
---

## SYNOPSIS
Function is getting Architectures informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsOSArchitectures [-All] [<CommonParameters>]
```

### OSArchitectureId
```
Get-GlpiToolsDropdownsOSArchitectures -OSArchitectureId <String[]> [-Raw] [<CommonParameters>]
```

### OSArchitectureName
```
Get-GlpiToolsDropdownsOSArchitectures -OSArchitectureName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on OSArchitectureId which you can find in GLPI website
Returns object with property's of Architectures Packs

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsOSArchitectures -All
```

Example will return all Architectures Packs from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsOSArchitectures
```

Function gets OSArchitectureId from GLPI from Pipline, and return Architectures Packs object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsOSArchitectures
```

Function gets OSArchitectureId from GLPI from Pipline (u can pass many ID's like that), and return Architectures Packs object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsOSArchitectures -OSArchitectureId 326
```

Function gets OSArchitectureId from GLPI which is provided through -OSArchitectureId after Function type, and return Architectures Packs object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsOSArchitectures -OSArchitectureId 326, 321
```

Function gets Architectures PacksId from GLPI which is provided through -OSArchitectureId keyword after Function type (u can provide many ID's like that), and return Architectures Packs object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsOSArchitectures -OSArchitectureName Fusion
```

Example will return glpi Architectures Packs, but what is the most important, Architectures Packs will be shown exactly as you see in glpi dropdown Architectures Packs.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Architectures Packs from GLPI

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

### -OSArchitectureId
This parameter can take pipline input, either, you can use this function with -OSArchitectureId keyword.
Provide to this param OSArchitectureId from GLPI Architectures Packs Bookmark

```yaml
Type: String[]
Parameter Sets: OSArchitectureId
Aliases: OSAID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with OSArchitectureId Parameter.
OSArchitectureId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: OSArchitectureId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -OSArchitectureName
This parameter can take pipline input, either, you can use this function with -OSArchitectureId keyword.
Provide to this param Architectures Packs Name from GLPI Architectures Packs Bookmark

```yaml
Type: String
Parameter Sets: OSArchitectureName
Aliases: OSAN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Architectures Packs ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Architectures Packs from GLPI
## NOTES
PSP 08/2019

## RELATED LINKS
