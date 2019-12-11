---
title: Get-GlpiToolsDropdownsStatesOfTheVirtualMachine
---

## SYNOPSIS
Function is getting States of the virtual machine informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsStatesOfTheVirtualMachine [-All] [<CommonParameters>]
```

### StateOfTheVirtualMachineId
```
Get-GlpiToolsDropdownsStatesOfTheVirtualMachine -StateOfTheVirtualMachineId <String[]> [-Raw]
 [<CommonParameters>]
```

### StateOfTheVirtualMachineName
```
Get-GlpiToolsDropdownsStatesOfTheVirtualMachine -StateOfTheVirtualMachineName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on StateOfTheVirtualMachineId which you can find in GLPI website
Returns object with property's of States of the virtual machine

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsStatesOfTheVirtualMachine -All
```

Example will return all States of the virtual machine from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsStatesOfTheVirtualMachine
```

Function gets StateOfTheVirtualMachineId from GLPI from pipeline, and return States of the virtual machine object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsStatesOfTheVirtualMachine
```

Function gets StateOfTheVirtualMachineId from GLPI from pipeline (u can pass many ID's like that), and return States of the virtual machine object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsStatesOfTheVirtualMachine -StateOfTheVirtualMachineId 326
```

Function gets StateOfTheVirtualMachineId from GLPI which is provided through -StateOfTheVirtualMachineId after Function type, and return States of the virtual machine object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsStatesOfTheVirtualMachine -StateOfTheVirtualMachineId 326, 321
```

Function gets States of the virtual machine Id from GLPI which is provided through -StateOfTheVirtualMachineId keyword after Function type (u can provide many ID's like that), and return States of the virtual machine object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsStatesOfTheVirtualMachine -StateOfTheVirtualMachineName Fusion
```

Example will return glpi States of the virtual machine, but what is the most important, States of the virtual machine will be shown exactly as you see in glpi dropdown States of the virtual machine.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all States of the virtual machine from GLPI

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

### -StateOfTheVirtualMachineId
This parameter can take pipeline input, either, you can use this function with -StateOfTheVirtualMachineId keyword.
Provide to this param StateOfTheVirtualMachineId from GLPI States of the virtual machine Bookmark

```yaml
Type: String[]
Parameter Sets: StateOfTheVirtualMachineId
Aliases: SOTVMID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with StateOfTheVirtualMachineId Parameter.
StateOfTheVirtualMachineId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: StateOfTheVirtualMachineId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -StateOfTheVirtualMachineName
This parameter can take pipeline input, either, you can use this function with -StateOfTheVirtualMachineId keyword.
Provide to this param States of the virtual machine Name from GLPI States of the virtual machine Bookmark

```yaml
Type: String
Parameter Sets: StateOfTheVirtualMachineName
Aliases: SOTVMN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### States of the virtual machine ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of States of the virtual machine from GLPI
## NOTES
PSP 09/2019

## RELATED LINKS
