---
title: Get-GlpiToolsGroupsMembers
---

## SYNOPSIS
Function is getting Group Members informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsGroupsMembers [-All] [<CommonParameters>]
```

### GroupMemberId
```
Get-GlpiToolsGroupsMembers -GroupMemberId <String[]> [-Raw] [<CommonParameters>]
```

## DESCRIPTION
Function is based on GroupMemberId which you can find in GLPI website
Returns object with property's of Group Members

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsGroupsMembers -All
```

Example will return all Group Members from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsGroupsMembers
```

Function gets GroupMemberId from GLPI from pipeline, and return Group Members object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsGroupsMembers
```

Function gets GroupMemberId from GLPI from pipeline (u can pass many ID's like that), and return Group Members object

### EXAMPLE 4
```
Get-GlpiToolsGroupsMembers -GroupMemberId 326
```

Function gets GroupMemberId from GLPI which is provided through -GroupMemberId after Function type, and return Group Members object

### EXAMPLE 5
```
Get-GlpiToolsGroupsMembers -GroupMemberId 326, 321
```

Function gets Group Members Id from GLPI which is provided through -GroupMemberId keyword after Function type (u can provide many ID's like that), and return Group Members object

## PARAMETERS

### -All
This parameter will return all Group Members from GLPI

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

### -GroupMemberId
This parameter can take pipeline input, either, you can use this function with -GroupMemberId keyword.
Provide to this param GroupMemberId from GLPI Group Members Bookmark

```yaml
Type: String[]
Parameter Sets: GroupMemberId
Aliases: GMID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with GroupMemberId Parameter.
GroupMemberId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: GroupMemberId
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

### Group Members ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Group Members from GLPI
## NOTES
PSP 09/2019

## RELATED LINKS
