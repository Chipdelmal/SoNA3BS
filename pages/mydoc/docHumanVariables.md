---
title: Humans
sidebar: mydoc_sidebar
permalink: docHumanVariables.html
folder: mydoc
toc: true
summary: "Humans are extremely flexible in their behaviour to accomodate different epidemiological scenarios. Their movement and activity times help determine the patterns in which a disease can spread so their relevance in the process of can not be neglected."
---

## General Behaviour 

In general terms humans are divided into households. Each person 'belongs' to a household to which it returns each night (generally speaking). Humans are further divided into 'workers' and 'home-stayers'. Worker humans go to their assigned work zone every day for a predetermined amount of time. Humans can be also programmed with a certain probability of visiting other households.

## Variables

### replacementCooldown  
* V:Int
* Timer that avoids a loop in the population replacement strategies

### workZone  
* C:Int
* Determines to which work zone a human must go to CURRENTLY UNUSED

### visitingHouseNumber  
* V:Int
* Determines which house a human will visit

### visitingCooldown  
* V:Int 
* Timer that avoids visiting loops

### visiting?  
* V:Bool 
* Determines if a human is currently visiting another house

### group  

### groupP 

### worker?  
* C:Bool: 
* Differentiates workers from homestayers

### name  
* C:String 
* Person's name

### goWork?  
* V:Bool
* Determines if a person should transit to work or not

### workHoursTimer  
* V:Int
* Timer of the missing work hours for an individual to go home

### dengue  
* V:Bool
* Stores the dengue sick state of an individual CURRENTLY UNUSED

### flu  
* V:Bool
* Stores the flu sick state of an individual CURRENTLY UNUSED

### contacts_list
* V:StringArray
* Stores the direct contacts between the current individual and other ones

### contacts_houses_list
* V:StringArray
* Stores the direct contacts between the current individual and buildings

### contacted?  
* V:Bool
* Temporary flow variable to avoid contacts loop 

### contacted_house?
* V:Bool
* Temporary flow variable to avoid contacts loop

### contacted_workZone? 
* V:Bool
* Temporary flow variable to avoid contacts loop