---
title: Get-GlpiToolsPdus
---

## SYNOPSIS
Function is getting Pdu informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsPdus [-All] [<CommonParameters>]
```

### PduId
```
Get-GlpiToolsPdus -PduId <String[]> [-Raw] [-Parameter <String>] [<CommonParameters>]
```

### PduName
```
Get-GlpiToolsPdus -PduName <String> [-SearchInTrash <String>] [<CommonParameters>]
```

## DESCRIPTION
Function is based on PduID which you can find in GLPI website
Returns object with property's of Pdu

## EXAMPLES

### EXAMPLE 1
```
326 | Get-GlpiToolsPdus
```

Function gets PduID from GLPI from Pipline, and return Pdu object

### EXAMPLE 2
```
326, 321 | Get-GlpiToolsPdus
```

Function gets PduID from GLPI from Pipline (u can pass many ID's like that), and return Pdu object

### EXAMPLE 3
```
Get-GlpiToolsPdus -PduId 326
```

Function gets PduID from GLPI which is provided through -PduId after Function type, and return Pdu object

### EXAMPLE 4
```
Get-GlpiToolsPdus -PduId 326, 321
```

Function gets PduID from GLPI which is provided through -PduId keyword after Function type (u can provide many ID's like that), and return Pdu object

### EXAMPLE 5
```
Get-GlpiToolsPdus -PduId 234 -Raw
```

Example will show Pdu with id 234, but without any parameter converted

### EXAMPLE 6
```
234 | Get-GlpiToolsPdus -Raw
```

Example will show Pdu with id 234, but without any parameter converted

### EXAMPLE 7
```
Get-GlpiToolsPdus -PduName glpi
```

Example will return glpi Pdu, but what is the most important, Pdu will be shown exacly as you see in glpi Pdus tab.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

### EXAMPLE 8
```
Get-GlpiToolsPdus -PduName glpi -SearchInTrash Yes
```

Example will return glpi Pdu, but from trash

## PARAMETERS

### -All
This parameter will return all Pdus from GLPI

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

### -PduId
This parameter can take pipline input, either, you can use this function with -PduId keyword.
Provide to this param Pdu ID from GLPI Pdus Bookmark

```yaml
Type: String[]
Parameter Sets: PduId
Aliases: PID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with PduId Parameter.
PduId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: PduId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -PduName
Provide to this param Pdu Name from GLPI Pdus Bookmark

```yaml
Type: String
Parameter Sets: PduName
Aliases: PN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SearchInTrash
Parameter which you can use with PduName Parameter.
If you want Search for Pdu name in trash, that parameter allow you to do it.

```yaml
Type: String
Parameter Sets: PduName
Aliases: SIT

Required: False
Position: Named
Default value: No
Accept pipeline input: False
Accept wildcard characters: False
```

### -Parameter
Parameter which you can use with PduId Parameter. 
If you want to get additional parameter of Pdu object like, disks, or logs, use this parameter.

```yaml
Type: String
Parameter Sets: PduId
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

### Pdu ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Pdus from GLPI
## NOTES
PSP 05/2019

## RELATED LINKS
