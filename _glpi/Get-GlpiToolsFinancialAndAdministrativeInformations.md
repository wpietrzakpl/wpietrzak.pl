---
title: Get-GlpiToolsFinancialAndAdministrativeInformations
---

## SYNOPSIS
Function is getting FinancialAndAdminstrativeId informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsFinancialAndAdministrativeInformations [-All] [<CommonParameters>]
```

### FinancialAndAdminstrativeId
```
Get-GlpiToolsFinancialAndAdministrativeInformations -FinancialAndAdminstrativeId <String[]> [-Raw]
 [<CommonParameters>]
```

## DESCRIPTION
Function is based on FinancialAndAdminstrativeId which you can find in GLPI website
Returns object with property's of FinancialAndAdminstrativeId Tab

## EXAMPLES

### EXAMPLE 1
```
326 | Get-GlpiToolsFinancialAndAdministrativeInformations
```

Function gets FinancialAndAdminstrativeId from GLPI from Pipline, and return FinancialAndAdminstrative object

### EXAMPLE 2
```
326, 321 | Get-GlpiToolsFinancialAndAdministrativeInformations
```

Function gets FinancialAndAdminstrativeId from GLPI from Pipline (u can pass many ID's like that), and return FinancialAndAdminstrative object

### EXAMPLE 3
```
Get-GlpiToolsFinancialAndAdministrativeInformations -FinancialAndAdminstrativeId 326
```

Function gets FinancialAndAdminstrativeId from GLPI which is provided through -FinancialAndAdminstrativeId after Function type, and return FinancialAndAdminstrative object

### EXAMPLE 4
```
Get-GlpiToolsFinancialAndAdministrativeInformations -FinancialAndAdminstrativeId 326, 321
```

Function gets FinancialAndAdminstrativeId from GLPI which is provided through -FinancialAndAdminstrativeId keyword after Function type (u can provide many ID's like that), and return FinancialAndAdminstrative object

### EXAMPLE 5
```
Get-GlpiToolsFinancialAndAdministrativeInformations -FinancialAndAdminstrativeId 234 -Raw
```

Example will show FinancialAndAdminstrativeId with id 234, but without any parameter converted

### EXAMPLE 6
```
234 | Get-GlpiToolsFinancialAndAdministrativeInformations -Raw
```

Example will show FinancialAndAdminstrativeId with id 234, but without any parameter converted

## PARAMETERS

### -All
This parameter will return all FinancialAndAdminstrativeId informations for All Assets from GLPI

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

### -FinancialAndAdminstrativeId
This parameter can take pipline input, either, you can use this function with -FinancialAndAdminstrativeId keyword.
Provide to this param FinancialAndAdminstrativeId ID running this function before with parameter All to retrieve id's

```yaml
Type: String[]
Parameter Sets: FinancialAndAdminstrativeId
Aliases: FAAID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with FinancialAndAdminstrativeId Parameter.
FinancialAndAdminstrativeId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: FinancialAndAdminstrativeId
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

### FinancialAndAdminstrativeIdID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Financial And Adminstrative Tab from GLPI
## NOTES
PSP 08/2018

## RELATED LINKS
