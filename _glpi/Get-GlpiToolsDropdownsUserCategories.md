---
title: Get-GlpiToolsDropdownsUserCategories
---

## SYNOPSIS
Function is getting User Categories informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsUserCategories [-All] [<CommonParameters>]
```

### UserCategoryId
```
Get-GlpiToolsDropdownsUserCategories -UserCategoryId <String[]> [-Raw] [<CommonParameters>]
```

### UserCategoryName
```
Get-GlpiToolsDropdownsUserCategories -UserCategoryName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on UserCategoryId which you can find in GLPI website
Returns object with property's of User Categories

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsUserCategories -All
```

Example will return all User Categories from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsUserCategories
```

Function gets UserCategoryId from GLPI from Pipline, and return User Categories object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsUserCategories
```

Function gets UserCategoryId from GLPI from Pipline (u can pass many ID's like that), and return User Categories object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsUserCategories -UserCategoryId 326
```

Function gets UserCategoryId from GLPI which is provided through -UserCategoryId after Function type, and return User Categories object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsUserCategories -UserCategoryId 326, 321
```

Function gets User CategoriesId from GLPI which is provided through -UserCategoryId keyword after Function type (u can provide many ID's like that), and return User Categories object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsUserCategories -UserCategoryName Fusion
```

Example will return glpi User Categories, but what is the most important, User Categories will be shown exactly as you see in glpi dropdown User Categories.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all User Categories from GLPI

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

### -UserCategoryId
This parameter can take pipline input, either, you can use this function with -UserCategoryId keyword.
Provide to this param UserCategoryId from GLPI User Categories Bookmark

```yaml
Type: String[]
Parameter Sets: UserCategoryId
Aliases: UCID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with UserCategoryId Parameter.
UserCategoryId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: UserCategoryId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -UserCategoryName
This parameter can take pipline input, either, you can use this function with -UserCategoryId keyword.
Provide to this param User Categories Name from GLPI User Categories Bookmark

```yaml
Type: String
Parameter Sets: UserCategoryName
Aliases: UCN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### User Categories ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of User Categories from GLPI
## NOTES
PSP 08/2019

## RELATED LINKS
