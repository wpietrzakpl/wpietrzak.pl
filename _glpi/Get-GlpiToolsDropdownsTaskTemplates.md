---
title: Get-GlpiToolsDropdownsTaskTemplates
---

## SYNOPSIS
Function is getting Task Templates informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsTaskTemplates [-All] [<CommonParameters>]
```

### TaskTemplateId
```
Get-GlpiToolsDropdownsTaskTemplates -TaskTemplateId <String[]> [-Raw] [<CommonParameters>]
```

### TaskTemplateName
```
Get-GlpiToolsDropdownsTaskTemplates -TaskTemplateName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on TaskTemplateId which you can find in GLPI website
Returns object with property's of Task Templates

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsTaskTemplates -All
```

Example will return all Task Templates from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsTaskTemplates
```

Function gets TaskTemplateId from GLPI from Pipline, and return Task Templates object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsTaskTemplates
```

Function gets TaskTemplateId from GLPI from Pipline (u can pass many ID's like that), and return Task Templates object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsTaskTemplates -TaskTemplateId 326
```

Function gets TaskTemplateId from GLPI which is provided through -TaskTemplateId after Function type, and return Task Templates object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsTaskTemplates -TaskTemplateId 326, 321
```

Function gets Task Templates Id from GLPI which is provided through -TaskTemplateId keyword after Function type (u can provide many ID's like that), and return Task Templates object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsTaskTemplates -TaskTemplateName Fusion
```

Example will return glpi Task Templates, but what is the most important, Task Templates will be shown exactly as you see in glpi dropdown Task Templates.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Task Templates from GLPI

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

### -TaskTemplateId
This parameter can take pipline input, either, you can use this function with -TaskTemplateId keyword.
Provide to this param TaskTemplateId from GLPI Task Templates Bookmark

```yaml
Type: String[]
Parameter Sets: TaskTemplateId
Aliases: TTID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with TaskTemplateId Parameter.
TaskTemplateId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: TaskTemplateId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -TaskTemplateName
This parameter can take pipline input, either, you can use this function with -TaskTemplateId keyword.
Provide to this param Task Templates Name from GLPI Task Templates Bookmark

```yaml
Type: String
Parameter Sets: TaskTemplateName
Aliases: TTN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Task Templates ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Task Templates from GLPI
## NOTES
PSP 09/2019

## RELATED LINKS
