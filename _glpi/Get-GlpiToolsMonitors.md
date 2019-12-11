---
title: Get-GlpiToolsMonitors
---

## SYNOPSIS
Function is getting Monitor informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsMonitors [-All] [<CommonParameters>]
```

### MonitorId
```
Get-GlpiToolsMonitors -MonitorId <String[]> [-Raw] [-Parameter <String>] [<CommonParameters>]
```

### MonitorName
```
Get-GlpiToolsMonitors -MonitorName <String> [-SearchInTrash <String>] [<CommonParameters>]
```

## DESCRIPTION
Function is based on MonitorID which you can find in GLPI website
Returns object with property's of Monitor

## EXAMPLES

### EXAMPLE 1
```
326 | Get-GlpiToolsMonitors
```

Function gets MonitorID from GLPI from Pipline, and return Monitor object

### EXAMPLE 2
```
326, 321 | Get-GlpiToolsMonitors
```

Function gets MonitorID from GLPI from Pipline (u can pass many ID's like that), and return Monitor object

### EXAMPLE 3
```
Get-GlpiToolsMonitors -MonitorId 326
```

Function gets MonitorID from GLPI which is provided through -MonitorId after Function type, and return Monitor object

### EXAMPLE 4
```
Get-GlpiToolsMonitors -MonitorId 326, 321
```

Function gets MonitorID from GLPI which is provided through -MonitorId keyword after Function type (u can provide many ID's like that), and return Monitor object

### EXAMPLE 5
```
Get-GlpiToolsMonitors -MonitorId 234 -Raw
```

Example will show Monitor with id 234, but without any parameter converted

### EXAMPLE 6
```
234 | Get-GlpiToolsMonitors -Raw
```

Example will show Monitor with id 234, but without any parameter converted

### EXAMPLE 7
```
Get-GlpiToolsMonitors -MonitorName glpi
```

Example will return glpi Monitor, but what is the most important, Monitor will be shown exacly as you see in glpi Monitors tab.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

### EXAMPLE 8
```
Get-GlpiToolsMonitors -MonitorName glpi -SearchInTrash Yes
```

Example will return glpi Monitor, but from trash

## PARAMETERS

### -All
This parameter will return all Monitors from GLPI

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

### -MonitorId
This parameter can take pipline input, either, you can use this function with -MonitorId keyword.
Provide to this param Monitor ID from GLPI Monitors Bookmark

```yaml
Type: String[]
Parameter Sets: MonitorId
Aliases: MID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with MonitorId Parameter.
MonitorId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: MonitorId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -MonitorName
Provide to this param Monitor Name from GLPI Monitors Bookmark

```yaml
Type: String
Parameter Sets: MonitorName
Aliases: MN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SearchInTrash
Parameter which you can use with MonitorName Parameter.
If you want Search for Monitor name in trash, that parameter allow you to do it.

```yaml
Type: String
Parameter Sets: MonitorName
Aliases: SIT

Required: False
Position: Named
Default value: No
Accept pipeline input: False
Accept wildcard characters: False
```

### -Parameter
Parameter which you can use with MonitorId Parameter. 
If you want to get additional parameter of Monitor object like, disks, or logs, use this parameter.

```yaml
Type: String
Parameter Sets: MonitorId
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

### Monitor ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Monitors from GLPI
## NOTES
PSP 05/2019

## RELATED LINKS
