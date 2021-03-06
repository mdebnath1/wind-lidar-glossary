[![CI](https://github.com/IEA-Wind-Task-32/wind-lidar-glossary/workflows/CI/badge.svg)](https://github.com/IEA-Wind-Task-32/wind-lidar-glossary/actions?query=workflow%3ACI)

# Wind lidar glossary
This repository provides the source file for a glossary of terms for wind lidar (see the file, `glossary.ttl`). This glossary can be used to help organise and explore data, publications and software.

[**Check out a human-friendly version of the repository**](https://data.windenergy.dtu.dk/ontologies/view/IEATask32Glossary/en/).

## Glossary, ontology, taxonomy, ...
There are two main files in this repository:
- The Task 32 wind lidar glossary (`glossary.ttl`) is a controlled vocabulary about wind lidar that includes a hierarchy, synonyms, and interrelationships.
- The Task 32 ontology (`ontology.ttl`) includes more custom information

Confused? [Read more about the difference between a glossary and ontology](https://asistdl.onlinelibrary.wiley.com/doi/epdf/10.1002/bult.2013.1720390211).

## Link to the OpenLidar module definitions
This glossary includes terms used to describe the design of a wind lidar. These are structured according to the modular layout proposed in the OpenLidar project.

![The OpenLidar modular wind lidar architecture](https://github.com/e-WindLidar/OpenLidarModuleDefinitions/blob/master/OpenLidarModules.png)

For more details about OpenLidar see Zenodo.

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3414197.svg)](https://doi.org/10.5281/zenodo.3414197)


## How to use this

### To define the inputs for simulations
The glossary defines a structure for the data that describe the design of a wind lidar and how it is used. This could be encoded in a YAML file and used as the input to a lidar simulation.

### To define a reference lidar device
The glossary defines a structure for the data that describe the design of a wind lidar. A very incomplete example of how this could be used is included as [`reference-designs/staring_lidar.yaml`](https://github.com/IEA-Wind-Task-32/wind-lidar-glossary/blob/main/reference-designs/staring_lidar.yml.

## Implementation

### Syntax
The file is written using the [Simple Knowledge Organisation System (skos) schema](https://www.w3.org/2009/08/skos-reference/skos.html). It can be checked for conformance to the skos schema using e.g. the [SPARNA skos verification tool](http://labs.sparna.fr/skos-testing-tool/test?url=https://raw.githubusercontent.com/IEA-Wind-Task-32/wind-lidar-glossary/main/glossary.ttl&rules=anr,chr,dcc,dlv,el,hr,husv,ilc,ipl,ml,mri,ncl,oc,oilt,ol,otc,rc,rrc,strc,tchbc,uc,ucil,urc,usr&format=html).

### Building the glossary and ontology files
The glossary and ontology files are built from information contained in the text files in this repository.
- the glossary is created by concatenating `00_headers.ttl` with all of the other text files.
- the ontology is created by concatenating `00_headers.ttl` and `01_parameters.ttl` with all of the other text files.

The ontology and glossary are created automatically by a CI process on commit.


# To contribute
The data in the glossary can only be changed by the repository maintainers. The glossary data is protected to avoid misuse or abuse, and to help provide a clear way for modifying the data in the repository
- [Suggest a new definition](https://github.com/IEA-Wind-Task-32/wind-lidar-glossary/issues/new?assignees=&labels=&template=new-definition.md&title=%5BNew+definition%5D).
- [Change a definition](https://github.com/IEA-Wind-Task-32/wind-lidar-glossary/issues/new?assignees=&labels=&template=change-definition.md&title=%5BChange+a+definition%5D).

For any other feedback please [raise an issue](https://github.com/IEA-Wind-Task-32/wind-lidar-glossary/issues/new?assignees=&labels=&template=new-definition.md&title=%5BNew+definition%5D).

Contributions will become part of this repository according to the terms of the contributor agreement.

# Maintainers
This repository is maintained by
- [Andy Clifton](https://github.com/andyclifton), IEA Wind Task 32 Operating Agent
- [Nikola Vasiljevic](niva83) at the Danish Technical University.

... and uses contributions from
- [Francisco Costa](https://github.com/pacocosta)


# Contact
Questions, comments, and feedback about the glossary should be [shared as an issue](https://github.com/IEA-Wind-Task-32/wind-lidar-glossary/issues/new/choose) or sent to ieawind.task32@ifb.uni-stuttgart.de.
