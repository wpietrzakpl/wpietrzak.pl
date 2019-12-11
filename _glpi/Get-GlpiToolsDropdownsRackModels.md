---
title: Get-GlpiToolsDropdownsRackModels
---

## SYNOPSIS
Function is getting Rack Models informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsRackModels [-All] [<CommonParameters>]
```

### RackModelId
```
Get-GlpiToolsDropdownsRackModels -RackModelId <String[]> [-Raw] [<CommonParameters>]
```

### RackModelName
```
Get-GlpiToolsDropdownsRackModels -RackModelName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on RackModelId which you can find in GLPI website
Returns object with property's of Rack Models

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsRackModels -All
```

Example will return all Rack Models from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsRackModels
```

Function gets RackModelId from GLPI from Pipline, and return Rack Models object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsRackModels
```

Function gets RackModelId from GLPI from Pipline (u can pass many ID's like that), and return Rack Models object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsRackModels -RackModelId 326
```

Function gets RackModelId from GLPI which is provided through -RackModelId after Function type, and return Rack Models object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsRackModels -RackModelId 326, 321
```

Function gets Rack Models Id from GLPI which is provided through -RackModelId keyword after Function type (u can provide many ID's like that), and return Rack Models object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsRackModels -RackModelName Fusion
```

Example will return glpi Rack Models, but what is the most important, Rack Models will be shown exactly as you see in glpi dropdown Rack Models.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Rack Models from GLPI

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

### -RackModelId
This parameter can take pipline input, either, you can use this function with -RackModelId keyword.
Provide to this param RackModelId from GLPI Rack Models Bookmark

```yaml
Type: String[]
Parameter Sets: RackModelId
Aliases: RMID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with RackModelId Parameter.
RackModelId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: RackModelId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -RackModelName
This parameter can take pipline input, either, you can use this function with -RackModelId keyword.
Provide to this param Rack Models Name from GLPI Rack Models Bookmark

```yaml
Type: String
Parameter Sets: RackModelName
Aliases: RMN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Rack Models ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Rack Models from GLPI
## NOTES
PSP 09/2019

## RELATED LINKS
