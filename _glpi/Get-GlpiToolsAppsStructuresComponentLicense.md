---
title: Get-GlpiToolsAppsStructuresComponentLicense
---

## SYNOPSIS
Function to show Apps Structures Licenses from GLPI

## SYNTAX

### All
```
Get-GlpiToolsAppsStructuresComponentLicense [-All] [<CommonParameters>]
```

### AppsStructureComponentLicenseId
```
Get-GlpiToolsAppsStructuresComponentLicense [-AppsStructureComponentLicenseId <Int32[]>] [<CommonParameters>]
```

## DESCRIPTION
Function to show Apps Structures Licenses from GLPI.
Function will show all Licenses from Apps Structures.

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsAppsStructuresComponentLicense -All
```

Example will show All Apps Structures Licenses

### EXAMPLE 2
```
Get-GlpiToolsAppsStructuresComponentLicense -AppsStructureComponentLicenseId 2
```

Example will show Apps Structure License which id is 2.
Object will have converted values.

### EXAMPLE 3
```
Get-GlpiToolsAppsStructuresComponentLicense -AppsStructureComponentLicenseId 2 -Raw
```

Example will show Apps Structure License which id is 2.
Object will not have converted values.

### EXAMPLE 4
```
2 | Get-GlpiToolsAppsStructuresComponentLicense
```

Example will show Apps Structure License which id is 2.
Object will have converted values.

### EXAMPLE 5
```
2 | Get-GlpiToolsAppsStructuresComponentLicense -Raw
```

Example will show Apps Structure License which id is 2.
Object will not have converted values.

## PARAMETERS

### -All
Switch parameter, if you will choose, you will get All available Apps License.

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

### -AppsStructureComponentLicenseId
Int parameter, you can provide here number of Apps Structure License.
It is ID which you can find in GLPI or with parameter -All.
Can take pipeline input.

```yaml
Type: Int32[]
Parameter Sets: AppsStructureComponentLicenseId
Aliases: ASCLID

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
