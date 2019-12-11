---
title: Get-GlpiToolsDropdownsProjectTaskTemplates
---

## SYNOPSIS
Function is getting Project Task Templates informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsProjectTaskTemplates [-All] [<CommonParameters>]
```

### ProjectTaskTemplateId
```
Get-GlpiToolsDropdownsProjectTaskTemplates -ProjectTaskTemplateId <String[]> [-Raw] [<CommonParameters>]
```

### ProjectTaskTemplateName
```
Get-GlpiToolsDropdownsProjectTaskTemplates -ProjectTaskTemplateName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on ProjectTaskTemplateId which you can find in GLPI website
Returns object with property's of Project Task Templates

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsProjectTaskTemplates -All
```

Example will return all Project Task Templates from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsProjectTaskTemplates
```

Function gets ProjectTaskTemplateId from GLPI from Pipline, and return Project Task Templates object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsProjectTaskTemplates
```

Function gets ProjectTaskTemplateId from GLPI from Pipline (u can pass many ID's like that), and return Project Task Templates object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsProjectTaskTemplates -ProjectTaskTemplateId 326
```

Function gets ProjectTaskTemplateId from GLPI which is provided through -ProjectTaskTemplateId after Function type, and return Project Task Templates object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsProjectTaskTemplates -ProjectTaskTemplateId 326, 321
```

Function gets Project Task Templates Id from GLPI which is provided through -ProjectTaskTemplateId keyword after Function type (u can provide many ID's like that), and return Project Task Templates object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsProjectTaskTemplates -ProjectTaskTemplateName Fusion
```

Example will return glpi Project Task Templates, but what is the most important, Project Task Templates will be shown exactly as you see in glpi dropdown Project Task Templates.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Project Task Templates from GLPI

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

### -ProjectTaskTemplateId
This parameter can take pipline input, either, you can use this function with -ProjectTaskTemplateId keyword.
Provide to this param ProjectTaskTemplateId from GLPI Project Task Templates Bookmark

```yaml
Type: String[]
Parameter Sets: ProjectTaskTemplateId
Aliases: PTTID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with ProjectTaskTemplateId Parameter.
ProjectTaskTemplateId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: ProjectTaskTemplateId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -ProjectTaskTemplateName
This parameter can take pipline input, either, you can use this function with -ProjectTaskTemplateId keyword.
Provide to this param Project Task Templates Name from GLPI Project Task Templates Bookmark

```yaml
Type: String
Parameter Sets: ProjectTaskTemplateName
Aliases: PTTN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Project Task Templates ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Project Task Templates from GLPI
## NOTES
PSP 09/2019

## RELATED LINKS
