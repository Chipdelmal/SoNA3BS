---
title: Documentation
sidebar: mydoc_sidebar
permalink: docMosquitoVariables.html
folder: mydoc
toc: true
summary: "Mosquitoes are the most complex class in our simulation. It is not difficult to envision why as they are the ones that transmit the diseases and because of that we payed special interest in the way their behaviours were modelled so that we could accomodate a wide array of biological and epidemiological scenarios."
---

## General Behaviour
The following pseudo-code shows the general way adult mosquito individuals behave in the simulation.

{% highlight r %}
if(is hungry?):
    look for food and feed
else:
    if(is not female?):
        if(reproductively ready?):
            move towards mating zone
        else:
            rest
    else:
        if(has not mated?):
            look for mate and copulate
        else:
            if(has not bloodfed?):
                look for human and bloodfeed
            else:
                if(has not finished gonotrophic cycle?):
                    rest
                else:
                    look for breeding zone and lay eggs
update metabolic development
{% endhighlight %}


## Variables

A brief description of the variables each mosquito individual contains follows. 
The first line on each description contains if the value should be treated as a variable or constant (V or C respectively) and the type of the variable.

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
