VLSI-LAB-EXP-6
SIMULATE AND SYNTHESIS INVERTER USING CADENCE

AIM:
To create,simulate the design of CMOS inverter,NAND,NOR from schematic using cadence.

APPARATUS REQUIRED:
cadence

PROCEDURE:

Commands to get into Cadence
Right Click and open the terminal window Type the following commands as follows and press enter. i) tcsh ii) source /home/install/cshrc iii) virtuoso

Procedure for Schematic simulation using Cadence
Now two windows must open i)virtuoso/command interpreter window ii)”Whats New…” Close the 2nd window Use 1st window i.e virtuoso window(CIW) for further processing. i) Create a New Library ii) Create Schematic Cell view. iii) Create the Symbol for schematic Cell view. iv) Create the test Cell view. v) Analog simulation by spectre

Procedure for Creating New Library.
a) File –New – Library b) Name : Give name for ur library Ex: VLSILAB , Enable Attach to an existing technology library, Click OK c) Attach the library to the technology library gpdk045.Click OK

Create Schematic Cell view.
a) Go to 1st window i.e virtuoso(CIW) b) File-New-Cell view c) Setup the new file form, Library: Select the one you a created. Cell : Give the experiment name Ex: Inverter View: Schematic d) Type: Schematic press OK e) Add the required components from the libraries and make the connections. f) Go to instance fixed menu or use shortcut key “I” from keypad to go instances Click on browse. This opens the library browser ow select the appropriate library for components like Gpdk045,nmos, pmos g) Analog library Vdd, Gnd, Vcc, Vpulse, Vsin h) Make the connections by using fixed narrow wire key i) Click Check and Save button

Creating the Symbol for schematic Cell view
a. In the schematic window, execute Crate – Cell view – From Cell view The cell view from cell view window appears Check Lib Name, Cell Name, From View name must be schematic Press ok b. Now Symbol generation form appears. Click Ok If No changes required c. A new window with with default symbol is created. d. Edit the symbol if you want to give actual symbol shape else continue. i. Execute Create-Cell view-from cell view ii. Library Name and Cell Name must be same which you have used for schematic. Press OK iii. Check for the position of pin side.Prss OK iv. Edit for the shape by Create-Shape-Choose required options to edit.

Creating the new test cell view
a) Go to CIW window, Execute File-New-Cell view b) Setup the new file form Library: Select the one you a created. Cell: Cell name must be different from the name used in schematic cell view. Ex: Inverter_test View: Schematic Type: Schematic press OK

Analog simulation by SPECTRE.
a. In test cell view window i. Launch – ADE L(Analog Design Environment) b. Execute Setup—Simulation/directory/Host A new window opens c. Set the simulation window to spectre and click ok d. Execute Setup-Model Library. Anew window opens, Check of gpdk.scs as lib and section type as stat then press OK. e. Execute Analysis – Choose. A window opens. f. Select the type and set the specifications and press OK g. Execute Output s—to be plotted – Select on Schematic h. Then Select the INPUT WIRE(Vin ) and OUTPUT WIRE(Vout) from your test Schematic using mouse i. Execute Simulation -- Net list and Run

INVERTER SCHEMATIC:
![331263006-71c59b42-02d9-4620-a614-03dd6bbf0110](https://github.com/alwaysajay3011/VLSI-LAB-EXP-6/assets/161150132/ffe6e607-2766-4060-99c1-35c03abac730)
![331263074-06653b3c-1d35-4d20-97ed-68ff1f21abec](https://github.com/alwaysajay3011/VLSI-LAB-EXP-6/assets/161150132/0866b0fc-4a4c-476f-98d1-5dc1f7c9ae8a)

Specifications: Vpulse

V1 = 0

V2 = 1

td = 0,tr=tf=1 n, ton= 100n ,T=200n

Vdc = 1 Simulation Settings

Setup for transient analysis:

Stop time =400n

Setup for D.C analysis

Component to be selected in schematic is for d.c analysis

Start = -1 Stop = 1 resp. Expected Waveform:

Transient Analysis: 
![331263217-862395ba-441d-4a39-a65d-28a24c31e3c9](https://github.com/alwaysajay3011/VLSI-LAB-EXP-6/assets/161150132/3d429ac6-36e4-4834-aa28-7923f92a29bb)

DC Analysis:
![331263390-a19cd120-3c56-4fb5-a2fd-c155078ae3b0](https://github.com/alwaysajay3011/VLSI-LAB-EXP-6/assets/161150132/9543d919-92d2-4ee0-add7-a45618a84bb3)

NAND SCHEMATIC : 
![331263612-d1e2feaf-4932-41b2-a2f9-16897f0ada26](https://github.com/alwaysajay3011/VLSI-LAB-EXP-6/assets/161150132/0a8046b5-f78c-4f73-b46d-d5b80fa4923b)
![331263666-4661e9d8-0b26-4d65-a5ba-eb68e67c2f96](https://github.com/alwaysajay3011/VLSI-LAB-EXP-6/assets/161150132/a891e197-66dd-496b-bdeb-b10922401158)

Specifications:

Vpulse

Va1 = 0 Va2 = 1 tr=tf=50ps, period=20ns pulse width = 10ns

Vb1 = 0 Vb2 = 1 tr=tf=50ps, period=40ns pulse width = 20ns

Vdc = 1

Expected Waveform:

Transient Analysis:
![331263807-743b07f1-fa64-4f45-8102-8f4d96737158](https://github.com/alwaysajay3011/VLSI-LAB-EXP-6/assets/161150132/727b43c8-e5dc-49db-96ad-6586a85b60a8)

NOR SCHEMATIC:
![331263993-b0e0affe-678e-4768-be36-aff4b111b9b7](https://github.com/alwaysajay3011/VLSI-LAB-EXP-6/assets/161150132/7443bbdb-9aca-4bd9-a811-81621271bd02)
![331264102-f76153d6-d3ad-424d-ae17-62c2db653cb6](https://github.com/alwaysajay3011/VLSI-LAB-EXP-6/assets/161150132/20b5274a-b89f-489e-a542-396b0e3f2cae)

Specifications:

Vpulse

Va1 = 0 Va2 = 1 tr=tf=50ps, period=20ns pulse width = 10ns

Vb1 = 0 Vb2 = 1 tr=tf=50ps, period=40ns pulse width = 20ns

Vdc = 1

Expected Waveform:

Transient Analysis:
![331264316-6936f930-0188-4409-886f-a0200a7a258a](https://github.com/alwaysajay3011/VLSI-LAB-EXP-6/assets/161150132/23cc7006-18cb-43cc-91bf-59749b03c1c5)

RESULT:

Thus, the design,simulation and verification of the CMOS inverter,NAND,NOR from schematic using cadence was successfully completed.
