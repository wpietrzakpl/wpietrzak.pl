---
title: Update-GlpiToolsItems
---

## SYNOPSIS
Function Update an object (or multiple objects) existing in GLPI.

## SYNTAX

### ID
```
Update-GlpiToolsItems -UpdateTo <String> -ItemId <Int32> -ItemsHashtableWithoutId <Hashtable>
 [<CommonParameters>]
```

### JsonPayload
```
Update-GlpiToolsItems -UpdateTo <String> -JsonPayload <Array> [<CommonParameters>]
```

## DESCRIPTION
Function Update an object (or multiple objects) into GLPI.
You can choose between every items in Asset Tab.\

## EXAMPLES

### EXAMPLE 1
```
$example = "@
{
"input" : [
{
"id" : "15",
"comment" : "updated from script 4"
},
{
"id" : "17",
"comment" : "updated from script 2"
}
]
}
@"
PS C:\> Update-GlpiToolsItems -UpdateTo Computer -JsonPayload $example
```
Example will Update item which id is 15 and 17 into Computers

### EXAMPLE 2
```
$example =  @{name = "test"}
PS C:\> Update-GlpiToolsItems -UpdateTo Computer -ItemId 5 -ItemsHashtableWithoutId $example
```
Example will Update item which id is 5 into Computers

## PARAMETERS

### -UpdateTo
Parameter specify where you want to update object.
You can add your custom parameter options to Parameters.json file located in Private folder

```yaml
Type: String
Parameter Sets: (All)
Aliases: UT

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ItemId
Parameter specify item id.
You can find id in GLPI or, when you run Get-GlpiToolsComputer function.

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

### -ItemsHashtableWithoutId
Parameter specify a hashtable without id of item to be updated, and others fields.
You provide id in -ItemId parameter.
You can get values to use, when you run Get-GlpiToolsComputer function.

```yaml
Type: Hashtable
Parameter Sets: ID
Aliases: IHWID

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -JsonPayload
Parameter specify a JsonPayload with id of item to be updated, and others fields.
You can get values to use, when you run Get-GlpiToolsComputer function.

```yaml
Type: Array
Parameter Sets: JsonPayload
Aliases: JsPa

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### JsonPayload, or hashtable.
## OUTPUTS

### Information with id and message, which items were Updated.
## NOTES
PSP 04/2019

## RELATED LINKS
