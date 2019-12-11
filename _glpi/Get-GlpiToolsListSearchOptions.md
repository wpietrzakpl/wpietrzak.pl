---
title: Get-GlpiToolsListSearchOptions
---

## SYNOPSIS
Function gets list of Search Options for specific Search in GLPI

## SYNTAX

```
Get-GlpiToolsListSearchOptions [-ListOptionsFor] <String> [<CommonParameters>]
```

## DESCRIPTION
Function gets list of Search Options for specific Search in GLPI
Parameters are the names of options in GLPI
Remember that, names used in cmdlet coming from glpi URL, and can be hard to understand, but most of them are intuitional.
To get name you always have to look at the URL in GLPI, for example "http://glpi/front/computer.php" where "computer" is the name to use in parameter.

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsListSearchOptions -ListOptionsFor DeviceCase
```

Example will return object which is list of Search Option for Setup -\> Components Tab from GLPI

## PARAMETERS

### -ListOptionsFor
You can use this function with -ListOptionsFor parameter.
Using TAB button you can choose desired option.
You can add your custom parameter options to Parameters.json file located in Private folder

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### None
## OUTPUTS

### Function returns PSCustomObject with property's of List Options from GLPI
## NOTES
PSP 03/2019

## RELATED LINKS
