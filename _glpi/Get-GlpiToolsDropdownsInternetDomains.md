---
title: Get-GlpiToolsDropdownsInternetDomains
---

## SYNOPSIS
Function is getting Internet Domains informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsInternetDomains [-All] [<CommonParameters>]
```

### InternetDomainId
```
Get-GlpiToolsDropdownsInternetDomains -InternetDomainId <String[]> [-Raw] [<CommonParameters>]
```

### InternetDomainName
```
Get-GlpiToolsDropdownsInternetDomains -InternetDomainName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on InternetDomainId which you can find in GLPI website
Returns object with property's of Internet Domains

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsInternetDomains -All
```

Example will return all Internet Domains from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsInternetDomains
```

Function gets InternetDomainId from GLPI from pipeline, and return Internet Domains object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsInternetDomains
```

Function gets InternetDomainId from GLPI from pipeline (u can pass many ID's like that), and return Internet Domains object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsInternetDomains -InternetDomainId 326
```

Function gets InternetDomainId from GLPI which is provided through -InternetDomainId after Function type, and return Internet Domains object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsInternetDomains -InternetDomainId 326, 321
```

Function gets Internet Domains Id from GLPI which is provided through -InternetDomainId keyword after Function type (u can provide many ID's like that), and return Internet Domains object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsInternetDomains -InternetDomainName Fusion
```

Example will return glpi Internet Domains, but what is the most important, Internet Domains will be shown exactly as you see in glpi dropdown Internet Domains.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Internet Domains from GLPI

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

### -InternetDomainId
This parameter can take pipeline input, either, you can use this function with -InternetDomainId keyword.
Provide to this param InternetDomainId from GLPI Internet Domains Bookmark

```yaml
Type: String[]
Parameter Sets: InternetDomainId
Aliases: IDID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with InternetDomainId Parameter.
InternetDomainId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: InternetDomainId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -InternetDomainName
This parameter can take pipeline input, either, you can use this function with -InternetDomainId keyword.
Provide to this param Internet Domains Name from GLPI Internet Domains Bookmark

```yaml
Type: String
Parameter Sets: InternetDomainName
Aliases: IDN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Internet Domains ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Internet Domains from GLPI
## NOTES
PSP 09/2019

## RELATED LINKS
