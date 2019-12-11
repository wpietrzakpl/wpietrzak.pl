---
title: Get-GlpiToolsRecurrentTickets
---

## SYNOPSIS
Function is getting RecurrentTicket informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsRecurrentTickets [-All] [<CommonParameters>]
```

### RecurrentTicketId
```
Get-GlpiToolsRecurrentTickets -RecurrentTicketId <String[]> [-Raw] [-Parameter <String>] [<CommonParameters>]
```

### RecurrentTicketName
```
Get-GlpiToolsRecurrentTickets -RecurrentTicketName <String> [-SearchInTrash <String>] [<CommonParameters>]
```

## DESCRIPTION
Function is based on RecurrentTicketID which you can find in GLPI website
Returns object with property's of RecurrentTicket

## EXAMPLES

### EXAMPLE 1
```
326 | Get-GlpiToolsRecurrentTickets
```

Function gets RecurrentTicketID from GLPI from Pipline, and return RecurrentTicket object

### EXAMPLE 2
```
326, 321 | Get-GlpiToolsRecurrentTickets
```

Function gets RecurrentTicketID from GLPI from Pipline (u can pass many ID's like that), and return RecurrentTicket object

### EXAMPLE 3
```
Get-GlpiToolsRecurrentTickets -RecurrentTicketId 326
```

Function gets RecurrentTicketID from GLPI which is provided through -RecurrentTicketId after Function type, and return RecurrentTicket object

### EXAMPLE 4
```
Get-GlpiToolsRecurrentTickets -RecurrentTicketId 326, 321
```

Function gets RecurrentTicketID from GLPI which is provided through -RecurrentTicketId keyword after Function type (u can provide many ID's like that), and return RecurrentTicket object

### EXAMPLE 5
```
Get-GlpiToolsRecurrentTickets -RecurrentTicketId 234 -Raw
```

Example will show RecurrentTicket with id 234, but without any parameter converted

### EXAMPLE 6
```
234 | Get-GlpiToolsRecurrentTickets -Raw
```

Example will show RecurrentTicket with id 234, but without any parameter converted

### EXAMPLE 7
```
Get-GlpiToolsRecurrentTickets -RecurrentTicketName glpi
```

Example will return glpi RecurrentTicket, but what is the most important, RecurrentTicket will be shown exacly as you see in glpi RecurrentTickets tab.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

### EXAMPLE 8
```
Get-GlpiToolsRecurrentTickets -RecurrentTicketName glpi -SearchInTrash Yes
```

Example will return glpi RecurrentTicket, but from trash

## PARAMETERS

### -All
This parameter will return all RecurrentTickets from GLPI

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

### -RecurrentTicketId
This parameter can take pipline input, either, you can use this function with -RecurrentTicketId keyword.
Provide to this param RecurrentTicket ID from GLPI RecurrentTickets Bookmark

```yaml
Type: String[]
Parameter Sets: RecurrentTicketId
Aliases: RTID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with RecurrentTicketId Parameter.
RecurrentTicketId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: RecurrentTicketId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -RecurrentTicketName
Provide to this param RecurrentTicket Name from GLPI RecurrentTickets Bookmark

```yaml
Type: String
Parameter Sets: RecurrentTicketName
Aliases: RTN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SearchInTrash
Parameter which you can use with RecurrentTicketName Parameter.
If you want Search for RecurrentTicket name in trash, that parameter allow you to do it.

```yaml
Type: String
Parameter Sets: RecurrentTicketName
Aliases: SIT

Required: False
Position: Named
Default value: No
Accept pipeline input: False
Accept wildcard characters: False
```

### -Parameter
Parameter which you can use with RecurrentTicketId Parameter. 
If you want to get additional parameter of RecurrentTicket object like, disks, or logs, use this parameter.

```yaml
Type: String
Parameter Sets: RecurrentTicketId
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

### RecurrentTicket ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of RecurrentTickets from GLPI
## NOTES
PSP 05/2019

## RELATED LINKS
