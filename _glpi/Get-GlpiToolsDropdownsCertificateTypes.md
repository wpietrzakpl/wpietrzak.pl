---
title: Get-GlpiToolsDropdownsCertificateTypes
---

## SYNOPSIS
Function is getting Certificate Types informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsCertificateTypes [-All] [<CommonParameters>]
```

### CertificateTypeId
```
Get-GlpiToolsDropdownsCertificateTypes -CertificateTypeId <String[]> [-Raw] [<CommonParameters>]
```

### CertificateTypeName
```
Get-GlpiToolsDropdownsCertificateTypes -CertificateTypeName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on CertificateTypeId which you can find in GLPI website
Returns object with property's of Certificate Types

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsCertificateTypes -All
```

Example will return all Certificate Types from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsCertificateTypes
```

Function gets CertificateTypeId from GLPI from Pipline, and return Certificate Types object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsCertificateTypes
```

Function gets CertificateTypeId from GLPI from Pipline (u can pass many ID's like that), and return Certificate Types object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsCertificateTypes -CertificateTypeId 326
```

Function gets CertificateTypeId from GLPI which is provided through -CertificateTypeId after Function type, and return Certificate Types object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsCertificateTypes -CertificateTypeId 326, 321
```

Function gets Certificate Types Id from GLPI which is provided through -CertificateTypeId keyword after Function type (u can provide many ID's like that), and return Certificate Types object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsCertificateTypes -CertificateTypeName Fusion
```

Example will return glpi Certificate Types, but what is the most important, Certificate Types will be shown exactly as you see in glpi dropdown Certificate Types.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Certificate Types from GLPI

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

### -CertificateTypeId
This parameter can take pipline input, either, you can use this function with -CertificateTypeId keyword.
Provide to this param CertificateTypeId from GLPI Certificate Types Bookmark

```yaml
Type: String[]
Parameter Sets: CertificateTypeId
Aliases: CTID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with CertificateTypeId Parameter.
CertificateTypeId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: CertificateTypeId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -CertificateTypeName
This parameter can take pipline input, either, you can use this function with -CertificateTypeId keyword.
Provide to this param Certificate Types Name from GLPI Certificate Types Bookmark

```yaml
Type: String
Parameter Sets: CertificateTypeName
Aliases: CTN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Certificate Types ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Certificate Types from GLPI
## NOTES
PSP 09/2019

## RELATED LINKS
