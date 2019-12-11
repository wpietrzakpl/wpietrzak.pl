---
title: Get-GlpiToolsContacts
---

## SYNOPSIS
Function is getting Contact informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsContacts [-All] [<CommonParameters>]
```

### ContactId
```
Get-GlpiToolsContacts -ContactId <String[]> [-Raw] [<CommonParameters>]
```

### ContactName
```
Get-GlpiToolsContacts -ContactName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on ContactId which you can find in GLPI website
Returns object with property's of Contact

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsContacts -All
```

Example will return all Contact from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsContacts
```

Function gets ContactId from GLPI from Pipline, and return Contact object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsContacts
```

Function gets ContactId from GLPI from Pipline (u can pass many ID's like that), and return Contact object

### EXAMPLE 4
```
Get-GlpiToolsContacts -ContactId 326
```

Function gets ContactId from GLPI which is provided through -ContactId after Function type, and return Contact object

### EXAMPLE 5
```
Get-GlpiToolsContacts -ContactId 326, 321
```

Function gets Contact Id from GLPI which is provided through -ContactId keyword after Function type (u can provide many ID's like that), and return Contact object

### EXAMPLE 6
```
Get-GlpiToolsContacts -ContactName Fusion
```

Example will return glpi Contact, but what is the most important, Contact will be shown exactly as you see in glpi dropdown Contact.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Contact from GLPI

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

### -ContactId
This parameter can take pipline input, either, you can use this function with -ContactId keyword.
Provide to this param ContactId from GLPI Contact Bookmark

```yaml
Type: String[]
Parameter Sets: ContactId
Aliases: CID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with ContactId Parameter.
ContactId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: ContactId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -ContactName
This parameter can take pipline input, either, you can use this function with -ContactId keyword.
Provide to this param Contact Name from GLPI Contact Bookmark

```yaml
Type: String
Parameter Sets: ContactName
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

### Contact ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Contact from GLPI
## NOTES
PSP 11/2019

## RELATED LINKS
