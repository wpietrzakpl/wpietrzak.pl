---
title: Get-GlpiToolsPhones
---

## SYNOPSIS
Function is getting Phone informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsPhones [-All] [<CommonParameters>]
```

### PhoneId
```
Get-GlpiToolsPhones -PhoneId <String[]> [-Raw] [-Parameter <String>] [<CommonParameters>]
```

### PhoneName
```
Get-GlpiToolsPhones -PhoneName <String> [-SearchInTrash <String>] [<CommonParameters>]
```

## DESCRIPTION
Function is based on PhoneID which you can find in GLPI website
Returns object with property's of Phone

## EXAMPLES

### EXAMPLE 1
```
326 | Get-GlpiToolsPhones
```

Function gets PhoneID from GLPI from Pipline, and return Phone object

### EXAMPLE 2
```
326, 321 | Get-GlpiToolsPhones
```

Function gets PhoneID from GLPI from Pipline (u can pass many ID's like that), and return Phone object

### EXAMPLE 3
```
Get-GlpiToolsPhones -PhoneId 326
```

Function gets PhoneID from GLPI which is provided through -PhoneId after Function type, and return Phone object

### EXAMPLE 4
```
Get-GlpiToolsPhones -PhoneId 326, 321
```

Function gets PhoneID from GLPI which is provided through -PhoneId keyword after Function type (u can provide many ID's like that), and return Phone object

### EXAMPLE 5
```
Get-GlpiToolsPhones -PhoneId 234 -Raw
```

Example will show Phone with id 234, but without any parameter converted

### EXAMPLE 6
```
234 | Get-GlpiToolsPhones -Raw
```

Example will show Phone with id 234, but without any parameter converted

### EXAMPLE 7
```
Get-GlpiToolsPhones -PhoneName glpi
```

Example will return glpi Phone, but what is the most important, Phone will be shown exacly as you see in glpi Phones tab.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

### EXAMPLE 8
```
Get-GlpiToolsPhones -PhoneName glpi -SearchInTrash Yes
```

Example will return glpi Phone, but from trash

## PARAMETERS

### -All
This parameter will return all Phones from GLPI

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

### -PhoneId
This parameter can take pipline input, either, you can use this function with -PhoneId keyword.
Provide to this param Phone ID from GLPI Phones Bookmark

```yaml
Type: String[]
Parameter Sets: PhoneId
Aliases: PID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with PhoneId Parameter.
PhoneId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: PhoneId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -PhoneName
Provide to this param Phone Name from GLPI Phones Bookmark

```yaml
Type: String
Parameter Sets: PhoneName
Aliases: PN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SearchInTrash
Parameter which you can use with PhoneName Parameter.
If you want Search for Phone name in trash, that parameter allow you to do it.

```yaml
Type: String
Parameter Sets: PhoneName
Aliases: SIT

Required: False
Position: Named
Default value: No
Accept pipeline input: False
Accept wildcard characters: False
```

### -Parameter
Parameter which you can use with PhoneId Parameter. 
If you want to get additional parameter of Phone object like, disks, or logs, use this parameter.

```yaml
Type: String
Parameter Sets: PhoneId
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

### Phone ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Phones from GLPI
## NOTES
PSP 05/2019

## RELATED LINKS
