---
title: Get-GlpiToolsContracts
---

## SYNOPSIS
Function is getting Contract informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsContracts [-All] [<CommonParameters>]
```

### ContractId
```
Get-GlpiToolsContracts -ContractId <String[]> [-Raw] [<CommonParameters>]
```

### ContractName
```
Get-GlpiToolsContracts -ContractName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on ContractId which you can find in GLPI website
Returns object with property's of Contract

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsContracts -All
```

Example will return all Contract from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsContracts
```

Function gets ContractId from GLPI from Pipline, and return Contract object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsContracts
```

Function gets ContractId from GLPI from Pipline (u can pass many ID's like that), and return Contract object

### EXAMPLE 4
```
Get-GlpiToolsContracts -ContractId 326
```

Function gets ContractId from GLPI which is provided through -ContractId after Function type, and return Contract object

### EXAMPLE 5
```
Get-GlpiToolsContracts -ContractId 326, 321
```

Function gets Contract Id from GLPI which is provided through -ContractId keyword after Function type (u can provide many ID's like that), and return Contract object

### EXAMPLE 6
```
Get-GlpiToolsContracts -ContractName Fusion
```

Example will return glpi Contract, but what is the most important, Contract will be shown exactly as you see in glpi dropdown Contract.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Contract from GLPI

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

### -ContractId
This parameter can take pipline input, either, you can use this function with -ContractId keyword.
Provide to this param ContractId from GLPI Contract Bookmark

```yaml
Type: String[]
Parameter Sets: ContractId
Aliases: CID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with ContractId Parameter.
ContractId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: ContractId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -ContractName
This parameter can take pipline input, either, you can use this function with -ContractId keyword.
Provide to this param Contract Name from GLPI Contract Bookmark

```yaml
Type: String
Parameter Sets: ContractName
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

### Contract ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Contract from GLPI
## NOTES
PSP 11/2019

## RELATED LINKS
