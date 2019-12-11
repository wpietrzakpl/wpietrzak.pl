---
title: Get-GlpiToolsDropdownsDomains
---

## SYNOPSIS
Function is getting Domain informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsDomains [-All] [<CommonParameters>]
```

### DomainId
```
Get-GlpiToolsDropdownsDomains -DomainId <String[]> [-Raw] [<CommonParameters>]
```

### DomainName
```
Get-GlpiToolsDropdownsDomains -DomainName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on DomainID which you can find in GLPI website
Returns object with property's of Domain

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsDomains -All
```

Example will return all Domain from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsDomains
```

Function gets DomainId from GLPI from Pipline, and return Domain object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsDomains
```

Function gets DomainId from GLPI from Pipline (u can pass many ID's like that), and return Domain object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsDomains -DomainId 326
```

Function gets DomainId from GLPI which is provided through -DomainId after Function type, and return Domain object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsDomains -DomainId 326, 321
```

Function gets DomainId from GLPI which is provided through -DomainId keyword after Function type (u can provide many ID's like that), and return Domain object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsDomains -DomainName Fusion
```

Example will return glpi Domain, but what is the most important, Domain will be shown exactly as you see in glpi dropdown Domain.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Domain from GLPI

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

### -DomainId
This parameter can take pipline input, either, you can use this function with -DomainId keyword.
Provide to this param Domain ID from GLPI Domain Bookmark

```yaml
Type: String[]
Parameter Sets: DomainId
Aliases: DID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with DomainId Parameter.
DomainId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: DomainId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -DomainName
This parameter can take pipline input, either, you can use this function with -DomainName keyword.
Provide to this param Domain Name from GLPI Domain Bookmark

```yaml
Type: String
Parameter Sets: DomainName
Aliases: DN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Domain ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Domain from GLPI
## NOTES
PSP 06/2019

## RELATED LINKS
