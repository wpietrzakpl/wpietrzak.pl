---
title: Get-GlpiToolsGroups
---

## SYNOPSIS
Function is getting Group informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsGroups [-All] [<CommonParameters>]
```

### GroupId
```
Get-GlpiToolsGroups -GroupId <String[]> [-Raw] [<CommonParameters>]
```

### GroupName
```
Get-GlpiToolsGroups -GroupName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on GroupID which you can find in GLPI website
Returns object with property's of group

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsGroups -All
```

Example will return all Groups from Groups.

### EXAMPLE 2
```
326 | Get-GlpiToolsGroups
```

Function gets GroupID from GLPI from Pipline, and return Group object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsGroups
```

Function gets GroupID from GLPI from Pipline (u can pass many ID's like that), and return Group object

### EXAMPLE 4
```
Get-GlpiToolsGroups -GroupId 326
```

Function gets GroupID from GLPI which is provided through -GroupId after Function type, and return Group object

### EXAMPLE 5
```
Get-GlpiToolsGroups -GroupId 326, 321
```

Function gets GroupID from GLPI which is provided through -GroupId keyword after Function type (u can provide many ID's like that), and return Group object

### EXAMPLE 6
```
Get-GlpiToolsGroups -GroupId 234 -Raw
```

Example will show Group with id 234, but without any parameter converted

### EXAMPLE 7
```
234 | Get-GlpiToolsGroups -Raw
```

Example will show Group with id 234, but without any parameter converted

### EXAMPLE 8
```
Get-GlpiToolsGroups -GroupName glpi
```

Example will return glpi Group, but what is the most important, Group will be shown exactly as you see in glpi Groups tab.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Groups from GLPI

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

### -GroupId
This parameter can take pipline input, either, you can use this function with -GroupId keyword.
Provide to this param Group ID from GLPI Group Bookmark

```yaml
Type: String[]
Parameter Sets: GroupId
Aliases: GID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with GroupId Parameter.
GroupId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: GroupId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -GroupName
This parameter can take pipline input, either, you can use this function with -GroupName keyword.
Provide to this param Group Name from GLPI Group Bookmark

```yaml
Type: String
Parameter Sets: GroupName
Aliases: GN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Group ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Groups from GLPI
## NOTES
PSP 03/2019

## RELATED LINKS
