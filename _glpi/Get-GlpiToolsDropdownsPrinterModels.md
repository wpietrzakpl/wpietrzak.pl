---
title: Get-GlpiToolsDropdownsPrinterModels
---

## SYNOPSIS
Function is getting Printer Models informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsPrinterModels [-All] [<CommonParameters>]
```

### PrinterModelId
```
Get-GlpiToolsDropdownsPrinterModels -PrinterModelId <String[]> [-Raw] [<CommonParameters>]
```

### PrinterModelName
```
Get-GlpiToolsDropdownsPrinterModels -PrinterModelName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on PrinterModelId which you can find in GLPI website
Returns object with property's of Printer Models

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsPrinterModels -All
```

Example will return all Printer Models from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsPrinterModels
```

Function gets PrinterModelId from GLPI from Pipline, and return Printer Models object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsPrinterModels
```

Function gets PrinterModelId from GLPI from Pipline (u can pass many ID's like that), and return Printer Models object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsPrinterModels -PrinterModelId 326
```

Function gets PrinterModelId from GLPI which is provided through -PrinterModelId after Function type, and return Printer Models object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsPrinterModels -PrinterModelId 326, 321
```

Function gets Printer Models Id from GLPI which is provided through -PrinterModelId keyword after Function type (u can provide many ID's like that), and return Printer Models object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsPrinterModels -PrinterModelName Fusion
```

Example will return glpi Printer Models, but what is the most important, Printer Models will be shown exactly as you see in glpi dropdown Printer Models.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Printer Models from GLPI

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

### -PrinterModelId
This parameter can take pipline input, either, you can use this function with -PrinterModelId keyword.
Provide to this param PrinterModelId from GLPI Printer Models Bookmark

```yaml
Type: String[]
Parameter Sets: PrinterModelId
Aliases: PMID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with PrinterModelId Parameter.
PrinterModelId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: PrinterModelId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -PrinterModelName
This parameter can take pipline input, either, you can use this function with -PrinterModelId keyword.
Provide to this param Printer Models Name from GLPI Printer Models Bookmark

```yaml
Type: String
Parameter Sets: PrinterModelName
Aliases: PMN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Printer Models ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Printer Models from GLPI
## NOTES
PSP 09/2019

## RELATED LINKS
