---
title: Get-GlpiToolsDropdownsContractTypes
---

## SYNOPSIS
Function is getting Contract Types informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsContractTypes [-All] [<CommonParameters>]
```

### ContractTypeId
```
Get-GlpiToolsDropdownsContractTypes -ContractTypeId <String[]> [-Raw] [<CommonParameters>]
```

### ContractTypeName
```
Get-GlpiToolsDropdownsContractTypes -ContractTypeName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on ContractTypeId which you can find in GLPI website
Returns object with property's of Contract Types

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsContractTypes -All
```

Example will return all Contract Types from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsContractTypes
```

Function gets ContractTypeId from GLPI from Pipline, and return Contract Types object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsContractTypes
```

Function gets ContractTypeId from GLPI from Pipline (u can pass many ID's like that), and return Contract Types object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsContractTypes -ContractTypeId 326
```

Function gets ContractTypeId from GLPI which is provided through -ContractTypeId after Function type, and return Contract Types object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsContractTypes -ContractTypeId 326, 321
```

Function gets Contract Types Id from GLPI which is provided through -ContractTypeId keyword after Function type (u can provide many ID's like that), and return Contract Types object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsContractTypes -ContractTypeName Fusion
```

Example will return glpi Contract Types, but what is the most important, Contract Types will be shown exactly as you see in glpi dropdown Contract Types.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Contract Types from GLPI

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

### -ContractTypeId
This parameter can take pipline input, either, you can use this function with -ContractTypeId keyword.
Provide to this param ContractTypeId from GLPI Contract Types Bookmark

```yaml
Type: String[]
Parameter Sets: ContractTypeId
Aliases: CTID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with ContractTypeId Parameter.
ContractTypeId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: ContractTypeId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -ContractTypeName
This parameter can take pipline input, either, you can use this function with -ContractTypeId keyword.
Provide to this param Contract Types Name from GLPI Contract Types Bookmark

```yaml
Type: String
Parameter Sets: ContractTypeName
Aliases: CTN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Contract Types ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Contract Types from GLPI
## NOTES
PSP 09/2019

## RELATED LINKS
