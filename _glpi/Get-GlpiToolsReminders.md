---
title: Get-GlpiToolsReminders
---

## SYNOPSIS
Function is getting Reminders informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsReminders [-All] [<CommonParameters>]
```

### ReminderId
```
Get-GlpiToolsReminders -ReminderId <String[]> [-Raw] [<CommonParameters>]
```

### ReminderName
```
Get-GlpiToolsReminders -ReminderName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on ReminderId which you can find in GLPI website
Returns object with property's of Reminders

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsReminders -All
```

Example will return all Reminders from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsReminders
```

Function gets ReminderId from GLPI from Pipline, and return Reminders object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsReminders
```

Function gets ReminderId from GLPI from Pipline (u can pass many ID's like that), and return Reminders object

### EXAMPLE 4
```
Get-GlpiToolsReminders -ReminderId 326
```

Function gets ReminderId from GLPI which is provided through -ReminderId after Function type, and return Reminders object

### EXAMPLE 5
```
Get-GlpiToolsReminders -ReminderId 326, 321
```

Function gets Reminders Id from GLPI which is provided through -ReminderId keyword after Function type (u can provide many ID's like that), and return Reminders object

### EXAMPLE 6
```
Get-GlpiToolsReminders -ReminderName Fusion
```

Example will return glpi Reminders, but what is the most important, Reminders will be shown exactly as you see in glpi dropdown Reminders.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Reminders from GLPI

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

### -ReminderId
This parameter can take pipline input, either, you can use this function with -ReminderId keyword.
Provide to this param ReminderId from GLPI Reminders Bookmark

```yaml
Type: String[]
Parameter Sets: ReminderId
Aliases: RID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with ReminderId Parameter.
ReminderId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: ReminderId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -ReminderName
This parameter can take pipline input, either, you can use this function with -ReminderId keyword.
Provide to this param Reminders Name from GLPI Reminders Bookmark

```yaml
Type: String
Parameter Sets: ReminderName
Aliases: RN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Reminders ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Reminders from GLPI
## NOTES
PSP 11/2019

## RELATED LINKS
