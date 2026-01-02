# Template BeBOP PCR Protocol
Hell world!
## MIOP: Minimum Information about an Omics Protocol

### 1. 
| MIOP Term             | Savings |
| --------------------- | ------- |
| methodology category  | omics analysis    |
| project               | NOAA PMEL OME Program     |
| purpose               | eDNA sampling     |
| analyses              |     |
| geographical location |      |
|broad-scale environmental context | |
|local environmental context | |
|environmental medium | |
|target | |
|creator | |
|materials required | |
|skills required | |
|time required | |
|personnel required | |
|language | |
|issued | |
|audience | |
|publisher | |
|hasVersion | |
|license | |
|maturity level | |

See https://github.com/BeBOP-OBON/miop/blob/main/model/schema/terms.yaml for list and definitions.

## AUTHORS
### 2.
| PREPARED BY          | AFFILIATION | ORCID (visist https://orcid.org/) | DATE |
| --------------------- | --------------------- |--------------------- |------- |

## RELATED PROTOCOLS

### 3. 
| PROTOCOL NAME          | LINK | ISSUER/AUTHOR | RELEASE DATE |
| --------------------- | --------------------- |--------------------- | --------------------- |
| MBARI MBON eDNA CO1 PCR V2 | https://github.com/MBARI-BOG/MBON-Protocols/blob/main/eDNA_COI_PCR_V2.md	|Jacoby Baker|	3/20/18|
## ACRONYMS AND ABBREVIATIONS
### 4. 
| ACRONYMS / ABBREVIATIONS             | DEFINITION |
| --------------------- | ------- |
| eDNA | environmental DNA |

## GLOSSARY
### 5. 
| SPECIALIZED TERM             | DEFINITION |
| --------------------- | ------- |
| eDNA | environmental DNA |

## BACKGROUND

### 6. Summary
This protocol is for amplifying the cytochrome c oxidase subunit I (COI) mitochondrial gene in eukaryotes. The primers (forward: mlCOIintF, reverse: HCO2198) were first presented in Leray et al. 2013 (forward) and Folmer et al. 1994 (reverse).

This amplification can be the first of a two-step PCR protocol for Illumina sequencing library preparation. It does not include the second PCR step in which sample-specific barcodes and sequencing adapters are attached.

### 7. Method description and rationale
This protocol was chosen because it has been widely and historically used in marine eDNA time series by the Monterey Bay Aquarium Research Institute (MBARI), a leader in the field of eDNA research and an important partner in the Marine Biodiversity Observation Network (MBON). The primers encompass a broad range of eukaryotic taxa including single-celled phytoplankton (e.g., dinoflagellates, diatoms, and haptophytes) as well as metazoans (e.g., molluscs and arthropods) and the amplification protocol is accessible to most molecular biology labs.

### 8. Spatial coverage and environment(s) of relevance
This protocol has been used to amplify extracted DNA from filtered sea water samples taken from marine coastal stations off the western coast of North America (primarily off California, Oregon, Washington, and Alaska).

sea water [ENVO:00002149]
http://purl.obolibrary.org/obo/ENVO_00002149

### 9. Personnel Required

One person with molecular biology experience.

### 10. Safety

This protocol does not involve any hazardous chemicals, although standard precautions including wearing PPE should be take to avoid skin and eye exposure to reagents.

### 11. Training Requirements
Molecular biology training (including, at a minimum, sterile technique, pipetting small volumes, and programming and running PCR thermocyclers) is required to conduct this protocol.

### 12. Time needed to execute the procedure
PCR preparation and running the PCR protocol for a single 96-well plate takes 3.5 hours. Preparing and running a large gel for 96 samples takes 2 hours, including a 75 min run-time. 

*Additional plates (2-3) can be run simultaneously without greatly increasing the time needed.

## EQUIPMENT

### 13.
| DESCRIPTION          | PRODUCT NAME/MODEL | MANUFACTURER | QUANTITITY | REMARK | 
| --------------------- | --------------------- |--------------------- |------- | ------- |
| **Durable Equipment**|||||
|Thermocycler||||
|Pipetter: 1-10 μl |	Pipetman P10L |	Gilson |	1	| Can be substituted with any accurate pipetter. |
|** Optional Equipment**|||||

## STANDARD OPERATING PROCEDURE
### 14. 
In the following SOP, please use the exact names of equipment as noted in the table above.

Provide a step-by-step description of the protocol. The identification of difficult steps in the protocol and the provision of recommendations for the execution of those steps are encouraged.

## PREPARATION
### 15. 
Samples are collected in the field and extracted in the lab using the below protocols:


### 16. 
Before Starting the PCR Setup:

All workspaces within the BSC are cleaned with 10% bleach followed by a 70% ethanol wipe down. Pipets, racks, and equipment (e.g., vortex) are also wiped down with bleach and ethanol. All materials within the BSC are UV'd for 30 minutes before starting the protocol using BSC UV light. Pipets are wiped down with ethanol additionally sterilized in a UV crosslinker for 2 minutes regularly. 

## PCR

### 17.
Please specify the actions you took to amplify the previously extracted DNA and the equipment and primers you used (ingredients for the PCR reaction, number of triplicates, PCR cycle parameter)

| PCR PRIMER NAME            | DIRECTION | SEQUENCE (5' -> 3') |
| --------------------- | ------- | ------- |
| Leray F / mlCOIinfF	| forward	| GGWACWGGWTGAACWGTWTAYCCYCC |
| Folmer R / HCO2198	| reverse	| TAAACTTCAGGGTGACCAAAAAATCA |

The forward and reverse primers used. Primary and alternative primer names are provided.

### 18.

Positive Control?

### 19. 

| REAGENTS           | ONE REACTION (µL) | 96x reactions (µL) |
| --------------------- | ------- | ------- |
|AmpliTaq Gold Fast PCR master mix (Applied Biosystems)	|12.5	|1300|
|5 uM Forward Primer	|1|	104|
|5 uM Reverse Primer	|1|	104|
|Nuclease-Free Water	|8.5|	884|
|Template DNA|	2	||
|Total	|25|	2392|
The Master Mix components and volumes used in the reaction.

### 20.

| PCR STEP           | TEMPERATURE | DURATION | REPETITION|
| --------------------- | ------- | ------- |------- |
|Initial denaturation	95°C	10 min	1X|
|Denaturation|	94°C|	10 s|	16X|
|Annealing|	62°C - 47°C	|30 s	|16X|
|Extension / elongation|	68°C|	60 s|	16X|
|Denaturation|	94°C	|10 s|	25X|
|Annealing|	46°C	|30 s|	25X|
|Extension / elongation|	68°C|	60 s|	25X|
|Final elongation|	7°C|	10 min|	1X|
|Hold	|4°C|	Inf.|	1X|
COI thermocycling protocol. In step 3, the annealing temperature in the first cycle is 62°C and it decreases by 1°C with every subsequent cycle, with the 16th cycle running at 47°C (i.e., a touchdown PCR).

## PCR CLEAN UP

### 21.

## QUALITY CONTROL
### 22.
After primary PCR amplification of the marker region, the PCR products are run through a 1% agarose gel to confirm the presence of target bands and absence of non-specific amplification across environmental samples as well as the absence of amplification in no-template controls (NTCs). Target bands should be ~313 bp in length. 

## BASIC TROUBLESHOOTING GUIDE

### 23.
Identify known issues associated with the procedure, if any.

Provide troubleshooting guidelines when available.
### 24.
Issue: Streaking is observed for sample wells in gel but positive control is a normal band. 

Solution: Try diluting samples 1:10 with RO water before adding to Master Mix
### 25. 
Issue:

Solution: 

## REFERENCES

### 26.
- Leray et al. 2013. A new versatile primer set targeting a short fragment of the mitochondrial COI region for metabarcoding metazoan diversity: application for characterizing coral reef fish gut contents. Frontiers in Zoology. 10 (34). https://doi.org/10.1186/1742-9994-10-34
- Folmer et al. 1994. DNA primers for amplification of mitochondrial cytochrome c
oxidase subunit I from diverse metazoan invertebrates. Molecular Marine Biology and Biotechnology 3 (5): 294-299. PMID: 7881515

## APPENDIX A: DATASHEETS

### 27.
Link templates (e.g. preformatted spreadsheets) used to record measurements and report on the quality of the data as well as any documents such as manufacturer specifications, images, etc that support this protocol. Please include a short note describing the document’s relevance.
