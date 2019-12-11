---
title: Get-GlpiToolsKnowledgeBase
---

## SYNOPSIS
Function is getting Knowledge Base informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsKnowledgeBase [-All] [<CommonParameters>]
```

### KnowledgeBaseId
```
Get-GlpiToolsKnowledgeBase -KnowledgeBaseId <String[]> [-Raw] [<CommonParameters>]
```

## DESCRIPTION
Function is based on KnowledgeBaseId which you can find in GLPI website
Returns object with property's of Knowledge Base

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsKnowledgeBase -All
```

Example will return all Knowledge Base from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsKnowledgeBase
```

Function gets KnowledgeBaseId from GLPI from Pipline, and return Knowledge Base object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsKnowledgeBase
```

Function gets KnowledgeBaseId from GLPI from Pipline (u can pass many ID's like that), and return Knowledge Base object

### EXAMPLE 4
```
Get-GlpiToolsKnowledgeBase -KnowledgeBaseId 326
```

Function gets KnowledgeBaseId from GLPI which is provided through -KnowledgeBaseId after Function type, and return Knowledge Base object

### EXAMPLE 5
```
Get-GlpiToolsKnowledgeBase -KnowledgeBaseId 326, 321
```

Function gets Knowledge Base Id from GLPI which is provided through -KnowledgeBaseId keyword after Function type (u can provide many ID's like that), and return Knowledge Base object

## PARAMETERS

### -All
This parameter will return all Knowledge Base from GLPI

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

### -KnowledgeBaseId
This parameter can take pipline input, either, you can use this function with -KnowledgeBaseId keyword.
Provide to this param KnowledgeBaseId from GLPI Knowledge Base Bookmark

```yaml
Type: String[]
Parameter Sets: KnowledgeBaseId
Aliases: KBID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with KnowledgeBaseId Parameter.
KnowledgeBaseId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: KnowledgeBaseId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Knowledge Base ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Knowledge Base from GLPI
## NOTES
PSP 11/2019

## RELATED LINKS
