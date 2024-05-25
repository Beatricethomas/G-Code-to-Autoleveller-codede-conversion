# G-Code-to-Autoleveller-codede-conversion
# Aim
To convert the G-Code into Auto leveler Code using Autoleveller software.
# Software Required
Autoleveller
# Procedure
1.Open the Autoleveller software </br>
2. Select the software option as Mach3 </br>
3. Load the G Code - Click “Browse for G Code” button and open your Engraving G-Code.</br>
4. After loading G-Code below a window will open. In that Select Unit “millimeters”</br>
5. Create level code and the save the code</br>
6. Remove the unwanted portion from your Auto Levelled G-Code. </br>
7. Add few lines in the code and save the file</br>
8. Follow this same procedure for remaining all G-codes ( Drill and cut).</br>
9.Autolevelling should be done for only engraving file.</br>

# Theory

PCB AutoLEVLER is a software tool used in conjunction with CNC (Computer Numerical Control) machines for PCB (Printed Circuit Board) manufacturing. Its primary function is to compensate for variations in the flatness of the substrate or the surface of the copper-clad board. This compensation ensures that the depth of milling or engraving remains consistent across the entire board, even if the board itself is not perfectly flat.

## Purpose:
PCB AutoLEVLER is designed to address the following challenges in PCB manufacturing:
### Substrate Variations: 
Substrates or copper-clad boards may have variations in flatness, which can affect the accuracy of milling or engraving depths.
### Consistency: 
Ensuring consistent depth of milling or engraving across the entire PCB surface is crucial for precise PCB fabrication.
## Functionality:
### Automatic Depth Adjustment: 
PCB AutoLEVLER automatically adjusts the Z-axis depth of the milling or engraving tool based on the surface variations of the PCB substrate. It dynamically compensates for any unevenness in the board to maintain a consistent depth of cut.
### Surface Mapping: 
The software typically includes a surface mapping feature that scans the surface of the PCB and generates a digital map indicating areas of variation in flatness. This map is then used to adjust the tool's depth as it moves across the board.
### Integration with CNC Machines:
PCB AutoLEVLER is integrated with CNC machines through compatible control software. It communicates with the CNC controller to adjust tool depth in real-time during the milling or engraving process.
## Benefits:
### Improved Accuracy: 
By compensating for surface variations, PCB AutoLEVLER helps maintain precise milling or engraving depths, resulting in higher accuracy and quality of PCBs.
### Time Savings:
The software automates the depth adjustment process, saving time compared to manual adjustments or rework caused by uneven milling depths.
Reduced Waste: Consistent depth of milling or engraving minimizes the risk of errors and waste material, resulting in cost savings for PCB manufacturers.
### Compatibility:
PCB AutoLEVLER is typically compatible with a range of CNC machines commonly used in PCB manufacturing, including routers, engravers, and milling machines. It may also integrate with various CAD/CAM software packages to streamline the design-to-manufacturing workflow.
## Implementation:
Implementing PCB AutoLEVLER involves installing the software on a computer connected to the CNC machine and configuring it to work with the specific machine and PCB design requirements. Training may be provided to operators on how to use the software effectively.
Overall, PCB AutoLEVLER plays a vital role in ensuring the accuracy, consistency, and efficiency of PCB manufacturing processes, particularly in environments where precise milling or engraving is essential for high-quality PCBs.
# Auto leveller Code
### Engraving Code
```
M6T5
G54
G0 X0 Y0
G0 Z5
M91


G31 Z-10 F100
G92 Z0
G0 Z2
G31 Z-1 F50
G92 Z0
G0 Z2
G0 X0 Y0
G31 Z-1 F100
#500=#2002
G0 Z2
G0 X10.51956 Y0
G31 Z-1 F100
#501=#2002
G0 Z2
G0 X21.03911 Y0
G31 Z-1 F100
#502=#2002
G0 Z2
G0 X31.55867 Y0
G31 Z-1 F100
#503=#2002
G0 Z2
G0 X42.07822 Y0
G31 Z-1 F100
#504=#2002
G0 Z2
G0 X52.59778 Y0
G31 Z-1 F100
#505=#2002
G0 Z2
G0 X63.11733 Y0
G31 Z-1 F100
#506=#2002
G0 Z2
G0 X73.63689 Y0
G31 Z-1 F100
#507=#2002
G0 Z2
G0 X84.15644 Y0
G31 Z-1 F100
#508=#2002
G0 Z2
G0 X94.676 Y0
G31 Z-1 F100
#509=#2002
G0 Z2
G0 X94.676 Y10.332
G31 Z-1 F100
#519=#2002
G0 Z2
G0 X84.15644 Y10.332
G31 Z-1 F100
#518=#2002
G0 Z2
G0 X73.63689 Y10.332
G31 Z-1 F100
#517=#2002
G0 Z2
G0 X63.11733 Y10.332
G31 Z-1 F100
#516=#2002
G0 Z2
G0 X52.59778 Y10.332
G31 Z-1 F100
#515=#2002
G0 Z2
G0 X42.07822 Y10.332
G31 Z-1 F100
#514=#2002
G0 Z2
G0 X31.55867 Y10.332
G31 Z-1 F100
#513=#2002
G0 Z2
G0 X21.03911 Y10.332
G31 Z-1 F100
#512=#2002
G0 Z2
G0 X10.51956 Y10.332
G31 Z-1 F100
#511=#2002
G0 Z2
G0 X0 Y10.332
G31 Z-1 F100
#510=#2002
G0 Z2
G0 X0 Y20.664
G31 Z-1 F100
#520=#2002
G0 Z2
G0 X10.51956 Y20.664
G31 Z-1 F100
#521=#2002
G0 Z2
G0 X21.03911 Y20.664
G31 Z-1 F100
#522=#2002
G0 Z2
G0 X31.55867 Y20.664
G31 Z-1 F100
#523=#2002
G0 Z2
G0 X42.07822 Y20.664
G31 Z-1 F100
#524=#2002
G0 Z2
G0 X52.59778 Y20.664
G31 Z-1 F100
#525=#2002
G0 Z2
G0 X63.11733 Y20.664
G31 Z-1 F100
#526=#2002
G0 Z2
G0 X73.63689 Y20.664
G31 Z-1 F100
#527=#2002
G0 Z2
G0 X84.15644 Y20.664
G31 Z-1 F100
#528=#2002
G0 Z2
G0 X94.676 Y20.664
G31 Z-1 F100
#529=#2002
G0 Z2
G0 X94.676 Y30.996
G31 Z-1 F100
#539=#2002
G0 Z2
G0 X84.15644 Y30.996
G31 Z-1 F100
#538=#2002
G0 Z2
G0 X73.63689 Y30.996
G31 Z-1 F100
#537=#2002
G0 Z2
G0 X63.11733 Y30.996
G31 Z-1 F100
#536=#2002
G0 Z2
G0 X52.59778 Y30.996
G31 Z-1 F100
#535=#2002
G0 Z2
G0 X42.07822 Y30.996
G31 Z-1 F100
#534=#2002
G0 Z2
G0 X31.55867 Y30.996
G31 Z-1 F100
#533=#2002
G0 Z2
G0 X21.03911 Y30.996
G31 Z-1 F100
#532=#2002
G0 Z2
G0 X10.51956 Y30.996
G31 Z-1 F100
#531=#2002
G0 Z2
G0 X0 Y30.996
G31 Z-1 F100
#530=#2002
G0 Z2
G0 X0 Y41.328
G31 Z-1 F100
#540=#2002
G0 Z2
G0 X10.51956 Y41.328
G31 Z-1 F100
#541=#2002
G0 Z2
G0 X21.03911 Y41.328
G31 Z-1 F100
#542=#2002
G0 Z2
G0 X31.55867 Y41.328
G31 Z-1 F100
#543=#2002
G0 Z2
G0 X42.07822 Y41.328
G31 Z-1 F100
#544=#2002
G0 Z2
G0 X52.59778 Y41.328
G31 Z-1 F100
#545=#2002
G0 Z2
G0 X63.11733 Y41.328
G31 Z-1 F100
#546=#2002
G0 Z2
G0 X73.63689 Y41.328
G31 Z-1 F100
#547=#2002
G0 Z2
G0 X84.15644 Y41.328
G31 Z-1 F100
#548=#2002
G0 Z2
G0 X94.676 Y41.328
G31 Z-1 F100
#549=#2002
G0 Z2
G0 X94.676 Y51.66
G31 Z-1 F100
#559=#2002
G0 Z2
G0 X84.15644 Y51.66
G31 Z-1 F100
#558=#2002
G0 Z2
G0 X73.63689 Y51.66
G31 Z-1 F100
#557=#2002
G0 Z2
G0 X63.11733 Y51.66
G31 Z-1 F100
#556=#2002
G0 Z2
G0 X52.59778 Y51.66
G31 Z-1 F100
#555=#2002
G0 Z2
G0 X42.07822 Y51.66
G31 Z-1 F100
#554=#2002
G0 Z2
G0 X31.55867 Y51.66
G31 Z-1 F100
#553=#2002
G0 Z2
G0 X21.03911 Y51.66
G31 Z-1 F100
#552=#2002
G0 Z2
G0 X10.51956 Y51.66
G31 Z-1 F100
#551=#2002
G0 Z2
G0 X0 Y51.66
G31 Z-1 F100
#550=#2002
G0 Z2
G0 X0 Y61.992
G31 Z-1 F100
#560=#2002
G0 Z2
G0 X10.51956 Y61.992
G31 Z-1 F100
#561=#2002
G0 Z2
G0 X21.03911 Y61.992
G31 Z-1 F100
#562=#2002
G0 Z2
G0 X31.55867 Y61.992
G31 Z-1 F100
#563=#2002
G0 Z2
G0 X42.07822 Y61.992
G31 Z-1 F100
#564=#2002
G0 Z2
G0 X52.59778 Y61.992
G31 Z-1 F100
#565=#2002
G0 Z2
G0 X63.11733 Y61.992
G31 Z-1 F100
#566=#2002
G0 Z2
G0 X73.63689 Y61.992
G31 Z-1 F100
#567=#2002
G0 Z2
G0 X84.15644 Y61.992
G31 Z-1 F100
#568=#2002
G0 Z2
G0 X94.676 Y61.992
G31 Z-1 F100
#569=#2002
G0 Z2
G0 X0 Y0 Z20



M91
M3 S12000




M7
G0 X32.789 Y18.476
G0 Z0











G1 Y18.476 Z[#100 + -0.2]
G0 Z2
G0 X35.185 Y17.171
G0 Z0

































G0 Z2

G00 X00 Y00

M5
M2
%



```
### Drill Code
```
M6T5
G54
G0 X0 Y0
G0 Z5
M91



M03 S12000

G4 P5



G00 X7.696 Y36.83
G00 Z0
G01 F60 Z-1
G00 Z2
G00 X17.704
G00 Z0
G01 F60 Z-1
G00 Z2
G00 X27.94 Y46.99
G00 Z0
G01 F60 Z-1
G00 Z2
G00 X33.02 Y49.53
G00 Z0
G01 F60 Z-1
G00 Z2
G00 X35.56
G00 Z0
G01 F60 Z-1
G00 Z2
G00 X27.94 Y57.15
G00 Z0
G01 F60 Z-1
G00 Z2
G00 X48.26 Y59.69
G00 Z0
G01 F60 Z-1
G00 Z2
G00 X58.42
G00 Z0
G01 F60 Z-1
G00 Z2
G00 X68.58
G00 Z0
G01 F60 Z-1
G00 Z2
G00 X78.74
G00 Z0
G01 F60 Z-1
G00 Z2
G00 X87.63
G00 Z0
G01 F60 Z-1
G00 Z2
G00 Y44.45
G00 Z0
G01 F60 Z-1
G00 Z2
G00 X78.74
G00 Z0
G01 F60 Z-1
G00 Z2
G00 X68.58
G00 Z0
G01 F60 Z-1
G00 Z2
G00 X58.42
G00 Z0
G01 F60 Z-1
G00 Z2
G00 X48.26
G00 Z0
G01 F60 Z-1
G00 Z2
G00 X45.72 Y35.56
G00 Z0
G01 F60 Z-1
G00 Z2
G00 X43.18
G00 Z0
G01 F60 Z-1
G00 Z2
G00 X53.34 Y34.29
G00 Z0
G01 F60 Z-1
G00 Z2
G00 X55.88
G00 Z0
G01 F60 Z-1
G00 Z2
G00 X63.5
G00 Z0
G01 F60 Z-1
G00 Z2
G00 X66.04
G00 Z0
G01 F60 Z-1
G00 Z2
G00 X72.39
G00 Z0
G01 F60 Z-1
G00 Z2
G00 X74.93
G00 Z0
G01 F60 Z-1
G00 Z2
G00 X81.28
G00 Z0
G01 F60 Z-1
G00 Z2



G00 X00 Y00


M05
M02
%


```
### Cuttting Code
```
MT65
G54
G0 X0 Y0
G0 Z5
M91

M03 S12000
G4 P5



G00 X1.167 Y0.363
G00 Z0
G01 F60 Z-2
G01 F300 X104.167
G01 Y70.663
G01 X1.167
G01 Y0.363
G00 Z2

G00 X00 Y00

M05
M02
%



```
# Result
Thus the G-Code is converted into Auto leveler Code using Autoleveller software.


