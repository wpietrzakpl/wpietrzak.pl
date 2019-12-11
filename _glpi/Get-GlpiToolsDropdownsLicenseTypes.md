---
title: Get-GlpiToolsDropdownsLicenseTypes
---

## SYNOPSIS
Function is getting License Types informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsLicenseTypes [-All] [<CommonParameters>]
```

### LicenseTypeId
```
Get-GlpiToolsDropdownsLicenseTypes -LicenseTypeId <String[]> [-Raw] [<CommonParameters>]
```

### LicenseTypeName
```
Get-GlpiToolsDropdownsLicenseTypes -LicenseTypeName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on LicenseTypeId which you can find in GLPI website
Returns object with property's of License Types

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsLicenseTypes -All
```

Example will return all License Types from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsLicenseTypes
```

Function gets LicenseTypeId from GLPI from Pipline, and return License Types object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsLicenseTypes
```

Function gets LicenseTypeId from GLPI from Pipline (u can pass many ID's like that), and return License Types object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsLicenseTypes -LicenseTypeId 326
```

Function gets LicenseTypeId from GLPI which is provided through -LicenseTypeId after Function type, and return License Types object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsLicenseTypes -LicenseTypeId 326, 321
```

Function gets License Types Id from GLPI which is provided through -LicenseTypeId keyword after Function type (u can provide many ID's like that), and return License Types object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsLicenseTypes -LicenseTypeName Fusion
```

Example will return glpi License Types, but what is the most important, License Types will be shown exactly as you see in glpi dropdown License Types.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all License Types from GLPI

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

### -LicenseTypeId
This parameter can take pipline input, either, you can use this function with -LicenseTypeId keyword.
Provide to this param LicenseTypeId from GLPI License Types Bookmark

```yaml
Type: String[]
Parameter Sets: LicenseTypeId
Aliases: LTID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with LicenseTypeId Parameter.
LicenseTypeId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: LicenseTypeId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -LicenseTypeName
This parameter can take pipline input, either, you can use this function with -LicenseTypeId keyword.
Provide to this param License Types Name from GLPI License Types Bookmark

```yaml
Type: String
Parameter Sets: LicenseTypeName
Aliases: LTN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### License Types ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of License Types from GLPI
## NOTES
PSP 09/2019

## RELATED LINKS
