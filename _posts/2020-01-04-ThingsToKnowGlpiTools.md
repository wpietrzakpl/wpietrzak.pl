---
title: 3 Things to know - GlpiTools
categories:
    - Glpi
tags:
    - GlpiTools
---

# Begin 
If you reading this article, I assume that you already did steps from:
[How to start with GlpiTools Module](https://www.wpietrzak.pl/glpi/StartGlpiTools/)

There is a few things that you have to know about the module, and in my opinion is important to know them

Ok, Let's go 😀

# Process

## Configuration store
Configuration is just a .json file  
I secure (just to hide real values, because converting is easy to revert) configuration parameters by converting them to secure strings  

Depend on OS where do you use module, Configuration is stored in different places  
On Linux
```powershell
"$env:HOME/.config/GlpiToolsConfig\Configuration.json"
```
On Windows
```powershell
"$env:LOCALAPPDATA\GlpiToolsConfig\Configuration.json" 
```
## Parameters.json
This file is using for autocomplete parameters from functions like:  
```powershell
Get-GlpiToolsItems
Get-GlpiToolsListSearchOptions
Search-GlpiToolsItems
Add-GlpiToolsItems
Update-GlpiToolsItems
Remove-GlpiToolsItems
```
Parameters.json is located inside the module, inside Private folder  
On my computer this is:  
```powershell
"c:\Program Files\WindowsPowerShell\Modules\GlpiTools\Private\"
```
But, you have to check in your system where module is installed  
Check inside folders shown by command  
```powershell
$env:PSModulePath
```
The most important thing is that, you can add to the file your own endpoints/components!!  
Do you installed new plugin and want to use it with module? You don't have to wait for new functions or write it on your own  
All what you doing is  
- locate module on the disk
- add new component to parameters.json  

like: 
```json
"GlpiComponents": [
        "Computer",
        "Monitor",
        "Software",
        "NetworkEquipment",
        "Peripheral",
        "Printer",
        "provide it here"
    ]
```
The best way to find name of the endpoint/component is to look on database structure and names of the tables  

Then you have to remember, to make a copy of this file if you updating/installing on your system or installing module on another system or server etc...

## Search-GlpiToolsItems 
Function Search-GlpiToolsItems, can a little bit confuse you if you don't know **two** things  
### One
This function will show that many properties, as see user which is use in API  

But, the best way is to show it on example  
We have a Computers Tab, you are logged in as user used in API  
You see only three properites: ID, Name, and Serial number of all computers there

You use  
```powershell
Get-GlpiToolsComputers -All 
```
And you get all computers with all properties inside  

Then, you use  
```powershell
Search-GlpiToolsItems -SearchFor Computer -SearchType contains -SearchValue <name of computer>
```
And get only 3 properties, why?  
Because, to get that you have to modify the view in GUI  

There is icon like "key" or "keytool" where you can define which properties do you see

Add there that many parameters, as you want to see when you will use Search function

### Two
Function has one special parameter called "-SearchField"  

This is a parameter where you provide an ID or parameter from output of another function  
```powershell
Get-GlpiToolsListSearchOptions
```
By default Search function use parameter "name", but if you want to search computer by property "serial number" you have to know which ID "serial number" has  

This parameter is not mandatory, but is good to know how it works and how you can customize command to Search not only for names 

# End
And that's it 😀  
If you have more questions, feel free to find me and PM on FB or Twitter