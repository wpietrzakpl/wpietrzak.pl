---
title: Search-GlpiToolsItems
---

## SYNOPSIS
Function is using GLPI Search Engine to get informations.

## SYNTAX

```
Search-GlpiToolsItems [-SearchFor] <String> [-SearchType] <String[]> [[-SearchField] <String[]>]
 [-SearchValue] <String[]> [[-SearchLink] <String[]>] [[-SearchInTrash] <String>] [<CommonParameters>]
```

## DESCRIPTION
Function Search for specific component in GLPI
Parameters are the names of options in GLPI
Remember that, names used in cmdlet coming from glpi URL, and can be hard to understand, but most of them are intuitional.
To get name you always have to look at the URL in GLPI, for example "http://glpi/front/computer.php" where "computer" is the name to use in parameter.

## EXAMPLES

### EXAMPLE 1
```
Search-GlpiToolsItems -SearchFor Computer -SearchType contains -SearchValue DC
```

Example will show every asset which contains value "DC" in the Name from Asset-\>Computers.

### EXAMPLE 2
```
Search-GlpiToolsItems -SearchFor Computer -SearchType contains -SearchValue DC -SearchField 1
```

Example will show every asset which contains value "DC" in the Name from Asset-\>Computers.
SearchFiled can be retrieved from Get-GlpiToolsListSearchOptions cmdlet, you can provide it throught pipeline.

### EXAMPLE 3
```
Search-GlpiToolsItems -SearchFor Computer -SearchType contains -SearchValue DC -SearchField 1 -SearchInTrash
```

Example will show every asset which contains value "DC" in the Name from Asset-\>Computers.
SearchFiled can be retrieved from Get-GlpiToolsListSearchOptions cmdlet, you can provide it throught pipeline.
SearchInTrash will allow you to search for assets from trash.

## PARAMETERS

### -SearchFor
You can use this function with -SearchFor parameter.
Using TAB button you can choose desired option.
You can add your custom parameter options to Parameters.json file located in Private folder

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SearchType
You can use this function with -SearchType parameter.
Using TAB button you can choose desired option.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases:

Required: True
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SearchField
You can use this function with -SearchField parameter.
This is an optional parameter, default value is 1 which is called Name in GLPI.
This parameter can take pipeline input, even from Get-GlpiToolsListSearchOptions cmdlet.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases:

Required: False
Position: 3
Default value: 1
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -SearchValue
You can use this function with -SearchValue parameter.
This parameter can take pipeline input.
Provide value to the function, which is used to search for.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases:

Required: True
Position: 4
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -SearchLink
{{ Fill SearchLink Description }}

```yaml
Type: String[]
Parameter Sets: (All)
Aliases:

Required: False
Position: 5
Default value: AND
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -SearchInTrash
{{ Fill SearchInTrash Description }}

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: False
Position: 6
Default value: No
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Only for -SearchValue, and -SearchField.
## OUTPUTS

### Function returns PSCustomObject with property's of Search results from GLPI
## NOTES
PSP 02/2019

## RELATED LINKS