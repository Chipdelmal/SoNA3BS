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

## Functions Tree

<center>
{% include image.html file="functionsTree.png" alt="Functions Tree" caption="Function calls tree of the main simulation."  max-width=800 %}
</center>

