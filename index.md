---
title: Social Network Aedes Aegypti Agent-Based Simulation
keywords: homepage
sidebar: mydoc_sidebar
permalink: index.html
summary: 
toc: false
summary: SoNA3BS is an individual-based model created to simulate the population dynamics of Aedes aegypti mosquitoes. This project is being developed by the Bioinformatics research group of Tecnológico de Monterrey in collaboration with UC Berkeley.
---

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
* SoNA3BS: just download the folder with the programs' files.
* BehaviorSearch: download the program from the project's download section (http://behaviorsearch.org/) and please note that BehaviorSearch was created to run on previous versions of NetLogo so it might not be compatible with newer ones
* Mathematica: unfortunately this is a non-free software so you have to buy it from Wolfram (http://www.wolfram.com/mathematica/)
* PajaroLoco: follow the instructions on the following link (https://bitbucket.org/chipdelmal/pajarolocopublic)
* BehaviourSpaceInterface: download and install following the same instruccions as the ones for PajaroLoco (https://bitbucket.org/chipdelmal/behaviorspaceinterface)

## Important Notes

* RIDL is sometimes referred to as Oxitec or Oxitech by mistake. Sorry about the lack of consistency in the code and the spelling error.

## Contact

* mail: sanchez.hmsc@itesm.com