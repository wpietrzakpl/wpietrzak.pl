---
title: Get-GlpiToolsUsers
---

## SYNOPSIS
Function based on GLPI User ID, returns Name and Surname of desired user.

## SYNTAX

### All
```
Get-GlpiToolsUsers [-All] [<CommonParameters>]
```

### UserId
```
Get-GlpiToolsUsers -UserId <String[]> [-Raw] [<CommonParameters>]
```

### UserName
```
Get-GlpiToolsUsers -UserName <String> [-SearchInTrash <String>] [<CommonParameters>]
```

## DESCRIPTION
Function based on GLPI User ID, returns Name and Surname of desired user.

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsUsers -All
```

Example will return all users from Users.

### EXAMPLE 2
```
326 | Get-GlpiToolsUsers
```

Function gets UserID from GLPI from Pipline, and return User object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsUsers
```

Function gets UserID from GLPI from Pipline (u can pass many ID's like that), and return User object

### EXAMPLE 4
```
Get-GlpiToolsUsers -UserId 326
```

Function gets UserID from GLPI which is provided through -UserId after Function type, and return User object

### EXAMPLE 5
```
Get-GlpiToolsUsers -UserId 326, 321
```

Function gets UserID from GLPI which is provided through -UserId keyword after Function type (u can provide many ID's like that), and return User object

### EXAMPLE 6
```
Get-GlpiToolsUsers -UserId 234 -Raw
```

Example will show user with id 234, but without any parameter converted

### EXAMPLE 7
```
234 | Get-GlpiToolsUsers -Raw
```

Example will show user with id 234, but without any parameter converted

### EXAMPLE 8
```
Get-GlpiToolsUsers -UserName glpi
```

Example will return glpi user, but what is the most important, user will be shown exactly as you see in glpi users tab.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

### EXAMPLE 9
```
Get-GlpiToolsUsers -UserName glpi -SearchInTrash Yes
```

Example will return glpi user, but from trash

## PARAMETERS

### -All
This parameter will return all users from GLPI

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

### -UserId
This parameter can take pipline input, either, you can use this function with -UserId keyword.
Provide to this param User ID from GLPI Users Bookmark

```yaml
Type: String[]
Parameter Sets: UserId
Aliases: UID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with UserId Parameter.
UserId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: UserId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -UserName
Provide to this param User Name from GLPI Users Bookmark

```yaml
Type: String
Parameter Sets: UserName
Aliases: UN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SearchInTrash
Parameter which you can use with UserName Parameter.
If you want Search for user name in trash, that parameter allow you to do it.

```yaml
Type: String
Parameter Sets: UserName
Aliases: SIT

Required: False
Position: Named
Default value: No
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### User ID which you can find in GLPI, or use this Function to convert ID returned from other Functions.
## OUTPUTS

### Function returns PSCustomObject with users data from GLPI.
## NOTES
PSP 12/2018

## RELATED LINKS
