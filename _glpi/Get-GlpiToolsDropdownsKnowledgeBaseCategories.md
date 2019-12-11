---
title: Get-GlpiToolsDropdownsKnowledgeBaseCategories
---

## SYNOPSIS
Function is getting Knowledge Base Categories informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsKnowledgeBaseCategories [-All] [<CommonParameters>]
```

### KnowledgeBaseCategoryId
```
Get-GlpiToolsDropdownsKnowledgeBaseCategories -KnowledgeBaseCategoryId <String[]> [-Raw] [<CommonParameters>]
```

### KnowledgeBaseCategoryName
```
Get-GlpiToolsDropdownsKnowledgeBaseCategories -KnowledgeBaseCategoryName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on KnowledgeBaseCategoryId which you can find in GLPI website
Returns object with property's of Knowledge Base Categories

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsKnowledgeBaseCategories -All
```

Example will return all Knowledge Base Categories from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsKnowledgeBaseCategories
```

Function gets KnowledgeBaseCategoryId from GLPI from pipeline, and return Knowledge Base Categories object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsKnowledgeBaseCategories
```

Function gets KnowledgeBaseCategoryId from GLPI from pipeline (u can pass many ID's like that), and return Knowledge Base Categories object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsKnowledgeBaseCategories -KnowledgeBaseCategoryId 326
```

Function gets KnowledgeBaseCategoryId from GLPI which is provided through -KnowledgeBaseCategoryId after Function type, and return Knowledge Base Categories object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsKnowledgeBaseCategories -KnowledgeBaseCategoryId 326, 321
```

Function gets Knowledge Base Categories Id from GLPI which is provided through -KnowledgeBaseCategoryId keyword after Function type (u can provide many ID's like that), and return Knowledge Base Categories object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsKnowledgeBaseCategories -KnowledgeBaseCategoryName Fusion
```

Example will return glpi Knowledge Base Categories, but what is the most important, Knowledge Base Categories will be shown exactly as you see in glpi dropdown Knowledge Base Categories.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Knowledge Base Categories from GLPI

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

### -KnowledgeBaseCategoryId
This parameter can take pipeline input, either, you can use this function with -KnowledgeBaseCategoryId keyword.
Provide to this param KnowledgeBaseCategoryId from GLPI Knowledge Base Categories Bookmark

```yaml
Type: String[]
Parameter Sets: KnowledgeBaseCategoryId
Aliases: KBCID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with KnowledgeBaseCategoryId Parameter.
KnowledgeBaseCategoryId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: KnowledgeBaseCategoryId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -KnowledgeBaseCategoryName
This parameter can take pipeline input, either, you can use this function with -KnowledgeBaseCategoryId keyword.
Provide to this param Knowledge Base Categories Name from GLPI Knowledge Base Categories Bookmark

```yaml
Type: String
Parameter Sets: KnowledgeBaseCategoryName
Aliases: KBCN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Knowledge Base Categories ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Knowledge Base Categories from GLPI
## NOTES
PSP 09/2019

## RELATED LINKS
