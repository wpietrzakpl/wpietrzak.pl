---
title: Get-GlpiToolsComputers
---

## SYNOPSIS
Function is getting Computer informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsComputers [-All] [<CommonParameters>]
```

### ComputerId
```
Get-GlpiToolsComputers -ComputerId <String[]> [-Raw] [-Parameter <String>] [<CommonParameters>]
```

### ComputerName
```
Get-GlpiToolsComputers -ComputerName <String> [-SearchInTrash <String>] [<CommonParameters>]
```

## DESCRIPTION
Function is based on ComputerID which you can find in GLPI website
Returns object with property's of computer

## EXAMPLES

### EXAMPLE 1
```
326 | Get-GlpiToolsComputers
```

Function gets ComputerID from GLPI from Pipline, and return Computer object

### EXAMPLE 2
```
326, 321 | Get-GlpiToolsComputers
```

Function gets ComputerID from GLPI from Pipline (u can pass many ID's like that), and return Computer object

### EXAMPLE 3
```
Get-GlpiToolsComputers -ComputerId 326
```

Function gets ComputerID from GLPI which is provided through -ComputerId after Function type, and return Computer object

### EXAMPLE 4
```
Get-GlpiToolsComputers -ComputerId 326, 321
```

Function gets ComputerID from GLPI which is provided through -ComputerId keyword after Function type (u can provide many ID's like that), and return Computer object

### EXAMPLE 5
```
Get-GlpiToolsComputers -ComputerId 234 -Raw
```

Example will show Computer with id 234, but without any parameter converted

### EXAMPLE 6
```
234 | Get-GlpiToolsComputers -Raw
```

Example will show Computer with id 234, but without any parameter converted

### EXAMPLE 7
```
Get-GlpiToolsComputers -ComputerName glpi
```

Example will return glpi Computer, but what is the most important, Computer will be shown exacly as you see in glpi Computers tab.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

### EXAMPLE 8
```
Get-GlpiToolsComputers -ComputerName glpi -SearchInTrash Yes
```

Example will return glpi Computer, but from trash

## PARAMETERS

### -All
This parameter will return all computers from GLPI

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

### -ComputerId
This parameter can take pipline input, either, you can use this function with -ComputerId keyword.
Provide to this param Computer ID from GLPI Computers Bookmark

```yaml
Type: String[]
Parameter Sets: ComputerId
Aliases: CID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with ComputerId Parameter.
ComputerId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: ComputerId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -ComputerName
Provide to this param Computer Name from GLPI Computers Bookmark

```yaml
Type: String
Parameter Sets: ComputerName
Aliases: CN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SearchInTrash
Parameter which you can use with ComputerName Parameter.
If you want Search for computer name in trash, that parameter allow you to do it.

```yaml
Type: String
Parameter Sets: ComputerName
Aliases: SIT

Required: False
Position: Named
Default value: No
Accept pipeline input: False
Accept wildcard characters: False
```

### -Parameter
Parameter which you can use with ComputerId Parameter. 
If you want to get additional parameter of computer object like, disks, or logs, use this parameter.

```yaml
Type: String
Parameter Sets: ComputerId
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

### Computer ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of computers from GLPI
## NOTES
PSP 12/2018

## RELATED LINKS
