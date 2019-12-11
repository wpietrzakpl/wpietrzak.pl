---
title: Get-GlpiToolsEntities
---

## SYNOPSIS
Function returns entities from GLPI

## SYNTAX

### All
```
Get-GlpiToolsEntities [-All] [<CommonParameters>]
```

### EntityId
```
Get-GlpiToolsEntities -EntityId <String[]> [-Raw] [<CommonParameters>]
```

### EntityName
```
Get-GlpiToolsEntities -EntityName <String> [<CommonParameters>]
```

## DESCRIPTION
Function returns all possible enitites, you can provide id or name to get informations about desired entity

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsEntities -All
```

Command will return all entities from GLPI

### EXAMPLE 2
```
Get-GlpiToolsEntities -EntityId 3
```

Command will return entity with Id number 3 from GLPI

### EXAMPLE 3
```
3 | Get-GlpiToolsEntities
```

Command will return entity with Id number 3 from GLPI

### EXAMPLE 4
```
Get-GlpiToolsEntities -EntityName Old
```

Command will return entity with Name Old from GLPI

## PARAMETERS

### -All
This parameter will return all Entities from GLPI

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

### -EntityId
This parameter can take pipline input, either, you can use this function with -ComputerId keyword.
Provide to this param Entity ID from GLPI Entities Bookmark

```yaml
Type: String[]
Parameter Sets: EntityId
Aliases: EID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
{{ Fill Raw Description }}

```yaml
Type: SwitchParameter
Parameter Sets: EntityId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -EntityName
This parameter can take pipline input, either, you can use this function with -ComputerName keyword.
Provide to this param entity Name from GLPI Entities Bookmark

```yaml
Type: String
Parameter Sets: EntityName
Aliases: EN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Entity ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of entity from GLPI
## NOTES
PSP 01/2019

## RELATED LINKS
