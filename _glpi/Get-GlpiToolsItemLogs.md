---
title: Get-GlpiToolsItemLogs
---

## SYNOPSIS
Function is getting Logs from Items from GLPI

## SYNTAX

```
Get-GlpiToolsItemLogs -LogsFor <String> -ItemId <Int32[]> [<CommonParameters>]
```

## DESCRIPTION
Function is based on ItemID which you can find on bookmark of item which you want to get logs.
Returns object with Logs for specific id of item.

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsItemLogs -LogsFor Computer -ItemId 2
```

Exaple will show logs for Computer which id is 2.

### EXAMPLE 2
```
2 | Get-GlpiToolsItemLogs -LogsFor Computer
```

Exaple will show logs for Computer which id is 2.
Id is taken from pipeline.

## PARAMETERS

### -LogsFor
Parameter where you have to provide itemtype.
You can choose itemtype from list.

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ItemId
Parameter where you have to provide item id.
You can find id in GLPI.

```yaml
Type: Int32[]
Parameter Sets: (All)
Aliases: CID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### You have to provide itemtype and itemid.
## OUTPUTS

### Function will return pscustomobject.
## NOTES
PSP 05/2019

## RELATED LINKS
