---
title: Get-GlpiToolsDropdownsComputerModels
---

## SYNOPSIS
Function is getting Computer Models informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsComputerModels [-All] [<CommonParameters>]
```

### ComputerModelsId
```
Get-GlpiToolsDropdownsComputerModels -ComputerModelsId <String[]> [-Raw] [<CommonParameters>]
```

### ComputerModelsName
```
Get-GlpiToolsDropdownsComputerModels -ComputerModelsName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on ComputerModelsID which you can find in GLPI website
Returns object with property's of Computer Models

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsComputerModels -All
```

Example will return all Computer Models from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsComputerModels
```

Function gets ComputerModelsId from GLPI from Pipline, and return Computer Models object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsComputerModels
```

Function gets ComputerModelsId from GLPI from Pipline (u can pass many ID's like that), and return Computer Models object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsComputerModels -ComputerModelsId 326
```

Function gets ComputerModelsId from GLPI which is provided through -ComputerModelsId after Function type, and return Computer Models object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsComputerModels -ComputerModelsId 326, 321
```

Function gets ComputerModelsId from GLPI which is provided through -ComputerModelsId keyword after Function type (u can provide many ID's like that), and return Computer Models object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsComputerModels -ComputerModelsName Lenovo
```

Example will return glpi computer model, but what is the most important, computer model will be shown exactly as you see in glpi dropdown computer models.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Computer Models from GLPI

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

### -ComputerModelsId
This parameter can take pipline input, either, you can use this function with -ComputerModelsId keyword.
Provide to this param Computer Models ID from GLPI Computer Models Bookmark

```yaml
Type: String[]
Parameter Sets: ComputerModelsId
Aliases: CMID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with ComputerModelsId Parameter.
ComputerModelsId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: ComputerModelsId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -ComputerModelsName
This parameter can take pipline input, either, you can use this function with -ComputerModelsName keyword.
Provide to this param Computer Models Name from GLPI Computer Models Bookmark

```yaml
Type: String
Parameter Sets: ComputerModelsName
Aliases: CMN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Computer Models ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Computer Models from GLPI
## NOTES
PSP 03/2019

## RELATED LINKS
