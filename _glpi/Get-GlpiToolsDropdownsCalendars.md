---
title: Get-GlpiToolsDropdownsCalendars
---

## SYNOPSIS
Function is getting Calendars informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsCalendars [-All] [<CommonParameters>]
```

### CalendarId
```
Get-GlpiToolsDropdownsCalendars -CalendarId <String[]> [-Raw] [<CommonParameters>]
```

### CalendarName
```
Get-GlpiToolsDropdownsCalendars -CalendarName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on CalendarId which you can find in GLPI website
Returns object with property's of Calendars

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsCalendars -All
```

Example will return all Calendars from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsCalendars
```

Function gets CalendarId from GLPI from pipeline, and return Calendars object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsCalendars
```

Function gets CalendarId from GLPI from pipeline (u can pass many ID's like that), and return Calendars object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsCalendars -CalendarId 326
```

Function gets CalendarId from GLPI which is provided through -CalendarId after Function type, and return Calendars object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsCalendars -CalendarId 326, 321
```

Function gets Calendars Id from GLPI which is provided through -CalendarId keyword after Function type (u can provide many ID's like that), and return Calendars object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsCalendars -CalendarName Fusion
```

Example will return glpi Calendars, but what is the most important, Calendars will be shown exactly as you see in glpi dropdown Calendars.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Calendars from GLPI

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

### -CalendarId
This parameter can take pipeline input, either, you can use this function with -CalendarId keyword.
Provide to this param CalendarId from GLPI Calendars Bookmark

```yaml
Type: String[]
Parameter Sets: CalendarId
Aliases: CID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with CalendarId Parameter.
CalendarId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: CalendarId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -CalendarName
This parameter can take pipeline input, either, you can use this function with -CalendarId keyword.
Provide to this param Calendars Name from GLPI Calendars Bookmark

```yaml
Type: String
Parameter Sets: CalendarName
Aliases: CN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Calendars ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Calendars from GLPI
## NOTES
PSP 09/2019

## RELATED LINKS
