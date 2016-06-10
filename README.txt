==============================================================
--------------------------------------------------------------
************SONA3BS README************************************
--------------------------------------------------------------
==============================================================
SoNA3BS (Social Network Aedes Aegypti Agent-Based Simulation) is an individual-based model created to simulate the population dynamics of Aedes aegypti mosquitoes.
This project is being developed by the Bioinformatics research group of "Tecnológico de Monterrey" university and as part of my Ph.D. thesis in Computer Science.
--------------------------------------------------------------
************OBJECTIVES****************************************
--------------------------------------------------------------
This simulation is being created to help guide global efforts to stop dengue epidemic processes. Although the main objective involves Dengue this simulation can be also used to help in Chikungunya, Zika and Yellow Fever control strategies as they are also spread by the Aedes aegypti mosquito.
--------------------------------------------------------------
************FEATURES******************************************
--------------------------------------------------------------
-The package is divided into two sections: the simulation (NetLogo) and data analysis (Mathematica)
-Data analysis can be performed in other software if necessary
-Data analysis notebooks are included in the package
-Four mosquitoes development stages are included: egg, larva, pupa and adult
-Metabolic development rates are included so that temperature can vary dynamically
-Optimisation techniques can be used through BehaviorSearch in NetLogo
-Novel control strategies are included (Wolbachia, RIDL and sterile males)
-Humans are included in the simulation
-Results of the simulation can be exported in XML format
-Open source code that can be extended
-Code is being documented and thoroughly commented
-Developed on NetLogo to run on Windows, MacOS and Linux
--------------------------------------------------------------
************REQUIREMENTS**************************************
--------------------------------------------------------------
Our IBM requires "Mathematica v10" to run the experiments definitions and analysis notebooks as well as "NetLogo v5.0.3" to run the simulation and "BehaviorSearch v1.0" (both NetLogo and BehaviorSearch are freely available online). Additionally to this Mathematica's package "PajaroLoco" and "SoNA3BSAnalysis" are required for some functionalities (also freely available online).
--------------------------------------------------------------
************INSTALLATION INSTRUCTIONS*************************
--------------------------------------------------------------
-NetLogo: simply download the program from the project's download section (https://ccl.northwestern.edu/netlogo/)
-BehaviorSearch: download the program from the project's download section (http://behaviorsearch.org/) and please note that BehaviorSearch was created to run on previous versions of NetLogo so it might not be compatible with newer ones
-Mathematica: unfortunately this is a non-free software so you have to buy it from Wolfram (http://www.wolfram.com/mathematica/)
-PajaroLoco: follow the instructions on the following link (https://www.youtube.com/watch?v=0h3WvMk60dg)
-SoNA3BS: just download the folder with the programs' files.
--------------------------------------------------------------
************SIMULATION FILES DESCRIPTION**********************
--------------------------------------------------------------
auxiliaryFunctions.nls: Functions that perform general unspecific activities
GoogleMap_HET.nls: Google Map's processed spatial layout in Catemaco, Veracruz
GoogleMap_HOM.nls: Artificially homogeneous spatial layout with same demographic characteristics as GoogleMap_HET
randomScenarios.nls: Five different artificially uniform generated scenarios for testing purposes
movement: Pseudo-Random walking routines for agents
schoolfield: Metabolic development model for mosquitos

--------------------------------------------------------------
************CONTACT*******************************************
--------------------------------------------------------------
mail: sanchez.hmsc@itesm.com
website: https://sites.google.com/site/sona3bs/ 
