---
title: Get-GlpiToolsAppsStructuresComponentDb
---

## SYNOPSIS
Function to show Apps Structures Dbs from GLPI

## SYNTAX

### All
```
Get-GlpiToolsAppsStructuresComponentDb [-All] [<CommonParameters>]
```

### AppsStructureComponentDbId
```
Get-GlpiToolsAppsStructuresComponentDb [-AppsStructureComponentDbId <Int32[]>] [<CommonParameters>]
```

## DESCRIPTION
Function to show Apps Structures Dbs from GLPI.
Function will show all Dbs from Apps Structures.

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsAppsStructuresComponentDb -All
```

Example will show All Apps Structures Dbs

### EXAMPLE 2
```
Get-GlpiToolsAppsStructuresComponentDb -AppsStructureComponentDbId 2
```

Example will show Apps Structure Db which id is 2.
Object will have converted values.

### EXAMPLE 3
```
Get-GlpiToolsAppsStructuresComponentDb -AppsStructureComponentDbId 2 -Raw
```

Example will show Apps Structure Db which id is 2.
Object will not have converted values.

### EXAMPLE 4
```
2 | Get-GlpiToolsAppsStructuresComponentDb
```

Example will show Apps Structure Db which id is 2.
Object will have converted values.

### EXAMPLE 5
```
2 | Get-GlpiToolsAppsStructuresComponentDb -Raw
```

Example will show Apps Structure Db which id is 2.
Object will not have converted values.

## PARAMETERS

### -All
Switch parameter, if you will choose, you will get All available Apps Db.

```yaml
Type: SwitchParameter
Parameter Sets: All
Aliases:

Required: True
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -AppsStructureComponentDbId
Int parameter, you can provide here number of Apps Structure Db.
It is ID which you can find in GLPI or with parameter -All.
Can take pipeline input.

```yaml
Type: Int32[]
Parameter Sets: AppsStructureComponentDbId
Aliases: ASCDID

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Inputs (if any)
## OUTPUTS

### Function returns PSCustomObject
## NOTES
PSP 05/2019

## RELATED LINKS
