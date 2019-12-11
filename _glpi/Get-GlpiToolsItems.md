---
title: Get-GlpiToolsItems
---

## SYNOPSIS
Function is getting all the items of a specific type in GLPI (also feature SearchText).

## SYNTAX

```
Get-GlpiToolsItems [-ItemType] <String> [[-SearchText] <Hashtable>] [[-Raw] <Boolean>]
 [[-SearchInTrash] <Boolean>] [[-OnlyId] <Boolean>] [[-ExtraParameter] <String>] [<CommonParameters>]
```

## DESCRIPTION
Function is getting all the items of a specific type in GLPI.
Can be filter with SearchText paramter
Like https://github.com/glpi-project/glpi/blob/master/apirest.md#get-all-items

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsItems -ItemType "Group_Ticket"
```

Function gets all items from Group_Ticket

### EXAMPLE 2
```
@{"groups_id"="^10$" ; "type"="^2$"} | Get-GlpiToolsItems -ItemType "Group_Ticket"
```

Function gets SearchCriteria from Pipeline, and return GLPI object

### EXAMPLE 3
```
@{"groups_id"="^10$" ; "type"="^2$"}  , @{"groups_id"="^15$" ; "type"="^2$"}  | Get-GlpiToolsItems -ItemType "Group_Ticket"
```

Function gets multiple SearchCriteria from Pipeline, and return GLPI object

### EXAMPLE 4
```
Get-GlpiToolsItems -ItemType "Group_Ticket" -SearchText @{"groups_id"="^10$" ; "type"="^2$"}
```

Function gets GLPI object filter by SearchText.

### EXAMPLE 5
```
Get-GlpiToolsItems -ItemType "Ticket" -SearchText @{"id"="^234$"}  -Raw
```

Example will show Ticket with id 234, but without any parameter converted

### EXAMPLE 6
```
@{"id"="^234$"} | Get-GlpiToolsItems -ItemType "Ticket" -Raw
```

Example will show Ticket with id 234, but without any parameter converted

### EXAMPLE 7
```
Get-GlpiToolsItems -ItemType "Ticket" -SearchInTrash $true
```

Example will return glpi Ticket, but from trash

## PARAMETERS

### -ItemType
Type of item wanted.
Exemples : Computer, Monitor, User, Group_Ticket, Group_User, etc.

```yaml
Type: String
Parameter Sets: (All)
Aliases: Type

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SearchText
SearchText (default NULL): hashtable of filters to pass on the query (with key = field and value = the text to search).
By default it act as a '-like "*value*"'.
Use ^ and $ to force an exact match.
Eg.
SearchText = @{"groups_id"="^10$" ; "type"="^2$"}
This parameter can take pipeline input.

```yaml
Type: Hashtable
Parameter Sets: (All)
Aliases: Search

Required: False
Position: 2
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Raw is always ON if the return contain more that one object.
If the return contain only one object and RAW is not use, parameters will be converted (expanded to show name instead of ID).
Use the parameter RAW to force to show ID in ALL cases.

```yaml
Type: Boolean
Parameter Sets: (All)
Aliases:

Required: False
Position: 3
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -SearchInTrash
(default: false): Return deleted element.
Optional

```yaml
Type: Boolean
Parameter Sets: (All)
Aliases: SIT

Required: False
Position: 4
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -OnlyId
(default: false): keep only id keys in returned data.
Optional.

```yaml
Type: Boolean
Parameter Sets: (All)
Aliases:

Required: False
Position: 5
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -ExtraParameter
String append to the query for extra option.
Refer to apirest.php.
Ex.
"&only_id=true" or "&with_infocoms", etc..

```yaml
Type: String
Parameter Sets: (All)
Aliases: Param

Required: False
Position: 6
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### SearchText hashtable.
## OUTPUTS

### Function returns PSCustomObject with property's of Object from GLPI
## NOTES
SilentBob999 10/2019

## RELATED LINKS
