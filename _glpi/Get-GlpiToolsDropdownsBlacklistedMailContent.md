---
title: Get-GlpiToolsDropdownsBlacklistedMailContent
---

## SYNOPSIS
Function is getting Blacklisted Mail Content informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsBlacklistedMailContent [-All] [<CommonParameters>]
```

### BlacklistedMailContentId
```
Get-GlpiToolsDropdownsBlacklistedMailContent -BlacklistedMailContentId <String[]> [-Raw] [<CommonParameters>]
```

### BlacklistedMailContentName
```
Get-GlpiToolsDropdownsBlacklistedMailContent -BlacklistedMailContentName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on BlacklistedMailContentId which you can find in GLPI website
Returns object with property's of Blacklisted Mail Content

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsBlacklistedMailContent -All
```

Example will return all Blacklisted Mail Content from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsBlacklistedMailContent
```

Function gets BlacklistedMailContentId from GLPI from Pipline, and return Blacklisted Mail Content object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsBlacklistedMailContent
```

Function gets BlacklistedMailContentId from GLPI from Pipline (u can pass many ID's like that), and return Blacklisted Mail Content object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsBlacklistedMailContent -BlacklistedMailContentId 326
```

Function gets BlacklistedMailContentId from GLPI which is provided through -BlacklistedMailContentId after Function type, and return Blacklisted Mail Content object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsBlacklistedMailContent -BlacklistedMailContentId 326, 321
```

Function gets Blacklisted Mail ContentId from GLPI which is provided through -Blacklisted Mail ContentId keyword after Function type (u can provide many ID's like that), and return Blacklisted Mail Content object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsBlacklistedMailContent -BlacklistedMailContentName Fusion
```

Example will return glpi Blacklisted Mail Content, but what is the most important, Blacklisted Mail Content will be shown exactly as you see in glpi dropdown Blacklisted Mail Content.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Blacklisted Mail Content from GLPI

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

### -BlacklistedMailContentId
This parameter can take pipline input, either, you can use this function with -BlacklistedMailContentId keyword.
Provide to this param BlacklistedMailContentID from GLPI Blacklisted Mail Content Bookmark

```yaml
Type: String[]
Parameter Sets: BlacklistedMailContentId
Aliases: BMCID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with BlacklistedMailContentId Parameter.
BlacklistedMailContentId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: BlacklistedMailContentId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -BlacklistedMailContentName
This parameter can take pipline input, either, you can use this function with -BlacklistedMailContentId keyword.
Provide to this param Blacklisted Mail Content Name from GLPI Blacklisted Mail Content Bookmark

```yaml
Type: String
Parameter Sets: BlacklistedMailContentName
Aliases: BMCN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Blacklisted Mail Content ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Blacklisted Mail Content from GLPI
## NOTES
PSP 08/2019

## RELATED LINKS
