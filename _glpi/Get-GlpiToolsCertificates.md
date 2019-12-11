---
title: Get-GlpiToolsCertificates
---

## SYNOPSIS
Function is getting Certificate informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsCertificates [-All] [<CommonParameters>]
```

### CertificateId
```
Get-GlpiToolsCertificates -CertificateId <String[]> [-Raw] [<CommonParameters>]
```

### CertificateName
```
Get-GlpiToolsCertificates -CertificateName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on CertificateId which you can find in GLPI website
Returns object with property's of Certificate

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsCertificates -All
```

Example will return all Certificate from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsCertificates
```

Function gets CertificateId from GLPI from PipCertificate, and return Certificate object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsCertificates
```

Function gets CertificateId from GLPI from PipCertificate (u can pass many ID's like that), and return Certificate object

### EXAMPLE 4
```
Get-GlpiToolsCertificates -CertificateId 326
```

Function gets CertificateId from GLPI which is provided through -CertificateId after Function type, and return Certificate object

### EXAMPLE 5
```
Get-GlpiToolsCertificates -CertificateId 326, 321
```

Function gets Certificate Id from GLPI which is provided through -CertificateId keyword after Function type (u can provide many ID's like that), and return Certificate object

### EXAMPLE 6
```
Get-GlpiToolsCertificates -CertificateName Fusion
```

Example will return glpi Certificate, but what is the most important, Certificate will be shown exactly as you see in glpi dropdown Certificate.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Certificate from GLPI

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

### -CertificateId
This parameter can take pipCertificate input, either, you can use this function with -CertificateId keyword.
Provide to this param CertificateId from GLPI Certificate Bookmark

```yaml
Type: String[]
Parameter Sets: CertificateId
Aliases: CID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with CertificateId Parameter.
CertificateId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: CertificateId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -CertificateName
This parameter can take pipCertificate input, either, you can use this function with -CertificateId keyword.
Provide to this param Certificate Name from GLPI Certificate Bookmark

```yaml
Type: String
Parameter Sets: CertificateName
Aliases: CN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Certificate ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Certificate from GLPI
## NOTES
PSP 11/2019

## RELATED LINKS
