# slope_rockbolt_optimisation
Integration of Rhino/Grasshopper and Rocscience RocSlope for evaluation of rock block stabilities and bolting optimisation

## Software
### Rhino
- Rhino Version 7 SR34 (7.34.23267.11001, 2023-09-24)


### Grasshopper Plug-in List
- Volvox                         by CITA (0.3.0.0)
- MetaHopper                     by Andrew Heumann (1.2.4)
- Pufferfish                     by Michael Pryor (2.9.0.0)
- Opossum2_0_Proto_A             by 'unknown author' (3.0.3.0)
- Tunny                          by hrntsm (0.9.0)
- LunchBox                       by 'unknown author' (2016.3.21.0)
- CockroachGH<sup>1</sup>                    by iboisepfl  (0.01 Rhino 7) 
- Pancake                        by Keyu Gan (2.5.0.0)

<sup>1</sup> To install CockroachGH, first go to https://github.com/9and3/Cockroach/tree/Cockroach/Build, then download from folder "RhinoCppPlugin" with the relevant Rhino version that you use, and download "CockroachGH.zip". Finally, unblock and unzipped all the downloaded files to the Components Folder in Grasshopper.

## Content
- Settings.json for the input setting parameters for Tunny, where all seeds are set to "42". See how to do that https://github.com/hrntsm/Tunny/discussions/169#discussioncomment-8242220
- Example Rhino file [TO-DO]
- Grasshopper file
- Example output file of all trials [TO-DO]
- Example output file of all trials showing pareto solutions [TO-DO]

## Instructions
- for selecting points that snap to PointCloud in Rhino. "Onsnap" should be turned on. See the following settings in Rhino (at the bottom of the Rhino-window):
![image](https://github.com/norwegian-geotechnical-institute/slope_rockbolt_optimisation/assets/74724769/bd528fdc-39b2-40a5-8694-d9a3464a53c4)
