---
title: Get-GlpiToolsDropdownsWifiNetworks
---

## SYNOPSIS
Function is getting Wifi Networks informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsWifiNetworks [-All] [<CommonParameters>]
```

### WifiNetworkId
```
Get-GlpiToolsDropdownsWifiNetworks -WifiNetworkId <String[]> [-Raw] [<CommonParameters>]
```

### WifiNetworkName
```
Get-GlpiToolsDropdownsWifiNetworks -WifiNetworkName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on WifiNetworkId which you can find in GLPI website
Returns object with property's of Wifi Networks

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsWifiNetworks -All
```

Example will return all Wifi Networks from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsWifiNetworks
```

Function gets WifiNetworkId from GLPI from pipeline, and return Wifi Networks object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsWifiNetworks
```

Function gets WifiNetworkId from GLPI from pipeline (u can pass many ID's like that), and return Wifi Networks object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsWifiNetworks -WifiNetworkId 326
```

Function gets WifiNetworkId from GLPI which is provided through -WifiNetworkId after Function type, and return Wifi Networks object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsWifiNetworks -WifiNetworkId 326, 321
```

Function gets Wifi Networks Id from GLPI which is provided through -WifiNetworkId keyword after Function type (u can provide many ID's like that), and return Wifi Networks object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsWifiNetworks -WifiNetworkName Fusion
```

Example will return glpi Wifi Networks, but what is the most important, Wifi Networks will be shown exactly as you see in glpi dropdown Wifi Networks.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Wifi Networks from GLPI

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

### -WifiNetworkId
This parameter can take pipeline input, either, you can use this function with -WifiNetworkId keyword.
Provide to this param WifiNetworkId from GLPI Wifi Networks Bookmark

```yaml
Type: String[]
Parameter Sets: WifiNetworkId
Aliases: WNID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with WifiNetworkId Parameter.
WifiNetworkId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: WifiNetworkId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -WifiNetworkName
This parameter can take pipeline input, either, you can use this function with -WifiNetworkId keyword.
Provide to this param Wifi Networks Name from GLPI Wifi Networks Bookmark

```yaml
Type: String
Parameter Sets: WifiNetworkName
Aliases: WNN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Wifi Networks ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Wifi Networks from GLPI
## NOTES
PSP 09/2019

## RELATED LINKS
