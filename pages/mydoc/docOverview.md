---
title: Documentation
sidebar: mydoc_sidebar
permalink: docOverview.html
folder: mydoc
toc: true
summary: "Documentation main page"
---

## Files Structure

### go
Main simulation file

### global
Global simulation parameters (exported from "ParameterExport.nb")

### auxiliaryFunctions.nls
Functions that perform general unspecific activities

### GoogleMap_HET.nls
Google Map processed spatial layout in "Catemaco, Veracruz"

### GoogleMap_HOM.nls
Artificially homogeneous spatial layout with same demographic characteristics as GoogleMap_HET

### randomScenarios.nls
Five different artificially uniform generated scenarios for testing purposes

### movement
Pseudo-Random walking routines for agents
 
### schoolfield
Metabolic development model for mosquitos

### controlMeasures
Population control intervention routines

### release
Interventions that deal with mosquitos releases with 

### turtlesCreation
Instantiation of the individuals in the environment

### xmlExport
Routines to export experiments' data into XML format

### humanBehaviour 
Human movement and 

### mosquitoBehaviour
Mosquitos general life routines

### reproductionRoutines
Mosquitos mating and reproductive routines

## Objects

SoNA3BS currently contains eight types of objects that represent the different entities that play a role in the epidemiological transmission of a mosquito-borne disease transmitted by an <i>Aedes aegypti</i> mosquito.

### Mosquitoes

### Humans

### Houses

### Breeding Zones

### Work Zones

### Sugar Sources

### Sugar Baits

### Ovitraps

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

<center>
{% include image.html file="functionsTree.png" alt="Functions Tree" caption="Function calls tree of the main simulation."  max-width=800 %}
</center>


