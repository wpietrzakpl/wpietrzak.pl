---
title: Add-GlpiToolsItems
---

## SYNOPSIS
Function Add an object (or multiple objects) into GLPI.

## SYNTAX

### HashtableToAdd
```
Add-GlpiToolsItems -AddTo <String> -HashtableToAdd <Hashtable> [<CommonParameters>]
```

### JsonPayload
```
Add-GlpiToolsItems -AddTo <String> [-JsonPayload <Array>] [<CommonParameters>]
```

## DESCRIPTION
Function Add an object (or multiple objects) into GLPI.
You can choose between every items in Asset Tab.

## EXAMPLES

### EXAMPLE 1
```
Add-GlpiToolsItems -AddTo Computer -HashtableToAdd @{name = "test"} | ConvertTo-Json
```

Example will add item into Computers

### EXAMPLE 2
```
$example =  @{name = "test"} | ConvertTo-Json
PS C:\> Add-GlpiToolsItems -AddTo Computer -HashtableToAdd $example
```
Example will add item into Computers

### EXAMPLE 3
```
$example = @{ name = "test" } | ConvertTo-Json
PS C:\> $upload = '{ "input" : ' + $example + '}'
PS C:\> Add-GlpiToolsItems -AddTo Computer -JsonPayload $upload
```

### EXAMPLE 4
```
$example = "@
{
"input" : [
{
"name" : "test1",
"comment" : "updated from script"
},
{
"name" : "test2",
"comment" : "updated from script"
}
]
}
@"
PS C:\> Add-GlpiToolsItems -AddTo Computer -JsonPayload $example
```
Example will Add items into Computers

## PARAMETERS

### -AddTo
Parameter specify where you want to add new object.
You can add your custom parameter options to Parameters.json file located in Private folder

```yaml
Type: String
Parameter Sets: (All)
Aliases: AT

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -HashtableToAdd
Parameter specify a hashtable with fields of itemtype to be inserted.

```yaml
Type: Hashtable
Parameter Sets: HashtableToAdd
Aliases: HashToAdd

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Hashtable with "input" parameter, or JsonPayload    .
## OUTPUTS

### Information with id and message, which items were added.
## NOTES
PSP 04/2019

## RELATED LINKS
