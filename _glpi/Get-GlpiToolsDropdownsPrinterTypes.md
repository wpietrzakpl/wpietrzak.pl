---
title: Get-GlpiToolsDropdownsPrinterTypes
---

## SYNOPSIS
Function is getting Printer Types informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsPrinterTypes [-All] [<CommonParameters>]
```

### PrinterTypeId
```
Get-GlpiToolsDropdownsPrinterTypes -PrinterTypeId <String[]> [-Raw] [<CommonParameters>]
```

### PrinterTypeName
```
Get-GlpiToolsDropdownsPrinterTypes -PrinterTypeName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on PrinterTypeId which you can find in GLPI website
Returns object with property's of Printer Types

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsPrinterTypes -All
```

Example will return all Printer Types from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsPrinterTypes
```

Function gets PrinterTypeId from GLPI from Pipline, and return Printer Types object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsPrinterTypes
```

Function gets PrinterTypeId from GLPI from Pipline (u can pass many ID's like that), and return Printer Types object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsPrinterTypes -PrinterTypeId 326
```

Function gets PrinterTypeId from GLPI which is provided through -PrinterTypeId after Function type, and return Printer Types object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsPrinterTypes -PrinterTypeId 326, 321
```

Function gets Printer Types Id from GLPI which is provided through -PrinterTypeId keyword after Function type (u can provide many ID's like that), and return Printer Types object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsPrinterTypes -PrinterTypeName Fusion
```

Example will return glpi Printer Types, but what is the most important, Printer Types will be shown exactly as you see in glpi dropdown Printer Types.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Printer Types from GLPI

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

### -PrinterTypeId
This parameter can take pipline input, either, you can use this function with -PrinterTypeId keyword.
Provide to this param PrinterTypeId from GLPI Printer Types Bookmark

```yaml
Type: String[]
Parameter Sets: PrinterTypeId
Aliases: PTID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with PrinterTypeId Parameter.
PrinterTypeId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: PrinterTypeId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -PrinterTypeName
This parameter can take pipline input, either, you can use this function with -PrinterTypeId keyword.
Provide to this param Printer Types Name from GLPI Printer Types Bookmark

```yaml
Type: String
Parameter Sets: PrinterTypeName
Aliases: PTN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Printer Types ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Printer Types from GLPI
## NOTES
PSP 09/2019

## RELATED LINKS
