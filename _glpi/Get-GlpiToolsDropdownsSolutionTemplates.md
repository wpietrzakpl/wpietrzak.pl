---
title: Get-GlpiToolsDropdownsSolutionTemplates
---

## SYNOPSIS
Function is getting Solution Templates informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsSolutionTemplates [-All] [<CommonParameters>]
```

### SolutionTemplateId
```
Get-GlpiToolsDropdownsSolutionTemplates -SolutionTemplateId <String[]> [-Raw] [<CommonParameters>]
```

### SolutionTemplateName
```
Get-GlpiToolsDropdownsSolutionTemplates -SolutionTemplateName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on SolutionTemplateId which you can find in GLPI website
Returns object with property's of Solution Templates

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsSolutionTemplates -All
```

Example will return all Solution Templates from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsSolutionTemplates
```

Function gets SolutionTemplateId from GLPI from Pipline, and return Solution Templates object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsSolutionTemplates
```

Function gets SolutionTemplateId from GLPI from Pipline (u can pass many ID's like that), and return Solution Templates object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsSolutionTemplates -SolutionTemplateId 326
```

Function gets SolutionTemplateId from GLPI which is provided through -SolutionTemplateId after Function type, and return Solution Templates object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsSolutionTemplates -SolutionTemplateId 326, 321
```

Function gets Solution Templates Id from GLPI which is provided through -SolutionTemplateId keyword after Function type (u can provide many ID's like that), and return Solution Templates object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsSolutionTemplates -SolutionTemplateName Fusion
```

Example will return glpi Solution Templates, but what is the most important, Solution Templates will be shown exactly as you see in glpi dropdown Solution Templates.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Solution Templates from GLPI

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

### -SolutionTemplateId
This parameter can take pipline input, either, you can use this function with -SolutionTemplateId keyword.
Provide to this param SolutionTemplateId from GLPI Solution Templates Bookmark

```yaml
Type: String[]
Parameter Sets: SolutionTemplateId
Aliases: STID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with SolutionTemplateId Parameter.
SolutionTemplateId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: SolutionTemplateId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -SolutionTemplateName
This parameter can take pipline input, either, you can use this function with -SolutionTemplateId keyword.
Provide to this param Solution Templates Name from GLPI Solution Templates Bookmark

```yaml
Type: String
Parameter Sets: SolutionTemplateName
Aliases: STN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Solution Templates ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Solution Templates from GLPI
## NOTES
PSP 09/2019

## RELATED LINKS
