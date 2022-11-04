#**AUX_CELL**

##**Generator Flow**

The temperature sensor applies the below described process to translate a specification into a circuit GDS.

Before beginning, we must set up our python environment with the necessary open-source tools. The generator uses a flexible set of tools and will support even more in the future. In the below flow walkthrough, we will use:

•	Yosys for logic synthesis  
•	Openroad for placing and routing  
•	Klayout to produce the final GDS file  
•	Magic for DRC and LVS checks as well as PEX  
•	Ngspice for simulation  

##**Overview of the Align Flow**

![image](https://user-images.githubusercontent.com/67214592/199898136-46696df2-7c9f-47fd-86cc-02b6b7d2e886.png)

##**AUX_CELL Generation Flow**

![20221104_110142](https://user-images.githubusercontent.com/67214592/199897916-63257df9-ae36-4367-9d17-5d45104b0043.jpg)

##**OpenFASOC Stage**

Notebook uses Schemdraw python package to draw schematics of temperature sensor generator. There are two parameters, n_header and n_inverter, which configure the temperature sensor generator.

Temperature Schematic

![image](https://user-images.githubusercontent.com/67214592/199896897-6e86b0d1-5c25-455a-a297-252878e4b3ee.png)

*netlist.py files which are required to generate aux_cells can be found in https://github.com/idea-fasoc/OpenFASOC/docs/source/notebooks/temp-sense-gen/temp_sense_schematic.ipynb

![image](https://user-images.githubusercontent.com/67214592/199897060-88337bc9-37be-4204-98dc-cd6440499c58.png)
