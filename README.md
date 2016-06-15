# SoNA3BS: Social Network Aedes Aegypti Agent-Based Simulation

SoNA3BS is an individual-based model created to simulate the population dynamics of Aedes aegypti mosquitoes.
This project is being developed by the Bioinformatics research group of Tecnológico de Monterrey in collaboration with UC Berkeley.

## Objectives

This simulation is being created to help guide global efforts to stop dengue epidemic processes. Although the main objective involves Dengue this simulation can be also used to help in Chikungunya, Zika and Yellow Fever control strategies as they are also spread by the Aedes aegypti mosquito.

## Features

* The package is divided into two sections: the simulation (NetLogo) and data analysis (Mathematica)
* Data analysis can be performed in other software if necessary
* Data analysis notebooks are included in the package
* Four mosquitoes development stages are included: egg, larva, pupa and adult
* Metabolic development rates are included so that temperature can vary dynamically
* Optimisation techniques can be used through BehaviorSearch in NetLogo
* Novel control strategies are included (Wolbachia, RIDL and sterile males)
* Humans are included in the simulation
* Results of the simulation can be exported in XML format
* Open source code that can be extended
* Code is being documented and thoroughly commented
* Developed on NetLogo to run on Windows, MacOS and Linux

## Requirements

Our IBM requires "Mathematica v10" to run the experiments definitions and analysis notebooks as well as "NetLogo v5.0.3" to run the simulation and "BehaviorSearch v1.0" in case optimisation routines are desired (both NetLogo and BehaviorSearch are freely available online). Additionally to this Mathematica's package "PajaroLoco" and "SoNA3BSAnalysis" are required for some functionalities (also freely available online).

## Installation Instructions

* NetLogo: simply download the program from the project's download section (https://ccl.northwestern.edu/netlogo/)
* BehaviorSearch: download the program from the project's download section (http://behaviorsearch.org/) and please note that BehaviorSearch was created to run on previous versions of NetLogo so it might not be compatible with newer ones
* Mathematica: unfortunately this is a non-free software so you have to buy it from Wolfram (http://www.wolfram.com/mathematica/)
* PajaroLoco: follow the instructions on the following link (https://www.youtube.com/watch?v=0h3WvMk60dg)
* SoNA3BS: just download the folder with the programs' files.

## Simulation's Files Brief Description
This is just for reference. For a more updated and thorough version look at the definitions within the files or the documentation folder.

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

## Important Notes

* RIDL is sometimes referred to as Oxitec or Oxitech by mistake. Sorry about the lack of consistency in the code and the spelling error.

## Contact

* mail: sanchez.hmsc@itesm.com
* website: https://sites.google.com/site/sona3bs/ 

## Licence

<a rel="license" href="http://creativecommons.org/licenses/by-nc/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc/4.0/88x31.png" /></a><br /><span xmlns:dct="http://purl.org/dc/terms/" property="dct:title">SoNA3BS</span> by <a xmlns:cc="http://creativecommons.org/ns#" href="https://sites.google.com/site/sona3bs/" property="cc:attributionName" rel="cc:attributionURL">Héctor Manuel Sánchez Castellanos</a> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc/4.0/">Creative Commons Attribution-NonCommercial 4.0 International License</a>.
