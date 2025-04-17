# slope_rockbolt_optimisation
Integration of Rhino/Grasshopper and Rocscience RocSlope3 for evaluation of rock block stabilities and bolting optimisation

## Citation/publication
This repository is associated with a manuscript of a journal article (published in the Journal of Rock Mechanics and Geotechnical Engineering)
- **Title:** Slope rockbolting using key block theory: Force transfer and artificial intelligence-assisted multi-objective optimisation 
- **Authors:** Jessica Ka Yi Chiu, Charlie Chunlin Li, Ole Jakob Mengshoel, Vidar Kveldsvik

### How to cite
Chiu JKY, Li CC, Mengshoel OJ, Kveldsvik V (2025) Slope rockbolting using key block theory: Force transfer and artificial intelligence-assisted multi-objective optimisation. Journal of Rock Mechanics and Geotechnical Engineering. https://doi.org/10.1016/j.jrmge.2025.03.026

Two Grasshopper scripts are included in this repository:
- Progressive failure analysis with force transfer **[ProgressiveFailureAnalysis_ForceTransfer.gh]**
- Optimisation of rockbolting **[RockBoltingOptim.gh]**


## Software
### Rhino
- Rhino Version 7 SR37 (7.37.24107.15001, 2024-04-16)


### Grasshopper Plug-in List
- Volvox                         by CITA (0.3.0.0)
- MetaHopper                     by Andrew Heumann (1.2.4)
- Pufferfish                     by Michael Pryor (2.9.0.0)
- Opossum2_0_Proto_A             by 'unknown author' (3.0.3.0)
- Tunny                          by hrntsm (0.12.0)
- LunchBox                       by 'unknown author' (2016.3.21.0)
- CockroachGH<sup>1</sup>        by iboisepfl  (0.01 Rhino 7) 
- Pancake                        by Keyu Gan (2.5.0.0)
- Anemone                        by Mateusz Zwierzycki (0.4)
- MeshEdit Components            by [uto] (2.0.0.0)
- eleFront                       by Front, Inc. (5.1.8)
- TT Toolbox                     by CORE studio | Thornton Tomasetti (1.9.6353.28734)
- Human                          by 'unknown author' (1.2.0)

<sup>1</sup> To install CockroachGH, first go to https://github.com/9and3/Cockroach/tree/Cockroach/Build, then download from the folder "RhinoCppPlugin" with the relevant Rhino version that you use, and download "CockroachGH.zip". Finally, unblock and unzipped all the downloaded files to the Components Folder in Grasshopper.


## Instructions
### [ProgressiveFailureAnalysis_ForceTransfer.gh]
- Inputs to this script are two OBJ files, separately for blocks and joints, exported from RocSlope3
- In RocSlope3, after the computation of blocks and kinematic analysis is completed, in the result tab, under "Results Set" in Properties, choose "All Valid Blocks". Then go to File > Export > Export Blocks, under "Blocks to Include", choose "Current Result Set", then export to OBJ file type. Follow the same procedure for exporting "Blocks" and "Joints".


### [RockBoltingOptim.gh]
- for selecting points that snap to PointCloud in Rhino. "Onsnap" should be turned on. See the following settings in Rhino (at the bottom of the Rhino-window):
![image](https://github.com/norwegian-geotechnical-institute/slope_rockbolt_optimisation/assets/74724769/bd528fdc-39b2-40a5-8694-d9a3464a53c4)
