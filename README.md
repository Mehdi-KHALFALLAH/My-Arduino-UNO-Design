# My-Arduino-UNO-Design


## Contents and Overview

During this project, I deepened and honed my knowledge about ***Altium Designer*** software and how to do professional PCB design. Altium Designer is a professional software used to design all kinds of boards, from very simple ones to motherboards or servers. It is one of the most used software for electronic design.

I started with Arduino Uno reference schematic. I learned how to re-draw the schematic, modify it, I learned how to improve it and how to do PCB layout. and by the end of the project, I learned what documents are necessary to manufacture the board and how to create them.

during this project, I learned how :

- Draw schematic, including tips for component selection and important circuits
- Create components, draw schematic symbols and footprints
- Place components into your PCB
- Route PCB and useful tips about layout
- Create a 3D model of your board
- Create board variants with different components fitted / not fitted
- Create Bill of Material (BOM)
- Create assembly drawings showing the position of components on the board
- Generate Gerbers, Pick and Place, Drill file, and other files needed for manufacturing
- Prepare professional documents needed to manufacture your PCB and assemble your board



 ## Summary of my project
 
 
 ***I.  [ Creating my own libraries ](#desc)***
 
 ***II. [ Components placement ](#usage)***
 
 ***III.[ Layer's stackup ](#easy)***
 
 ***IV. [ PCB Layout & Routing ](#hard)***

 ***V.   [ Gerber files, mechanical and assembly drawing ](#medium)***


 
 
 
 
 
 
 
 
 <a name="desc"></a>
## I. Creating my own libraries
 
 ### 1 - Designing my first component : the ATMEGA16U2-AU 
 Drawing the schematic and generating the footprint in my own using the Altium tool ***"footprint wizard"***. 
 P.S: footprint's dimensions are taken from the component datasheet :
 
 ![ATMEGA16U2-AU](https://user-images.githubusercontent.com/57021975/92661726-24692000-f2f5-11ea-8991-7cdcb7b960ff.png)
 
 ### 2 - Designing the second component : the ATMEGA328P-PU
 
 ![ATMEGA328P-PU](https://user-images.githubusercontent.com/57021975/92661980-bc670980-f2f5-11ea-92a5-096ae3e0160d.png)
 
 ### 3 - Designing the female header 1 row x 10 positions (pins)
 
 ![Female_Header_10Pins](https://user-images.githubusercontent.com/57021975/92662120-1667cf00-f2f6-11ea-87b2-7bf99a524432.png)
 
 ### 4 - Designing the female header 1 row x 8 positions (pins)
 
![8 Pos  Female SIL Vertical Throughboard Conn](https://user-images.githubusercontent.com/57021975/92662169-30a1ad00-f2f6-11ea-8969-52d0811f1f94.png)

 ### 5 - Designing the female header 1 row x 6 positions (pins)
 
 ![Female_Header_6Pins](https://user-images.githubusercontent.com/57021975/92665022-6ac27d00-f2fd-11ea-84d0-c060f2071f38.png)
 
 ### 5 - Designing the 100nF capacitor 
 
 ![CAP 100n](https://user-images.githubusercontent.com/57021975/92665094-9180b380-f2fd-11ea-8a84-5efb3acf6a13.png)
 
 ### 6 - Sesigning the 10uF capacitor with 1.45mm height 
 
 ![Cap 10uF_145_height](https://user-images.githubusercontent.com/57021975/92665434-7bbfbe00-f2fe-11ea-8cf2-f40354398336.png)

### 7 - Designing the 1M resistor 

![Resistor_1M](https://user-images.githubusercontent.com/57021975/92665502-a14cc780-f2fe-11ea-8b96-807df1f0b440.png)

### 8 - Designing the 16Mhz crystal 

![16MHz Crystal](https://user-images.githubusercontent.com/57021975/92665539-c17c8680-f2fe-11ea-8dcd-902c16fcb6bf.png)

### 9 - Designing the Micro USB 

![micro_USB](https://user-images.githubusercontent.com/57021975/92665588-dce79180-f2fe-11ea-8671-26186b34f492.png)

### 10 - Designing the 100uf aluminum clectrolytic Capacitor

![alu cap 100uf](https://user-images.githubusercontent.com/57021975/92666451-351f9300-f301-11ea-81b8-6ad9407dcfed.JPG)

### 11 - Designing the linear regulator 3.3V 1.5A

![regulator](https://user-images.githubusercontent.com/57021975/92666443-2df88500-f301-11ea-9c78-fe5140acf419.JPG)

### 12 - Designing the AND gate 

![and gate](https://user-images.githubusercontent.com/57021975/92666635-b414cb80-f301-11ea-8a80-b5c3b08bc432.JPG)

### 13 - Designing the Button

![button](https://user-images.githubusercontent.com/57021975/92666733-fdfdb180-f301-11ea-8c00-33ecf95fd691.JPG)

### 14 - Designing the LED 

![LED](https://user-images.githubusercontent.com/57021975/92666853-44eba700-f302-11ea-90f0-32d2db17cc08.JPG)

### 15 - Designing the male header 2 rows x 3 positions (pins)

![header 2w3](https://user-images.githubusercontent.com/57021975/92667023-bc213b00-f302-11ea-872e-2e40ba7b4813.JPG)

### 16 - Designing the male header 2 x 2

![male 2x2](https://user-images.githubusercontent.com/57021975/92667170-1a4e1e00-f303-11ea-8baa-24542abff90d.JPG)

### 17 - Designing the male header 1 x 3

![1x3 header](https://user-images.githubusercontent.com/57021975/92667251-4e294380-f303-11ea-95d3-b316b50907e4.JPG)

### 18 - Successful compilation of the project's schematics

![0 error](https://user-images.githubusercontent.com/57021975/92667338-934d7580-f303-11ea-9e5d-043150f96347.png)

<a name="usage"></a>
## II. Components placement

### 19 - Starting the placement of some components on the board 

![work in progress  more 273 component to place](https://user-images.githubusercontent.com/57021975/92667397-be37c980-f303-11ea-83b2-ca7614c2b175.png)

### 20 - Placement of half of the components
By taking advantage of the altium's features cross probe and components cross selection, i could select components from shematic sheet and at the same time they are selected in the PCB sheet, which make it easier to put couplage capacitors as close as possible to their power pins  

![half way](https://user-images.githubusercontent.com/57021975/92667486-f50ddf80-f303-11ea-9303-20984bad76c0.png)

### 21 - Placement of the components is complete 

![placement complete_blue](https://user-images.githubusercontent.com/57021975/92668707-74e97900-f307-11ea-9460-e5660df64d0a.png)

<a name="easy"></a>
## III. Layer's stackup

### 22 - Layer's stackup in 3D  
standard  dielectric   : 1.6mm 
![layer 3D](https://user-images.githubusercontent.com/57021975/92668801-b8dc7e00-f307-11ea-811b-c9978eb67788.png)

 <a name="hard"></a>
## IV. PCB Layout & Routing

### 23 - Starting to route long tracks

![Starting to route long connections first](https://user-images.githubusercontent.com/57021975/92669131-95660300-f308-11ea-9a18-1bd57fa7b091.png)

### 24 - Routing some long tracks through 2 layers
using vias to go from one layer to onother, I call this the "ping pong" routing

### 25 - Routing 2 tracks through 2 layers (some imporvements are made)

![routing 2 connections through 2 layers ( some imporvements are done )](https://user-images.githubusercontent.com/57021975/92669951-d4955380-f30a-11ea-99b6-3641e7422cf1.png)

### 26 - Finished routing long connections, short connections and Power connections (Power connections are highlighted in the picture)

![Finished routing long connections, short connections and Power connections (Power connections are highlighted in the picture)](https://user-images.githubusercontent.com/57021975/92670013-f4c51280-f30a-11ea-8fd4-0e4bbce37a00.png)

### 27 - Finished routing all the connections on the board and debugging and fixing all violations errors one by one

![Finished routing all the connections on the board and debugging and fixing all violations errors one by one](https://user-images.githubusercontent.com/57021975/92670106-2ccc5580-f30b-11ea-8367-613140a4f88c.png)

### 28 - All rule violations are fixed and the board is validated with 0 errors

![all rule violations are fixed and the board is validated with 0 errors](https://user-images.githubusercontent.com/57021975/92670157-479eca00-f30b-11ea-8f88-c1384f075f81.png)

### 29 - Drawing the power and the ground planes on the bottom layer

![drawing the power and Ground planes on the bottom layer](https://user-images.githubusercontent.com/57021975/92670247-82a0fd80-f30b-11ea-896b-2a51b9d9461f.png)

### 30 - DRC check with 0 errors after improving layout and finishing drawing power and ground planes

![DRC check 0 errors after imroving layout and finishing drawing power and ground planes](https://user-images.githubusercontent.com/57021975/92670349-c3007b80-f30b-11ea-85b9-4c1f7970e453.JPG)

### 31 - PCB layout after doing some improvements and drawing all the power and ground planes

![PCB layout after doing some improvments and drawing power and ground planes](https://user-images.githubusercontent.com/57021975/92670454-f5aa7400-f30b-11ea-896c-44db72fbb968.JPG)

### 32 - Bottom overlay

![bottom overlay](https://user-images.githubusercontent.com/57021975/92670512-1d014100-f30c-11ea-9fe7-972c0cb03011.JPG)

### 33 - Last compile after completing the layout 

![Last compile, last check](https://user-images.githubusercontent.com/57021975/92670631-56d24780-f30c-11ea-9736-3c9740ace571.png)

### 34 - Last design rule check after finishing the layout 

![Last design rule check](https://user-images.githubusercontent.com/57021975/92670690-749fac80-f30c-11ea-8620-7181d859653e.png)

<a name="medium"></a>
## V. Gerber files, mechanical and assembly drawing

### 35 - Gerber top layer

![Gerber Top Layer](https://user-images.githubusercontent.com/57021975/92670800-b0d30d00-f30c-11ea-841f-0421a113adaa.png)

### 36 - Gerber bottom layer

![Gerber bottom Layer](https://user-images.githubusercontent.com/57021975/92670846-cd6f4500-f30c-11ea-93ff-8cf4013e1a63.png)

### 37 - Gerber top overlay

![Gerber Top Overlay](https://user-images.githubusercontent.com/57021975/92670884-e37d0580-f30c-11ea-8bba-ea69fdc6409d.png)

### 38 - Gerber bottom overlay

![Gerber Bottom Overlay](https://user-images.githubusercontent.com/57021975/92671014-2a6afb00-f30d-11ea-9231-3ca2ebfb2397.png)


### 39 - Gerber mechanical drawing

![Gerber Mechanical Drawing](https://user-images.githubusercontent.com/57021975/92670947-03acc480-f30d-11ea-84c6-e9a862b16778.png)

### 40 - Generated PDF mechanical drawing

![Generated PDF Mechanical Drawing ](https://user-images.githubusercontent.com/57021975/92671120-600fe400-f30d-11ea-964a-81f10fc585bc.png)

### 41 - Generated PDF of the assembly drawing variant fixed 5V

![Assembly drawing variant fixed 5](https://user-images.githubusercontent.com/57021975/92671158-7158f080-f30d-11ea-878b-2161d65100cc.png)

### 42 - Generated PDF of the assembly drawing variant 5V 3V3

![Assembly drawing variant  5V 3V3](https://user-images.githubusercontent.com/57021975/92671239-9fd6cb80-f30d-11ea-896f-b3450791e749.png)

### 43 - Generated PDF of the assembly top view fixed 5V 

![Assembly top view 5V fixed](https://user-images.githubusercontent.com/57021975/92671289-c137b780-f30d-11ea-9140-18665d05e26f.png)

### 44 - Generated PDF of the assembly top view 5V 3V3

![Assembly top view 5V 3V3](https://user-images.githubusercontent.com/57021975/92671326-e0364980-f30d-11ea-8c63-f5ce82028583.png)

### 45 - 3D model of my board in Altium Designer

![3D Model in Altium](https://user-images.githubusercontent.com/57021975/92671407-18d62300-f30e-11ea-965f-991f84229cb6.JPG)

### 46 - Current density analysis using ANSYS SIwave 

using the advanced simulation software especially designed for PCBs, i could do a current density analysis and generate an easy-to-understand plot

![Current-Voltage analysis using SIwave from Ansys](https://user-images.githubusercontent.com/57021975/93142734-84d5d400-f6de-11ea-880f-57311c3e02d4.JPG)

### 47 -  High current density

showing high current density coming from OUT pin of the regulator to the ATMEGA16U2-AU

![showing high current density coming from OUT pin of the regulator to the atmega](https://user-images.githubusercontent.com/57021975/93143022-075e9380-f6df-11ea-9412-75072203bc75.JPG)

### 48 - Far end crosstalk analysis between traces

![far end crosstalk between traces](https://user-images.githubusercontent.com/57021975/93143084-21987180-f6df-11ea-8abb-03cdea69de1c.JPG)

### 49 - Near end crosstalk violations and warnings

![near end crosstalk violations and warnings](https://user-images.githubusercontent.com/57021975/93143132-3aa12280-f6df-11ea-8124-ffef3fbfb923.JPG)

### 50 - Trace impedance analysis

trace impedance analysis, some improvements and fixes must be done

![trace inpedance analisys, some imporvlements and fices must be done](https://user-images.githubusercontent.com/57021975/93143217-67553a00-f6df-11ea-98ee-ee542cd3ff3f.JPG)

### 60 - Resonance analysis

![resonance analysis with ansys](https://user-images.githubusercontent.com/57021975/93143413-ce72ee80-f6df-11ea-9410-d647f9bc23cf.JPG)

### 61 - Failure analysis, simulating MTTF(Mean time to Failure)

![Failure analysis , simulating MTTF(Mean time to Failure)](https://user-images.githubusercontent.com/57021975/93143475-f3676180-f6df-11ea-8c13-a3154dd8135d.JPG)

### 62 - MTTF plot

![MTTF plot, board is good to go](https://user-images.githubusercontent.com/57021975/93143522-09752200-f6e0-11ea-82dc-be8a67375fa6.JPG)






