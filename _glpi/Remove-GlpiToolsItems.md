---
title: Remove-GlpiToolsItems
---

## SYNOPSIS
Function Remove an object existing in GLPI.

## SYNTAX

### ID
```
Remove-GlpiToolsItems -RemoveFrom <String> -ItemId <Int32> [-Purge] [<CommonParameters>]
```

### HashtableToRemove
```
Remove-GlpiToolsItems -RemoveFrom <String> -HashtableToRemove <Hashtable> [-Purge] [<CommonParameters>]
```

### JsonPayload
```
Remove-GlpiToolsItems -RemoveFrom <String> [-JsonPayload <Array>] [-Purge] [<CommonParameters>]
```

## DESCRIPTION
Remove an object existing in GLPI.
You can choose between every items in Asset Tab.

## EXAMPLES

### EXAMPLE 1
```
Remove-GlpiToolsItems -RemoveFrom Computer -ItemId 1
```

Command will Remove item with id 1, and put item into trashbin.

### EXAMPLE 2
```
Remove-GlpiToolsItems -RemoveFrom Computer -ItemId 1 -Purge
```

Command will Remove item with id 1.
Command will Remove item from trashbin too.

### EXAMPLE 3
```
$example =  @{id = "1"}
PS C:\> Remove-GlpiToolsItems -RemoveFrom Computer -HashtableToRemove $example
```
Example will Remove item from Computers.

### EXAMPLE 4
```
$example = "@
{
"input" : [
{
"id" : "1"
},
{
"id" : "2"
}
]
}
@"
PS C:\> Remove-GlpiToolsItems -RemoveFrom Computer -JsonPayload $example
```
Example will Add items into Computers

## PARAMETERS

### -RemoveFrom
Parameter specify where you want to Remove object. 
You can add your custom parameter options to Parameters.json file located in Private folder

```yaml
Type: String
Parameter Sets: (All)
Aliases: DF

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ItemId
Paremter which indicate on item id to Remove.

```yaml
Type: Int32
Parameter Sets: ID
Aliases: IId

Required: True
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -HashtableToRemove
{{ Fill HashtableToRemove Description }}

```yaml
Type: Hashtable
Parameter Sets: HashtableToRemove
Aliases: HashToDel

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -JsonPayload
Parameter specify a hashtable with "input" parameter to be a JsonPayload.

```yaml
Type: Array
Parameter Sets: JsonPayload
Aliases: JsPa

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Purge
Switch parameter boolean, if the itemtype have a trashbin, you can force purge (Remove finally).
Optional.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Id of item, hashtable, JsonPayload.
## OUTPUTS

### Information with id and message, which items were added.
## NOTES
PSP 04/2019

## RELATED LINKS
