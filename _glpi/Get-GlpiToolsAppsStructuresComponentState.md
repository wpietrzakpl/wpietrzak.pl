---
title: Get-GlpiToolsAppsStructuresComponentState
---

## SYNOPSIS
Function to show Apps Structures States from GLPI

## SYNTAX

### All
```
Get-GlpiToolsAppsStructuresComponentState [-All] [<CommonParameters>]
```

### AppsStructureComponentStateId
```
Get-GlpiToolsAppsStructuresComponentState [-AppsStructureComponentStateId <Int32[]>] [<CommonParameters>]
```

## DESCRIPTION
Function to show Apps Structures States from GLPI.
Function will show all States from Apps Structures.

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsAppsStructuresComponentState -All
```

Example will show All Apps Structures States

### EXAMPLE 2
```
Get-GlpiToolsAppsStructuresComponentState -AppsStructureComponentStateId 2
```

Example will show Apps Structure State which id is 2.
Object will have converted values.

### EXAMPLE 3
```
Get-GlpiToolsAppsStructuresComponentState -AppsStructureComponentStateId 2 -Raw
```

Example will show Apps Structure State which id is 2.
Object will not have converted values.

### EXAMPLE 4
```
2 | Get-GlpiToolsAppsStructuresComponentState
```

Example will show Apps Structure State which id is 2.
Object will have converted values.

### EXAMPLE 5
```
2 | Get-GlpiToolsAppsStructuresComponentState -Raw
```

Example will show Apps Structure State which id is 2.
Object will not have converted values.

## PARAMETERS

### -All
Switch parameter, if you will choose, you will get All available Apps State.

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

### -AppsStructureComponentStateId
Int parameter, you can provide here number of Apps Structure State.
It is ID which you can find in GLPI or with parameter -All.
Can take pipeline input.

```yaml
Type: Int32[]
Parameter Sets: AppsStructureComponentStateId
Aliases: ASCSID

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
