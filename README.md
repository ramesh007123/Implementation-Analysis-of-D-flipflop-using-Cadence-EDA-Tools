## Ex No: 03-Design-and-Implementation-of-D-Flip-Flop-using-Cadence-EDA-Tools

### Aim:
To design and implement a D flip-flop circuit using Cadence EDA tools, analyze its functionality and performance, and understand the principles of digital logic design, including schematic creation, layout design, and simulation.

### Tools Required:
  - Personal Computer
  - Cadence Virtuoso Software

### Circuit Diagram:

![Screenshot (107)](https://github.com/user-attachments/assets/0a0f9ad6-f83d-4fc9-863b-ceeda225ca12)



### SCHEMATIC SIMULATION:
PROCEDURE FOR CREATING THE SCHEMATIC SIMULATION
Commands to get into Cadence:

1. Right-click and open the terminal window.
2. Type the following commands and press enter
    - csh
    - source /cadence/install/cshrc
    - virtuoso
    
Procedure for Schematic simulation using Cadence

1) Now two windows must open
  i)virtuoso/command interpreter window ii)”Whats New…”

2) Close the 2nd window
 
 
3) Use 1st window i.e virtuoso window(CIW) for further processing.
    - Create a New Library
    - Create Schematic Cell view.
    - Create the Symbol for schematic Cell view.
    - Create the test Cell view.
    - Analog simulation by spectre

### Steps for Schematic Simulation using Cadence:
i) Procedure for Creating a New Library:
  - File → New → Library
  - Name the library (e.g., VLSILAB_EXP_3).
  - Choose "Attach to an existing technology library" and click OK.
  - Attach the library to the technology library gpdk045. Click OK.
    
ii) Create Schematic Cell View:
 In the Virtuoso (CIW) window:
  - Go to 1st window i.e virtuoso(CIW)
  - File-New-Cell view
  - Setup the new file form
       + Library: Select the one you a created.
       + Cell : Give the experiment name Ex: Inverter View_Schematic
       + Type: Schematic press OK

   - Add the required components from the libraries and make the connections.
       + Go to instance fixed menu or use shortcut key “I” from keypad to go instances
       + Click on browse. This opens the library browser
       + Now select the appropriate library for components like
       + Gpdk45 ------------------------nmos1v, pmos1v
       + Create Input and Output pins
       + Make the connections by using fixed narrow wire key
       + Click Check and Save button

![Screenshot (108)](https://github.com/user-attachments/assets/f9e257fa-e3ed-484a-9275-7fa6caafde7c)




### iii) Creating the Symbol for Schematic Cell View:

   - In the schematic window, execute
       + Create – Cell view – From Cell view
       + The cell view from cell view window appears
       + Check Lib Name, Cell Name, From View name must be schematic Press ok
   - Now Symbol generation form appears. Click Ok If No changes required
   - A new window with with default symbol is created.
   - Edit the symbol if you want to give actual symbol shape else continue.
   - Execute Create-Cell view-from cell view
   - Library Name and Cell Name must be same which you have used for schematic. Press OK
   - Check for the position of pin side.Prss OK
   - Edit for the shape by Create-Shape-Choose required options to edit.



### iv) Creating the Test Cell View:
- In the CIW window:
  + File → New → Cell view
- In the new file form, set the following:
   + Library: Select the library you created earlier (e.g., VLSILAB_EXP_3).
   + Cell: Name it something different from the schematic cell (e.g., DFlipFlop_test).
   + View: Select "Schematic."
   + Type: Schematic. Press OK.
- Add the required components and make connections, similar to step ii.

![Screenshot (109)](https://github.com/user-attachments/assets/2ed16c46-8a35-4e8c-bd80-c6355db99baf)


### Analog Simulation by SPECTRE:

   - In test cell view window
   - Launch – ADE L(Analog Design Environment)
       + Execute Setup—Simulation/directory/Host A new window opens
       + Set the simulation window to spectre and click ok
       + Execute Analysis – Choose. A window opens.
       + Select the type and set the specifications and press OK
       + Execute Output s—to be plotted – Select on Schematic
       + Then Select the INPUT WIRE(Vin ) and OUTPUT WIRE(Vout) from your test Schematic using mouse
   - Execute Simulation -- Net list and Run


![Screenshot (111)](https://github.com/user-attachments/assets/478c9c52-c4e8-46d2-9d7e-0acdf20b2fd4)


###  For Transient Analysis:
  - In the simulation setup, choose transient analysis.
  - Specify the time range for the analysis (start and stop time).
  - Run the simulation and observe the output waveforms for the D and Q signals.

![Screenshot (110)](https://github.com/user-attachments/assets/80a87d2a-880b-41a3-9480-9c0f944b8ed8)


![Screenshot (115)](https://github.com/user-attachments/assets/0af44ca9-338e-46d1-9e0e-141935d8fcf8)



### Results:
   The experiment successfully demonstrated the design and implementation of a D flip-flop using Cadence EDA tools. The verification through schematic, symbol creation, and simulation highlighted the practical use of Cadence tools for digital circuit design, with the output correctly reflecting the functionality of the D flip-flop.
