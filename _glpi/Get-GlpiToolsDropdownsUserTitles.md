---
title: Get-GlpiToolsDropdownsUserTitles
---

## SYNOPSIS
Function is getting User Titles informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsUserTitles [-All] [<CommonParameters>]
```

### UserTitleId
```
Get-GlpiToolsDropdownsUserTitles -UserTitleId <String[]> [-Raw] [<CommonParameters>]
```

### UserTitleName
```
Get-GlpiToolsDropdownsUserTitles -UserTitleName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on UserTitleId which you can find in GLPI website
Returns object with property's of User Titles

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsUserTitles -All
```

Example will return all User Titles from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsUserTitles
```

Function gets UserTitleId from GLPI from Pipline, and return User Titles object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsUserTitles
```

Function gets UserTitleId from GLPI from Pipline (u can pass many ID's like that), and return User Titles object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsUserTitles -UserTitleId 326
```

Function gets UserTitleId from GLPI which is provided through -UserTitleId after Function type, and return User Titles object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsUserTitles -UserTitleId 326, 321
```

Function gets User TitlesId from GLPI which is provided through -UserTitleId keyword after Function type (u can provide many ID's like that), and return User Titles object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsUserTitles -UserTitleName Fusion
```

Example will return glpi User Titles, but what is the most important, User Titles will be shown exactly as you see in glpi dropdown User Titles.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all User Titles from GLPI

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

### -UserTitleId
This parameter can take pipline input, either, you can use this function with -UserTitleId keyword.
Provide to this param UserTitleId from GLPI User Titles Bookmark

```yaml
Type: String[]
Parameter Sets: UserTitleId
Aliases: UTID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with UserTitleId Parameter.
UserTitleId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: UserTitleId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -UserTitleName
This parameter can take pipline input, either, you can use this function with -UserTitleId keyword.
Provide to this param User Titles Name from GLPI User Titles Bookmark

```yaml
Type: String
Parameter Sets: UserTitleName
Aliases: UTN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### User Titles ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of User Titles from GLPI
## NOTES
PSP 08/2019

## RELATED LINKS
