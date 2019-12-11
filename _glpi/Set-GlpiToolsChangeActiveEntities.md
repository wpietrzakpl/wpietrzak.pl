---
title: Set-GlpiToolsChangeActiveEntities
---

## SYNOPSIS
Function change active entity of GLPI.

## SYNTAX

```
Set-GlpiToolsChangeActiveEntities [-EntitiesId] <Int32> [-IsRecursive] [<CommonParameters>]
```

## DESCRIPTION
Change active entity to the entities id one.
See Get-GlpiToolsEntities function /w -All parameter for possible entities.

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsEntities -EntityName "put entity name here" | Select-Object -ExpandProperty Id | Set-GlpiToolsChangeActiveEntities
```

Example changes active entity to entity which you provided to the pipeline

### EXAMPLE 2
```
Get-GlpiToolsEntities -EntityName "put entity name here" | Select-Object -ExpandProperty Id | Set-GlpiToolsChangeActiveEntities -IsRecursive
```

Example changes active entity to entity which you provided to the pipeline, and enable display sub entities of active entity.

### EXAMPLE 3
```
Set-GlpiToolsChangeActiveEntities -EntitiesId "id"
```

Example changes active entity to entity which you provided to the -EntitiesId parameter.

### EXAMPLE 4
```
Set-GlpiToolsChangeActiveEntities -EntitiesId "id" -IsRecursive
```

Example changes active entity to entity which you provided to the -EntitiesId parameter, and enable display sub entities of active entity.

## PARAMETERS

### -EntitiesId
This parameter provide to function entity id, on which you want to change.

```yaml
Type: Int32
Parameter Sets: (All)
Aliases: EID

Required: True
Position: 1
Default value: 0
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -IsRecursive
This parameter will enable display sub entities of the active entity.
Parameter is optional

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: IR

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Entities Id which you can find in GLPI, or using Get-GlpiToolsEntities parameter.
## OUTPUTS

### Output (if any)
## NOTES
PSP 03/2019

## RELATED LINKS
