---
title: Exporting Files
sidebar: mydoc_sidebar
permalink: docExportingFiles.html
folder: mydoc
toc: true
summary: "SoNA3BS includes exporting routines that make the analysis of simulations' results easy. These results can be exported in XML format directly from Behaviour Space Interface and can be analysed either with the Mathematica routines we include as part of the simulation or with other analysis software."
---

## General Behaviour

## XML Specification

### Header

Contains a description of the experiment.

### Parameters

Parameters used for a specific setting of the experiment.

#### parameter

#### independent

### Body

Contains the data exported every <i>N</i> ticks of the simulation. It is usually meant to be used for population dynamics data.

#### tick

##### output


### Tail

Information stored when the simulation finishes. Usually used for bites and contacts lists.

#### bitesList

{% highlight r %}
    [
        {[{mID1} {hbIDa,t1} {hbIDb,t2} ... {hbIDz,tn}]} 
        {[{mID2} {hbIDa,t1} {hbIDb,t2} ... {hbIDz,tn}]} 
        ...
        {[{mIDk} {hbIDa,t1} {hbIDb,t2} ... {hbIDz,tn}]} 
    ]
{% endhighlight %}

#### contactsList

#### contactHousesList

#### controlReleasesList