---
title: Get-GlpiToolsSoftwareLicenses
---

## SYNOPSIS
Function is getting Software License informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsSoftwareLicenses [-All] [<CommonParameters>]
```

### SoftwareLicenseId
```
Get-GlpiToolsSoftwareLicenses -SoftwareLicenseId <String[]> [-Raw] [<CommonParameters>]
```

### SoftwareLicenseName
```
Get-GlpiToolsSoftwareLicenses -SoftwareLicenseName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on SoftwareLicenseId which you can find in GLPI website
Returns object with property's of Software License

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsSoftwareLicenses -All
```

Example will return all Software License from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsSoftwareLicenses
```

Function gets SoftwareLicenseId from GLPI from Pipline, and return Software License object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsSoftwareLicenses
```

Function gets SoftwareLicenseId from GLPI from Pipline (u can pass many ID's like that), and return Software License object

### EXAMPLE 4
```
Get-GlpiToolsSoftwareLicenses -SoftwareLicenseId 326
```

Function gets SoftwareLicenseId from GLPI which is provided through -SoftwareLicenseId after Function type, and return Software License object

### EXAMPLE 5
```
Get-GlpiToolsSoftwareLicenses -SoftwareLicenseId 326, 321
```

Function gets Software License Id from GLPI which is provided through -SoftwareLicenseId keyword after Function type (u can provide many ID's like that), and return Software License object

### EXAMPLE 6
```
Get-GlpiToolsSoftwareLicenses -SoftwareLicenseName Fusion
```

Example will return glpi Software License, but what is the most important, Software License will be shown exactly as you see in glpi dropdown Software License.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Software License from GLPI

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

### -SoftwareLicenseId
This parameter can take pipline input, either, you can use this function with -SoftwareLicenseId keyword.
Provide to this param SoftwareLicenseId from GLPI Software License Bookmark

```yaml
Type: String[]
Parameter Sets: SoftwareLicenseId
Aliases: SLID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with SoftwareLicenseId Parameter.
SoftwareLicenseId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: SoftwareLicenseId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -SoftwareLicenseName
This parameter can take pipline input, either, you can use this function with -SoftwareLicenseId keyword.
Provide to this param Software License Name from GLPI Software License Bookmark

```yaml
Type: String
Parameter Sets: SoftwareLicenseName
Aliases: SLN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Software License ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Software License from GLPI
## NOTES
PSP 11/2019

## RELATED LINKS
