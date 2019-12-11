---
title: Get-GlpiToolsDropdownsSoftwareCategory
---

## SYNOPSIS
Function is getting Software Category's informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsSoftwareCategory [-All] [<CommonParameters>]
```

### SoftwareCategoryId
```
Get-GlpiToolsDropdownsSoftwareCategory -SoftwareCategoryId <String[]> [<CommonParameters>]
```

### SoftwareCategoryName
```
Get-GlpiToolsDropdownsSoftwareCategory -SoftwareCategoryName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on SoftwareCategoryId which you can find on GLPI website
Returns object with property's of Software Category's

## EXAMPLES

### EXAMPLE 1
```
326 | Get-GlpiToolsDropdownsSoftwareCategory
```

Function gets SoftwareCategoryId from GLPI from Pipline, and return Update Sources object

### EXAMPLE 2
```
326, 321 | Get-GlpiToolsDropdownsSoftwareCategory
```

Function gets SoftwareCategoryId from GLPI from Pipline (u can pass many ID's like that), and return Software Category object

### EXAMPLE 3
```
Get-GlpiToolsDropdownsSoftwareCategory -SoftwareCategoryId 326
```

Function gets SoftwareCategoryId from GLPI which is provided through -SoftwareCategoryId after Function type, and return Software Category object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsSoftwareCategory -SoftwareCategoryId 326, 321
```

Function gets SoftwareCategoryId from GLPI which is provided through -SoftwareCategoryId keyword after Function type (u can provide many ID's like that), and return Software Category object

## PARAMETERS

### -All
This parameter will return all Software Category's from GLPI

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

### -SoftwareCategoryId
This parameter can take pipline input, either, you can use this function with -SoftwareCategoryId keyword.
Provide to this param Software Category ID from GLPI Software Category Bookmark

```yaml
Type: String[]
Parameter Sets: SoftwareCategoryId
Aliases: SCID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -SoftwareCategoryName
You can use this function with -SoftwareCategoryName keyword.
Provide to this param Software Category Name from GLPI Software Category Bookmark

```yaml
Type: String
Parameter Sets: SoftwareCategoryName
Aliases: SCN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Software Category's ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Software Category's from GLPI
## NOTES
PSP 04/2019

## RELATED LINKS
