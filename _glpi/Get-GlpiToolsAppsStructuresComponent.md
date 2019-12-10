---
title: Get-GlpiToolsAppsStructuresComponent
---

## SYNOPSIS
Function to show Apps Structures Components from GLPI

## SYNTAX

### All
```
Get-GlpiToolsAppsStructuresComponent [-All] [<CommonParameters>]
```

### AppsStructureId
```
Get-GlpiToolsAppsStructuresComponent -AppsStructureId <Int32[]> [-Raw] [<CommonParameters>]
```

## DESCRIPTION
Function to show Apps Structures Components from GLPI.
Function will show all Components from Apps Structures.

## EXAMPLES

### EXAMPLE 1
```
GlpiToolsAppsStructuresComponent -All
```

Example will show All Apps Structures Items

### EXAMPLE 2
```
Get-GlpiToolsAppsStructuresComponent -AppsStructureId 2
```

Example will show Apps Structure Item which id is 2.
Object will have converted values.

### EXAMPLE 3
```
Get-GlpiToolsAppsStructuresComponent -AppsStructureId 2 -Raw
```

Example will show Apps Structure Item which id is 2.
Object will not have converted values.

### EXAMPLE 4
```
2 | Get-GlpiToolsAppsStructuresComponent
```

Example will show Apps Structure Item which id is 2.
Object will have converted values.

### EXAMPLE 5
```
2 | Get-GlpiToolsAppsStructuresComponent -Raw
```

Example will show Apps Structure Item which id is 2.
Object will not have converted values.

## PARAMETERS

### -All
Switch parameter, if you will choose, you will get All available Apps Component.

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

### -AppsStructureId
Int parameter, you can provide here number of Apps Structure.
It is ID which you can find in GLPI or with parameter -All.
Can take pipeline input.

```yaml
Type: Int32[]
Parameter Sets: AppsStructureId
Aliases: ASID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Switch parameter.
In default output has converted id to humanreadable format, that parameter can disable it and return raw object with id's.

```yaml
Type: SwitchParameter
Parameter Sets: AppsStructureId
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

### Inputs (if any)
## OUTPUTS

### Function returns PSCustomObject
## NOTES
PSP 05/2019

## RELATED LINKS
