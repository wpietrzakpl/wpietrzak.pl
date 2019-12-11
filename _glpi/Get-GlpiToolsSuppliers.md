---
title: Get-GlpiToolsSuppliers
---

## SYNOPSIS
Function is getting Supplier informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsSuppliers [-All] [<CommonParameters>]
```

### SupplierId
```
Get-GlpiToolsSuppliers -SupplierId <String[]> [-Raw] [<CommonParameters>]
```

### SupplierName
```
Get-GlpiToolsSuppliers -SupplierName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on SupplierId which you can find in GLPI website
Returns object with property's of Supplier

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsSuppliers -All
```

Example will return all Supplier from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsSuppliers
```

Function gets SupplierId from GLPI from Pipline, and return Supplier object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsSuppliers
```

Function gets SupplierId from GLPI from Pipline (u can pass many ID's like that), and return Supplier object

### EXAMPLE 4
```
Get-GlpiToolsSuppliers -SupplierId 326
```

Function gets SupplierId from GLPI which is provided through -SupplierId after Function type, and return Supplier object

### EXAMPLE 5
```
Get-GlpiToolsSuppliers -SupplierId 326, 321
```

Function gets Supplier Id from GLPI which is provided through -SupplierId keyword after Function type (u can provide many ID's like that), and return Supplier object

### EXAMPLE 6
```
Get-GlpiToolsSuppliers -SupplierName Fusion
```

Example will return glpi Supplier, but what is the most important, Supplier will be shown exactly as you see in glpi dropdown Supplier.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Supplier from GLPI

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

### -SupplierId
This parameter can take pipline input, either, you can use this function with -SupplierId keyword.
Provide to this param SupplierId from GLPI Supplier Bookmark

```yaml
Type: String[]
Parameter Sets: SupplierId
Aliases: SID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with SupplierId Parameter.
SupplierId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: SupplierId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -SupplierName
This parameter can take pipline input, either, you can use this function with -SupplierId keyword.
Provide to this param Supplier Name from GLPI Supplier Bookmark

```yaml
Type: String
Parameter Sets: SupplierName
Aliases: SN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Supplier ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Supplier from GLPI
## NOTES
PSP 11/2019

## RELATED LINKS
