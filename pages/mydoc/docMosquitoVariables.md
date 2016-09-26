---
title: Documentation
sidebar: mydoc_sidebar
permalink: docMosquitoVariables.html
folder: mydoc
toc: false
summary: "Mosquito Variables Descriptions"
---

### age
* V:Int 
* Stores the mosquito age in ticks

### mated?
* V:Bool
* Stores the female state in mating 

### female? 

* C:Bool
* Differentiates male mosquitos from females

### bloodfed?
* V:Bool
* Stores the female state in bloodfed as part of reproductive cycle

### laidEggs?
* V:Bool
* Stores the female state in oviposition

### sterile? 
* C:Bool
* Differentiates sterile mosquitos (males) from non-sterile mosquitos

### sterileMate? 
* V:Bool
* Stores if a female mated with a sterile male

### wolbachia?
* C:Bool
* Differentiates wolbachia-infected mosquitos from non-infected 

### wolbachiaMate?
* V:Bool
* Stores if a female mated with a wolbachia-infected mate

### oxitech?
* C:Bool
* Differentiates oxitec males from regular males

### oxitechMate?
* V:Bool
* Stores if a female mated with an oxitec male

### fitness_selected?
* Differentiates a fitness selected mosquito from a regular one

### fitness_selectedMate?
* Stores if the female has mated with a fitness selected male

### movement_speeds 
* C:IntArray
* Stores the movement speeds of the mosquitos in each life stage

### bitten_list
* V:StringArray
* Stores the individuals and times in which a mosquito has bitten persons

### feeding_cooldown 
* V:Int
* Stores the number of ticks missing so that a female can lay eggs

### dengue 
* V:Int
* Stores the dengue infection of a mosquito CURRENTLY UNUSED

### ovipositionCounter
* V:Int
* Counts the number of times a female has laid eggs

### maleReproductiveDelay 
* V:Int
* Timer from egg hatching until the time when males are ready to mate

### gonotrophic_cooldown 
* V:Int
* Timer from bloodfeed until oviposition ready

### metabolic_rate 
* V:Int
* Stores the metabolic development of the mosquito (when equal to one it resets)

### life_stage 
* V:Int
* Stores the current life phase of the mosquito for behaviour purposes

### life_stage_ticks
* V:Int
* Stores the number of ticks a mosquito has spent in a given life stage 

### life_stage_ticks_list 
* V:IntArray
* Stores the number of ticks a mosquito has spent in each life stage

### hunger 
* V:Int
* Stores the hunger level of the mosquito

### transition_ages

### ridl_gene 
* C:Int
* Stores the type of RIDL genotype a mosquito posseses (0: rr :: 1:Rr :: 2:RR)

### mate_ridl_gene 
* C:Int
* Stores the type of RIDL genotype a mosquito posseses (0: rr :: 1:Rr :: 2:RR)
