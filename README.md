# Git-Sathish-VSD-IAT
Digital VLSI SoC Design and Planning program-Nasscom
README.md
The LAB for day 2 gives the complete flow of the Floor planning and the placement process
Section 2 tasks:-
1.	Run 'picorv32a' design floorplan using OpenLANE flow and generate necessary outputs.
2.	Calculate the die area in microns from the values in floorplan def.
3.	Load generated floorplan def in magic tool and explore the floorplan.
4.	Run 'picorv32a' design congestion aware placement using OpenLANE flow and generate necessary outputs.
5.	Load generated placement def in magic tool and explore the placement.
Area of die in microns = Die width in micron * die hight in micron.
•	All section 2 logs, reports and results can be found in following run folder:

After the Synthesis process, type the command for running the Floor planning

Cd logs/floorplan 

Desktop/work/tools/openlande_working_dir/openlane/designs/picorv32a/runs/10 09_18 53/floorplan $less ioplacer.log 
Check for vertical metal : 5 and horizontal metal : 4

Check config.tcl in separate window.
Check for vertical metal : 4 and horizontal metal : 3

Note : runs folder config.tcl.
Desktop/work/tools/openlande_working_dir/openlane/designs/picorv32a /runs / 10 09 _18 53 $ less config.tcl 

To check floor plan 
Desktop/work/tools/openlande_working_dir/openlane/designs/picorv32a/runs/10 09_18 53
Cd results/floor plan 
Ls -ltr
Desktop/work/tools/openlande_working_dir/openlane/designs/picorv32a/runs/10 09_18 53/results/floorplan $lesspicorv32a.floorplan.def

You will find die area
Diearea ( 0 0 ) ( 1046535 798380 ) 
Units distance Microns 1000
1 microns = 1000 database units
Divide by thousand to get value in micro mtrs.


Cell design flow :
Library and suer -defined specs
Voltage level and noise level
Metal layers
Pin location 
Drawn gate length

Cell design flow : Design steps :
Circuit design ( out put of circuit design stage using spice model is circuit description language)
Layout design ( output of layout design is GDSII, LEF, extracted spice netlist )
Characterization ( out put of characterization is timing , nosie, power , ,libs, function

Characterization flow based on the input we have : 
-Reading the models and tek files comes with the model ( they come out of the factory or foundry)
2 step : read extracted spice netlist
3rd step Recognize the behavior of the buffer 
4th step : to read the sub circuit of the inverter
5th sept : Attach the power sources.
6th step : apply the stimulus . Varity of stimulus available. Like input
7th step : provide necessary out put capacitance 
8th step : simulation command 
Characterization software GUNA :software will generate timing, nosie, power , .libs and functions

