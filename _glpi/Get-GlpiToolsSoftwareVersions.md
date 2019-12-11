---
title: Get-GlpiToolsSoftwareVersions
---

## SYNOPSIS
Function is getting Software Version informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsSoftwareVersions [-All] [<CommonParameters>]
```

### SoftwareVersionId
```
Get-GlpiToolsSoftwareVersions -SoftwareVersionId <String[]> [-Raw] [<CommonParameters>]
```

## DESCRIPTION
Function is based on Software Version ID which you can find in GLPI website
Returns object with property's of Software Version

## EXAMPLES

### EXAMPLE 1
```
326 | Get-GlpiToolsSoftwareVersions
```

Function gets SoftwareVersionID from GLPI from Pipline, and return Software Version object

### EXAMPLE 2
```
326, 321 | Get-GlpiToolsSoftwareVersions
```

Function gets SoftwareVersionID from GLPI from Pipline (u can pass many ID's like that), and return Software Version object

### EXAMPLE 3
```
Get-GlpiToolsSoftwareVersions -SoftwareVersionId 326
```

Function gets SoftwareVersionID from GLPI which is provided through -SoftwareVersionId after Function type, and return Software Version object

### EXAMPLE 4
```
Get-GlpiToolsSoftwareVersions -SoftwareVersionId 326, 321
```

Function gets SoftwareVersionID from GLPI which is provided through -SoftwareVersionId keyword after Function type (u can provide many ID's like that), and return Software Version object

### EXAMPLE 5
```
Get-GlpiToolsSoftwareVersions -SoftwareVersionId 234 -Raw
```

Example will show Software Version with id 234, but without any parameter converted

### EXAMPLE 6
```
234 | Get-GlpiToolsSoftwareVersions -Raw
```

Example will show Software Version with id 234, but without any parameter converted

## PARAMETERS

### -All
This parameter will return all Software Versions from GLPI

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

### -SoftwareVersionId
This parameter can take pipline input, either, you can use this function with -SoftwareVersionId keyword.
Provide to this param Software Version ID from GLPI

```yaml
Type: String[]
Parameter Sets: SoftwareVersionId
Aliases: SVID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with SoftwareVersionId Parameter.
SoftwareVersionId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: SoftwareVersionId
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

### Software Version ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Software Versions from GLPI
## NOTES
PSP 08/2019

## RELATED LINKS
