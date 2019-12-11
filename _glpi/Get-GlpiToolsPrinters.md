---
title: Get-GlpiToolsPrinters
---

## SYNOPSIS
Function is getting Printer informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsPrinters [-All] [<CommonParameters>]
```

### PrinterId
```
Get-GlpiToolsPrinters -PrinterId <String[]> [-Raw] [-Parameter <String>] [<CommonParameters>]
```

### PrinterName
```
Get-GlpiToolsPrinters -PrinterName <String> [-SearchInTrash <String>] [<CommonParameters>]
```

## DESCRIPTION
Function is based on PrinterID which you can find in GLPI website
Returns object with property's of Printer

## EXAMPLES

### EXAMPLE 1
```
326 | Get-GlpiToolsPrinters
```

Function gets PrinterID from GLPI from Pipline, and return Printer object

### EXAMPLE 2
```
326, 321 | Get-GlpiToolsPrinters
```

Function gets PrinterID from GLPI from Pipline (u can pass many ID's like that), and return Printer object

### EXAMPLE 3
```
Get-GlpiToolsPrinters -PrinterId 326
```

Function gets PrinterID from GLPI which is provided through -PrinterId after Function type, and return Printer object

### EXAMPLE 4
```
Get-GlpiToolsPrinters -PrinterId 326, 321
```

Function gets PrinterID from GLPI which is provided through -PrinterId keyword after Function type (u can provide many ID's like that), and return Printer object

### EXAMPLE 5
```
Get-GlpiToolsPrinters -PrinterId 234 -Raw
```

Example will show Printer with id 234, but without any parameter converted

### EXAMPLE 6
```
234 | Get-GlpiToolsPrinters -Raw
```

Example will show Printer with id 234, but without any parameter converted

### EXAMPLE 7
```
Get-GlpiToolsPrinters -PrinterName glpi
```

Example will return glpi Printer, but what is the most important, Printer will be shown exacly as you see in glpi Printers tab.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

### EXAMPLE 8
```
Get-GlpiToolsPrinters -PrinterName glpi -SearchInTrash Yes
```

Example will return glpi Printer, but from trash

## PARAMETERS

### -All
This parameter will return all Printers from GLPI

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

### -PrinterId
This parameter can take pipline input, either, you can use this function with -PrinterId keyword.
Provide to this param Printer ID from GLPI Printers Bookmark

```yaml
Type: String[]
Parameter Sets: PrinterId
Aliases: PID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with PrinterId Parameter.
PrinterId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: PrinterId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -PrinterName
Provide to this param Printer Name from GLPI Printers Bookmark

```yaml
Type: String
Parameter Sets: PrinterName
Aliases: PN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SearchInTrash
Parameter which you can use with PrinterName Parameter.
If you want Search for Printer name in trash, that parameter allow you to do it.

```yaml
Type: String
Parameter Sets: PrinterName
Aliases: SIT

Required: False
Position: Named
Default value: No
Accept pipeline input: False
Accept wildcard characters: False
```

### -Parameter
Parameter which you can use with PrinterId Parameter. 
If you want to get additional parameter of Printer object like, disks, or logs, use this parameter.

```yaml
Type: String
Parameter Sets: PrinterId
Aliases: Param

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Printer ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Printers from GLPI
## NOTES
PSP 05/2019

## RELATED LINKS
