---
title: Get-GlpiToolsPeripherals
---

## SYNOPSIS
Function is getting Peripheral informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsPeripherals [-All] [<CommonParameters>]
```

### PeripheralId
```
Get-GlpiToolsPeripherals -PeripheralId <String[]> [-Raw] [-Parameter <String>] [<CommonParameters>]
```

### PeripheralName
```
Get-GlpiToolsPeripherals -PeripheralName <String> [-SearchInTrash <String>] [<CommonParameters>]
```

## DESCRIPTION
Function is based on PeripheralID which you can find in GLPI website
Returns object with property's of Peripheral

## EXAMPLES

### EXAMPLE 1
```
326 | Get-GlpiToolsPeripherals
```

Function gets PeripheralID from GLPI from Pipline, and return Peripheral object

### EXAMPLE 2
```
326, 321 | Get-GlpiToolsPeripherals
```

Function gets PeripheralID from GLPI from Pipline (u can pass many ID's like that), and return Peripheral object

### EXAMPLE 3
```
Get-GlpiToolsPeripherals -PeripheralId 326
```

Function gets PeripheralID from GLPI which is provided through -PeripheralId after Function type, and return Peripheral object

### EXAMPLE 4
```
Get-GlpiToolsPeripherals -PeripheralId 326, 321
```

Function gets PeripheralID from GLPI which is provided through -PeripheralId keyword after Function type (u can provide many ID's like that), and return Peripheral object

### EXAMPLE 5
```
Get-GlpiToolsPeripherals -PeripheralId 234 -Raw
```

Example will show Peripheral with id 234, but without any parameter converted

### EXAMPLE 6
```
234 | Get-GlpiToolsPeripherals -Raw
```

Example will show Peripheral with id 234, but without any parameter converted

### EXAMPLE 7
```
Get-GlpiToolsPeripherals -PeripheralName glpi
```

Example will return glpi Peripheral, but what is the most important, Peripheral will be shown exacly as you see in glpi Peripherals tab.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

### EXAMPLE 8
```
Get-GlpiToolsPeripherals -PeripheralName glpi -SearchInTrash Yes
```

Example will return glpi Peripheral, but from trash

## PARAMETERS

### -All
This parameter will return all Peripherals from GLPI

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

### -PeripheralId
This parameter can take pipline input, either, you can use this function with -PeripheralId keyword.
Provide to this param Peripheral ID from GLPI Peripherals Bookmark

```yaml
Type: String[]
Parameter Sets: PeripheralId
Aliases: PID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with PeripheralId Parameter.
PeripheralId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: PeripheralId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -PeripheralName
Provide to this param Peripheral Name from GLPI Peripherals Bookmark

```yaml
Type: String
Parameter Sets: PeripheralName
Aliases: PN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SearchInTrash
Parameter which you can use with PeripheralName Parameter.
If you want Search for Peripheral name in trash, that parameter allow you to do it.

```yaml
Type: String
Parameter Sets: PeripheralName
Aliases: SIT

Required: False
Position: Named
Default value: No
Accept pipeline input: False
Accept wildcard characters: False
```

### -Parameter
Parameter which you can use with PeripheralId Parameter. 
If you want to get additional parameter of Peripheral object like, disks, or logs, use this parameter.

```yaml
Type: String
Parameter Sets: PeripheralId
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

### Peripheral ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Peripherals from GLPI
## NOTES
PSP 05/2019

## RELATED LINKS
