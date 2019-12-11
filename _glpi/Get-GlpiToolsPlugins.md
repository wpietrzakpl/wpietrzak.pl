---
title: Get-GlpiToolsPlugins
---

## SYNOPSIS
Function to get GLPI Plugin list.

## SYNTAX

```
Get-GlpiToolsPlugins [-Raw] [<CommonParameters>]
```

## DESCRIPTION
Function is getting Plugin list from GLPI.
You can choose for Raw list, or list with translated status.

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsPlugins
```

Gets Plugin list from GLPI, with translated status from number to Enabled etc...

### EXAMPLE 2
```
Get-GlpiToolsPlugins -Raw
```

Gets Plugin list from GLPI, object isn't translated.
Original as it comes from GLPI.

## PARAMETERS

### -Raw
Switch parameter, you can use this parameter to get raw Plugin list.
Raw I mean, as that as it is from original object from GLPI.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
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

### None
## OUTPUTS

### Function returns PSCustomObject with property's of Plugins from GLPI
## NOTES
PSP 04/2019

## RELATED LINKS
