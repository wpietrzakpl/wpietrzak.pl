---
title: Get-GlpiToolsComputerSoftwareVersions
---

## SYNOPSIS
Function is getting Computer Software Version informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsComputerSoftwareVersions [-All] [<CommonParameters>]
```

### ComputerSoftwareVersionId
```
Get-GlpiToolsComputerSoftwareVersions -ComputerSoftwareVersionId <String[]> [-Raw] [<CommonParameters>]
```

## DESCRIPTION
Function is based on Computer Software Version ID which you can find in GLPI website
Returns object with property's of Computer Software Version

## EXAMPLES

### EXAMPLE 1
```
326 | Get-GlpiToolsComputerSoftwareVersions
```

Function gets ComputerSoftwareVersionId from GLPI from Pipline, and return Computer Software Version object

### EXAMPLE 2
```
326, 321 | Get-GlpiToolsComputerSoftwareVersions
```

Function gets ComputerSoftwareVersionId from GLPI from Pipline (u can pass many ID's like that), and return Computer Software Version object

### EXAMPLE 3
```
Get-GlpiToolsComputerSoftwareVersions -ComputerSoftwareVersionId 326
```

Function gets ComputerSoftwareVersionId from GLPI which is provided through -ComputerSoftwareVersionId after Function type, and return Computer Software Version object

### EXAMPLE 4
```
Get-GlpiToolsComputerSoftwareVersions -ComputerSoftwareVersionId 326, 321
```

Function gets ComputerSoftwareVersionId from GLPI which is provided through -ComputerSoftwareVersionId keyword after Function type (u can provide many ID's like that), and return Computer Software Version object

### EXAMPLE 5
```
Get-GlpiToolsComputerSoftwareVersions -ComputerSoftwareVersionId 234 -Raw
```

Example will show Computer Software Version with id 234, but without any parameter converted

### EXAMPLE 6
```
234 | Get-GlpiToolsComputerSoftwareVersions -Raw
```

Example will show Computer Software Version with id 234, but without any parameter converted

## PARAMETERS

### -All
This parameter will return all Computer Software Versions from GLPI

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

### -ComputerSoftwareVersionId
This parameter can take pipline input, either, you can use this function with -ComputerSoftwareVersionId keyword.
Provide to this param Computer Software Version ID from GLPI

```yaml
Type: String[]
Parameter Sets: ComputerSoftwareVersionId
Aliases: CSVID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with ComputerSoftwareVersionId Parameter.
ComputerSoftwareVersionId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: ComputerSoftwareVersionId
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

### Computer Software Version ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Computer Software Versions from GLPI
## NOTES
PSP 08/2019

## RELATED LINKS
