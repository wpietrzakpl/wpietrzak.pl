---
title: Get-GlpiToolsDropdownsEnclosureModels
---

## SYNOPSIS
Function is getting Enclosure Models informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsEnclosureModels [-All] [<CommonParameters>]
```

### EnclosureModelId
```
Get-GlpiToolsDropdownsEnclosureModels -EnclosureModelId <String[]> [-Raw] [<CommonParameters>]
```

### EnclosureModelName
```
Get-GlpiToolsDropdownsEnclosureModels -EnclosureModelName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on EnclosureModelId which you can find in GLPI website
Returns object with property's of Enclosure Models

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsEnclosureModels -All
```

Example will return all Enclosure Models from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsEnclosureModels
```

Function gets EnclosureModelId from GLPI from Pipline, and return Enclosure Models object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsEnclosureModels
```

Function gets EnclosureModelId from GLPI from Pipline (u can pass many ID's like that), and return Enclosure Models object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsEnclosureModels -EnclosureModelId 326
```

Function gets EnclosureModelId from GLPI which is provided through -EnclosureModelId after Function type, and return Enclosure Models object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsEnclosureModels -EnclosureModelId 326, 321
```

Function gets Enclosure Models Id from GLPI which is provided through -EnclosureModelId keyword after Function type (u can provide many ID's like that), and return Enclosure Models object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsEnclosureModels -EnclosureModelName Fusion
```

Example will return glpi Enclosure Models, but what is the most important, Enclosure Models will be shown exactly as you see in glpi dropdown Enclosure Models.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Enclosure Models from GLPI

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

### -EnclosureModelId
This parameter can take pipline input, either, you can use this function with -EnclosureModelId keyword.
Provide to this param EnclosureModelId from GLPI Enclosure Models Bookmark

```yaml
Type: String[]
Parameter Sets: EnclosureModelId
Aliases: EMID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with EnclosureModelId Parameter.
EnclosureModelId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: EnclosureModelId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -EnclosureModelName
This parameter can take pipline input, either, you can use this function with -EnclosureModelId keyword.
Provide to this param Enclosure Models Name from GLPI Enclosure Models Bookmark

```yaml
Type: String
Parameter Sets: EnclosureModelName
Aliases: EMN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Enclosure Models ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Enclosure Models from GLPI
## NOTES
PSP 09/2019

## RELATED LINKS
