---
title: Get-GlpiToolsTickets
---

## SYNOPSIS
Function is getting Ticket informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsTickets [-All] [<CommonParameters>]
```

### TicketId
```
Get-GlpiToolsTickets -TicketId <String[]> [-Raw] [-Parameter <String>] [<CommonParameters>]
```

### TicketName
```
Get-GlpiToolsTickets -TicketName <String> [-SearchInTrash <String>] [<CommonParameters>]
```

## DESCRIPTION
Function is based on TicketID which you can find in GLPI website
Returns object with property's of Ticket

## EXAMPLES

### EXAMPLE 1
```
326 | Get-GlpiToolsTickets
```

Function gets TicketID from GLPI from Pipline, and return Ticket object

### EXAMPLE 2
```
326, 321 | Get-GlpiToolsTickets
```

Function gets TicketID from GLPI from Pipline (u can pass many ID's like that), and return Ticket object

### EXAMPLE 3
```
Get-GlpiToolsTickets -TicketId 326
```

Function gets TicketID from GLPI which is provided through -TicketId after Function type, and return Ticket object

### EXAMPLE 4
```
Get-GlpiToolsTickets -TicketId 326, 321
```

Function gets TicketID from GLPI which is provided through -TicketId keyword after Function type (u can provide many ID's like that), and return Ticket object

### EXAMPLE 5
```
Get-GlpiToolsTickets -TicketId 234 -Raw
```

Example will show Ticket with id 234, but without any parameter converted

### EXAMPLE 6
```
234 | Get-GlpiToolsTickets -Raw
```

Example will show Ticket with id 234, but without any parameter converted

### EXAMPLE 7
```
Get-GlpiToolsTickets -TicketName glpi
```

Example will return glpi Ticket, but what is the most important, Ticket will be shown exacly as you see in glpi Tickets tab.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

### EXAMPLE 8
```
Get-GlpiToolsTickets -TicketName glpi -SearchInTrash Yes
```

Example will return glpi Ticket, but from trash

## PARAMETERS

### -All
This parameter will return all Tickets from GLPI

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

### -TicketId
This parameter can take pipline input, either, you can use this function with -TicketId keyword.
Provide to this param Ticket ID from GLPI Tickets Bookmark

```yaml
Type: String[]
Parameter Sets: TicketId
Aliases: TID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with TicketId Parameter.
TicketId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: TicketId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -TicketName
Provide to this param Ticket Name from GLPI Tickets Bookmark

```yaml
Type: String
Parameter Sets: TicketName
Aliases: TN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SearchInTrash
Parameter which you can use with TicketName Parameter.
If you want Search for Ticket name in trash, that parameter allow you to do it.

```yaml
Type: String
Parameter Sets: TicketName
Aliases: SIT

Required: False
Position: Named
Default value: No
Accept pipeline input: False
Accept wildcard characters: False
```

### -Parameter
Parameter which you can use with TicketId Parameter. 
If you want to get additional parameter of Ticket object like, disks, or logs, use this parameter.

```yaml
Type: String
Parameter Sets: TicketId
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

### Ticket ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Tickets from GLPI
## NOTES
PSP 05/2019

## RELATED LINKS
