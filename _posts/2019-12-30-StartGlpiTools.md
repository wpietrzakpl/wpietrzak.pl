---
title: How to start with GlpiTools Module
categories:
    - Glpi
tags:
    - GlpiTools
    - Glpi
---
# How To Start
To start with module GlpiTools which wrap Glpi API into PowerShell functions you have to complete few steps below. 
- Install Module from PS Gallery 
- Import Module to use functions
- Configure GLPI to use API
- Set API configuration 

Run PowerShell console with elevated permissions - its important! 
## Install Module from PS Gallery 
```powershell
Install-Module -Name GlpiTools 
```

## Import Module to use functions
After Module Instalation from PS Gallery you have to import module to use
```powershell
Import-Module -Name GlpiTools 
```

## Configure GLPI to use API
 * Enable API - Setup -> General -> API -] Enable Rest API
 * Configure Access From Localhost - Setup -> General -> API -> full access from localhost -] Filter access (I prefere to leave parameters, IPv4, IPv6 blank - not so secure but if you testing its enough, remember to change it)
 * Path to Glpi API - Setup -> General -> API -] URL of the API 
 * Get app_token - Setup -> General -> API -> full access from localhost -] Filter access (parameter Application token(app_token), click regenerate checkbox and save, after that app_token will show. Copy token and save it for later use)
 * Get User API token - Administration -> Users - (user) -> Settings -] Remote access keys (parameter API token, click regenerate checkbox and save, after that User Token will show. Copy token and save it for later use) - ! Remember that user must have permissions to do what u want to do with API

## Set API configuration
Last step, and you are ready to go! 
```powershell 
$param = {
    AppToken = "provide here app_token"
    UserToken = "provide here user_token"
    PathToGlpi = "provide here URL of the API"
}
Set-GlpiToolsConfig @param
```
# End 😀
You can check existing configuration by running
```powershell
Get-GlpiToolsConfig
```
There is always one configuration, so if you want to change, you have to run commands from "Set API configuration" step 

Enjoy! 