---
title: Get-GlpiToolsRacks
---

## SYNOPSIS
Function is getting Rack informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsRacks [-All] [<CommonParameters>]
```

### RackId
```
Get-GlpiToolsRacks -RackId <String[]> [-Raw] [-Parameter <String>] [<CommonParameters>]
```

### RackName
```
Get-GlpiToolsRacks -RackName <String> [-SearchInTrash <String>] [<CommonParameters>]
```

## DESCRIPTION
Function is based on RackID which you can find in GLPI website
Returns object with property's of Rack

## EXAMPLES

### EXAMPLE 1
```
326 | Get-GlpiToolsRacks
```

Function gets RackID from GLPI from Pipline, and return Rack object

### EXAMPLE 2
```
326, 321 | Get-GlpiToolsRacks
```

Function gets RackID from GLPI from Pipline (u can pass many ID's like that), and return Rack object

### EXAMPLE 3
```
Get-GlpiToolsRacks -RackId 326
```

Function gets RackID from GLPI which is provided through -RackId after Function type, and return Rack object

### EXAMPLE 4
```
Get-GlpiToolsRacks -RackId 326, 321
```

Function gets RackID from GLPI which is provided through -RackId keyword after Function type (u can provide many ID's like that), and return Rack object

### EXAMPLE 5
```
Get-GlpiToolsRacks -RackId 234 -Raw
```

Example will show Rack with id 234, but without any parameter converted

### EXAMPLE 6
```
234 | Get-GlpiToolsRacks -Raw
```

Example will show Rack with id 234, but without any parameter converted

### EXAMPLE 7
```
Get-GlpiToolsRacks -RackName glpi
```

Example will return glpi Rack, but what is the most important, Rack will be shown exacly as you see in glpi Racks tab.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

### EXAMPLE 8
```
Get-GlpiToolsRacks -RackName glpi -SearchInTrash Yes
```

Example will return glpi Rack, but from trash

## PARAMETERS

### -All
This parameter will return all Racks from GLPI

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

### -RackId
This parameter can take pipline input, either, you can use this function with -RackId keyword.
Provide to this param Rack ID from GLPI Racks Bookmark

```yaml
Type: String[]
Parameter Sets: RackId
Aliases: RID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with RackId Parameter.
RackId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: RackId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -RackName
Provide to this param Rack Name from GLPI Racks Bookmark

```yaml
Type: String
Parameter Sets: RackName
Aliases: RN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SearchInTrash
Parameter which you can use with RackName Parameter.
If you want Search for Rack name in trash, that parameter allow you to do it.

```yaml
Type: String
Parameter Sets: RackName
Aliases: SIT

Required: False
Position: Named
Default value: No
Accept pipeline input: False
Accept wildcard characters: False
```

### -Parameter
Parameter which you can use with RackId Parameter. 
If you want to get additional parameter of Rack object like, disks, or logs, use this parameter.

```yaml
Type: String
Parameter Sets: RackId
Aliases: Param

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Rack ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Racks from GLPI
## NOTES
PSP 05/2019

## RELATED LINKS
