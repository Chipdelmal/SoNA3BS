---
title: Documentation
sidebar: mydoc_sidebar
permalink: docFilesStructure.html
folder: mydoc
toc: false
summary: "Simulation Files Structure"
---

## Files

* go: Main simulation file
* global: Global simulation parameters (exported from "ParameterExport.nb")
* auxiliaryFunctions.nls: Functions that perform general unspecific activities
* GoogleMap_HET.nls: Google Map's processed spatial layout in Catemaco, Veracruz
* GoogleMap_HOM.nls: Artificially homogeneous spatial layout with same demographic characteristics as GoogleMap_HET
* randomScenarios.nls: Five different artificially uniform generated scenarios for testing purposes
* movement: Pseudo-Random walking routines for agents
* schoolfield: Metabolic development model for mosquitos
* controlMeasures: Population control intervention routines
* release: Interventions that deal with mosquitos releases with 
* turtlesCreation: Instantiation of the individuals in the environment
* xmlExport: Routines to export experiments' data into XML format
* humanBehaviour: Human movement and 
* mosquitoBehaviour: Mosquitos general life routines
* reproductionRoutines: Mosquitos mating and reproductive routines