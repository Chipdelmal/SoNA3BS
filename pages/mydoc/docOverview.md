---
title: Documentation
sidebar: mydoc_sidebar
permalink: docOverview.html
folder: mydoc
toc: true
summary: "This page contains a brief description of the way the model is divided and coded. More in-depth information of the specifics of the sub-parts can be found on the other sections of this documentation."
---

## Files Structure
The simulation's folder contains al the files required for the model to run. These files are divided to accomodate different modular aspects of the simulation. A brief description of each one of these files follows.

### go
Main simulation file. This file contains the top-layer routines to be called by the simulation in order to run.
Start here if any specific behaviour is to be changed/analysed.

### global
Global simulation parameters. This file contains all the biological/behavioural parameters that are required to control the agents' behaviours. In an ideal scenario these parameters are exported from "ParameterExport.nb" as this notebook contains all the function fits and scaling factors required for the simulation to run properly.

### auxiliaryFunctions.nls
Functions that perform general unspecific activities like random sampling, day-night cycles, contact updates, etcetera; that are not related to a particular agent type.

### randomScenarios.nls
Five different artificially uniformly distributed generated spatial scenarios. These settings can be created with routines included in "RandomMapGeneration.nb". 

### GoogleMap_HET.nls
Google Map processed spatial layout in "Catemaco, Veracruz". This map was obtained using the routine included in "MapFromGoogle.nb" for houses detection. The algorithm detects squares in a given map image and assigns them spatial coordinates along with a number of persons that live in the "house" according to its detected surface area.

### GoogleMap_HOM.nls
Artificially homogeneous spatial layout with same demographic characteristics as GoogleMap_HET but with all spatial variables removed. All houses and persons are concentrated at the center of the map and breeding/mating sites all are located in their vicinity.

### movement
Pseudo-Random walking routines for agents. All the agents have two basic movement behaviours: targetted movement (movement with a definite direction) and random movement (movement without any aim or goal).
 
### schoolfield
Metabolic development model for mosquitos. This model controls the way mosquitoes develop through their life stages. It depends on temperature and a set of biological parameters that are specific to the mosquito species being simulated.

### controlMeasures
Mosquito population control intervention routines. Contains the behaviour of each one of the mosquito population interventions and how they affect the agents.

### release
Interventions that deal with mosquitos releases. These functions control how often releases occur and their spatial distribution.

### turtlesCreation
Instantiation of the individuals in the environment. This routine parses the information on other files like the maps ones and creates agents at the required locations.

### xmlExport
Routines to export experiments' data into XML format for further analysis (see [exporting files](./docExportingFiles.html) for more detail).

### humanBehaviour 
Human movement and activities.

### mosquitoBehaviour
Mosquitos general life routines. This is the most complex file of the simulation and is explained in detail in [mosquitoes documentation](./docMosquitoVariables.html).

### reproductionRoutines
Mosquitos mating and reproductive routines. This file is separate from the mosquito behaviour one as mating routines present their own complexities.

## Objects

SoNA3BS currently contains eight types of objects that represent the different entities that play a role in the epidemiological transmission of a mosquito-borne disease transmitted by an <i>Aedes aegypti</i> mosquito.

### Mosquitoes

These are the most complicated agents of the simulation. Their behaviour can be extended and modified but care must be taken in doing so as slight changes in parameters might have big impacts due to emergent behaviours and sensitivity.

### Humans

Humans have been programmed with basic behaviours of movement and routines for both habitat destruction and intervention releases can be activated.

### Houses

Each person has a designated house to which they go back to every night. The "contacts" with these houses can be tracked and stored for further analysis.

### Breeding Zones

These are the reopositories where mosquitoes lay their eggs. For now they are containers but their behaviour can be extended to accomodate differential carrying capacity and other heterogeneous scenarios.

### Work Zones

Similar to houses. Each work zone attracts persons who work there and they attend their work zone during daytime.

### Sugar Sources

Agents that produce sugar for mosquitoes to feed upon.

### Sugar Baits

Traps that kill mosquitoes who feed on them.

### Ovitraps

Traps that kill females that lay eggs on them along with the eggs they have oviposited there.

## Interventions Description
Some of the main <i>Aedes</i>-control interventions are included in the model.

### ATSB
Poisoned sugar sources are distributed through the environment to kill both male and female mosquitoes that are trying to feed to fulfill their energetic needs.

### Fogging
Application of insecticide to kill adult mosquitoes.

### Wolbachia
<i>Wolbachia</i> bacteria is added to analyse its transmission blocking effects in the population.

### RIDL
Release of Insects with Dominant Lethal Gene was modelled to see how effective it is in reducing mosquitoes population sizes.

### Ovitraps
Traps intended to kill females in the process of laying eggs along with the eggs they are attempting to oviposit.

## Functions Tree

The following figure shows the way the functions are called in the simulation for mosquito behaviour. This is the standard behaviour of the simulation although it might be extended or certain processes can be deactivated as required for a certain study.

<center>
    <img src="./images/functionsTree.png" style="width: 100%;">
</center>


