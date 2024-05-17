# VLSI-LAB-EXP-6
# AIM:
To design and simulate the CMOS inverter and observe the DC and transient responses using cadence tool.

# APPARATUS REQUIRED:
1.Laptop with MobaXterm

2.Cadence tool PROCEDURE SCHEMATIC ENTRY: Creating a new library:

3.In the library manager, execute File - New library. The new library form appears.

4.In the new library form, type ‘my design lib’ in the name section.

5.In the field of directory section, verify that the path to the library is set to ~/Database / Cadence- analog – lab –bl3 and click ok.

6.In the next ‘technology file for new library form select option attach to an existing tech file and click ok.

7.In the ‘attach design library to technology file’ form, select gpdk045 form the cyclic field and click ok.

8.After creating a new library you can verify it from the library manager.

9.If you right click on the ‘my design lib’ and select properties, you will find that gpdk045 library is attached as techlib to ‘my design lib’.

# Creating a schematic cell view:
1.In the CIW or library manager, execute file – new – cell viw.

2.Setup the new file form as follows, Do not edit the library path file and the above might be different from the path shown in your form.

3.Click ok when done the above setting. A black schematic window for the inverter design appears.

# Adding components to schematic:
1.In the inverter schematic window, click the instance fixed menu icon to display the add instance form.

2.Click on the browse button. This opens up a library browser from which you can select components and the symbol view.

3.After you complete the add instance form move your cursor to the schematic window and click left to place a component. LIBRARY NAME CELL NAME gpdk045 PMOS gpdk045 NMOS

4.This is a table of components for building the inverter schematic.

5.After entering components, click cancel in the add instance form or press ESC with your cursor in the schematic window.
![EXP-6](https://github.com/navaneethans/VLSI-LAB-EXP-6/assets/165630121/01cd14eb-f3f7-4641-bcd3-d85bd013c1cd)
# Adding pins to schematic:
1.Click the pin fixed menu icon in the schematic window. You can execute create pin or press ‘p’.

2.Add pin form appears. Type the following in the ADD pin form in the next order leaving space between the pin. PIN NAMES DIRECTION Vin,Vdd,Vss Input Vout Output

3.Select cancel and then the schematic window enter window file or press the f bind key. Adding wires to schematic:

4.Click the wire (narrow) icon in the schematic window.

5.In the schematic window click on a pin of one of your components as the first point for your wiring. A diamond shape appears over the starting point of this wire.

6.Follow the prompts at the bottom of design window and click left on the destination point for your wire. A wire is routed between the source and destination points.

7.Complete the wiring as shown in the figure and when done wiring press ECS key in the schematic window to cancel wiring.

# Saving the design:
Click the check and save icon in the schematic editor window observe CIW output for any errors.

# BUILDING THE INVERTER TEST DESIGN: Creating the inverter test cell view:
1.In the CIW or library manager, execute file – new – cell view.

2.Setup the newfile as shown below.

3.Click ok when done. A blank schematic window for the inverter test design appears.

4.Using the components list and properties/ comments in this table build the inverter test schematic. LIBRARY NAME CELL VIEW NAME PROPERTIES/COMMENTS My design lib Inverter Symbol Analog lib Vpulse Voltage1 = 0, Voltage2 = 1.8, delay Time = 0, Rise time=Fall time=1ns Period=20ns Analog lib Vdc, gnd Vdc = 1.8v

5.Add the above components using create – instance or by pressing I.

6.Click the wire (narrow) icon and wire your schematic.

7.Click create wire name or press c to name the i/p (vsin) and output wires as in below schematic.

8.Click on the check and save icon to save the design.
![EXP-6(2)](https://github.com/navaneethans/VLSI-LAB-EXP-6/assets/165630121/0ca7aa13-cc86-4a18-ac26-115e5b5137e2)
# ANALOG SIMULATION WITH SPECTRA: Starting the simulation environment:
1.In the Inverter-test schematic window execute launch – ADEL. The variable virtuoso analog design environment (ADE) simulation window appears. Choosing a simulator:

2.In the simulation window (ADE) execute setup – simulator / directory / host.

3.In the choosing simulator form, set the simulator field to specra and click ok.

4.In the simulation window (ADE) execute the setup model libraries. To complete, move the cursor and click ok. Choosing Analysis:

5.Click the choose- Analysis icon in the simulation window (ADE).

6.The choosing analysis form appears.

7.To Setup the transient analysis. a. In the analysis section select tron. b. Set the stop time as 100ns c. Click at the moderate or enabled button and the bottom and then click apply.

8.To set for DC analysis a. In the analysis section select DC. b. Turn on save DC operating point. c. Turn on the component parameters. d. Double click the select Vpulse source or Type V0 (capital V zero). e. Select the DC voltage in the select window parameter and click in the form start and stop voltages are 0 to 1.8. f. Select the enable button and click apply and then click ok.

Selecting output for plotting:

1.Execute the o/p’s to be plotted -select on sschematic in the simulation window.

2.Follow the prompt at the bottom. Click on the o/p net vout input vin of the inverter. Press esc with the cursor after selecting.

# Running the simulation:
1.Execute the simulation Netlist and run in the simulation window to start the simulation on the icon. This will create the netlist as well as run the simulation.

2.When the simulation finishes the transient and DC plots automatically will be popped up along with netlist.
![EXP-6(3)](https://github.com/navaneethans/VLSI-LAB-EXP-6/assets/165630121/68325e51-4039-4115-894c-d52428b00f11)
![EXP-6(4)](https://github.com/navaneethans/VLSI-LAB-EXP-6/assets/165630121/93161b63-3174-4a02-92df-a11b78c4596c)
# CMOS NAND GATE
# NAND SCHEMATIC
![EXP-6(5)](https://github.com/navaneethans/VLSI-LAB-EXP-6/assets/165630121/e4255e1b-2ef2-40c7-863f-e9881cad9469)
# NAND TEST CELL VIEW
![EXP-6(6)](https://github.com/navaneethans/VLSI-LAB-EXP-6/assets/165630121/fa8615ac-44ce-4c41-a5da-c3ecae000e07)
# NAND SIMULATION WITH SPECTRA
![EXP-6(7)](https://github.com/navaneethans/VLSI-LAB-EXP-6/assets/165630121/66d2950a-ef90-4554-ab23-3501db735e14)
# CMOS NOR GATE
# NOR SCHEMATIC
![EXP-6(8)](https://github.com/navaneethans/VLSI-LAB-EXP-6/assets/165630121/83672965-ca7e-4dc1-a4c5-2507f8944af6)
# NOR TEST CELL VIEW
![EXP-6(9)](https://github.com/navaneethans/VLSI-LAB-EXP-6/assets/165630121/fe4e8484-ad0f-4cdd-aad3-2610002d9686)
# NOR SIMULATION WITH SPECTRA
![EXP-6(10)](https://github.com/navaneethans/VLSI-LAB-EXP-6/assets/165630121/925eb813-2461-47d3-9595-2d33196b6110)

# RESULT:
THe design and simulation of the CMOS inverter and the DC and transient responses using cadence tool is successfully observed and verified.






