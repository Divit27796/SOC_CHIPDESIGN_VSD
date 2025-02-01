# SOC_CHIPDESIGN_VSD
<details>
  <summary>
Expand or Collapse
  </summary>
  
## THEORY 

<details>
  <summary>
Expand or Collapse
  </summary>

### HOW TO TALK TO COMPUTERS

<details>
  <summary>
Expand or Collapse
  </summary>
  
![Image](https://github.com/user-attachments/assets/4f6c1547-0ad2-4fd7-9570-c7fd44b81e17)

### Chipset
- A computer's Chipset is an integrated circuit that takes care of the communication between the CPU, RAM, storage, and other peripherals. The chipset determines how many high-speed components or USB devices your motherboard can support. Chipsets are usually comprised of one to four chips and feature controllers for commonly used peripherals, like the keyboard, mouse or monitor.

![Image](https://github.com/user-attachments/assets/e1d057e1-dc14-4d33-9088-65e79ed6c1b7)

### Processor/SoC.
- A SoC, or System-on-a-Chip, integrates almost all of these components (chipset features) into a single silicon chip. Along with a processor, the SoC usually contains a GPU (graphics processor), memory, USB controller, power management circuits, and wireless radios. 

### DIE: 
- A die, in the context of integrated circuits, is a small block of semiconducting material on which a given functional circuit is fabricated. 

### PADS: 
- Pad refers to the place where (surface mount) pins are soldered to. The pad is a copper or what-have-you surface that gives the pin somewhere to connect to. Every pin is 
soldered to its pad on the board.

![Image](https://github.com/user-attachments/assets/f77baccb-fa25-4864-a2d0-525249d3389d)

![Image](https://github.com/user-attachments/assets/a9dd9aef-f703-4d03-bc02-52e8a42da6d4)

### INTRODUCTION TO RISC-V SoC
- An open-source instruction set architecture used to develop custom processors for a variety of applications.

### Foundry IP’s (Intellectual Process)
- Foundries are companies that manufacture semiconductor products as a service.

![Image](https://github.com/user-attachments/assets/1ad5e1b6-1198-40f8-8703-3fcab5f63d68)

### RISC-V Instruction Set Architecture (ISA)
- An open-source instruction set architecture (ISA) that provides a foundation for processor design. It is based on the principles of reduced instruction set computing (RISC) and offers a modular and extensible ISA that can be customized for specific applications and use cases.

![Image](https://github.com/user-attachments/assets/0c2aaad6-d8b1-4931-a68e-4b70a365d610)

### Software Application to Hardware

![Image](https://github.com/user-attachments/assets/d3a384ca-3fec-4948-933f-41e7b306bdf0)

### SOC DESIGN AND OPENLANE
### RTL: 
- Register-transfer-level (RTL) design is an essential step in the design process of digital circuits. It defines and optimizes the logical functionality of a digital design at an abstract level before specifying the circuit's physical layout.

### EDA:	
- Electronic Design Automation (EDA) is a specific category of hardware, software, services and processes that use computer-aided design to develop complex electronic systems like printed circuit boards, integrated circuits and microprocessors. It check out the different parts, and try to figure out what's happening in the data.

### PDK:	
- A process design kit (PDK) is a set of files used within the semiconductor industry to model a fabrication process for the design tools used to design an integrated circuit. The PDK is created by the foundry defining a certain technology variation for their processes.

![Image](https://github.com/user-attachments/assets/c719b65d-c8ce-4955-b5e8-a6d49f002948)

### RTL2GDSII flow:
- This complete flow is also known as RTL to GDS (RTL2GDS) flow. This is followed by the Fabrication or Manufacturing Process where designs are transferred onto silicon dies which are then packaged into ICs.

![Image](https://github.com/user-attachments/assets/8184f38c-21e9-4825-b32b-5ddb093a7934)

### Synthesis:
- Convert RTL to a circuit out of component cell library (SCL)
Synthesis is one of the important steps in chip designing flow as it allows us to visualize the design as it will appear after manufacturing. Here, designers review all reports and validate all required factors including timing, area, and power.

![Image](https://github.com/user-attachments/assets/e51f5080-a6c3-4689-816c-6a1207cda2f4)


 
  </details>
  
### Floor Planning/ Power Planning

  <details>
  <summary>
Expand or Collapse
  </summary>

### Floor planning:
- It involves determining the locations, shape and size of modules in a chip and as such it estimates the chip area, delay and the wiring congestion, thereby providing a ground work for layout. 

![Image](https://github.com/user-attachments/assets/53e23340-1d6c-4620-9eb6-b1cefc767f49)

### Power planning:
- It is stage typically part of the floor planning stage, in which power grid network is created to distribute the power uniformly to each part of the chip. Power planning means to provide power to the every macros and standard cells and all others cells are present in the design.

![Image](https://github.com/user-attachments/assets/449b3ff4-915d-459e-bbfb-e1c04d7489ed)

### Placement:
- It is an important step of digital hardware design where components such as logic gates (standard cells), or large collections of components (macros) have to be placed on a 2-dimensional physical chip based on a connectivity graph (netlist) of the components.

![Image](https://github.com/user-attachments/assets/9dddcc49-5751-4a7f-aa7e-652fa2d75c7e)

### Clock Tree Synthesis (CTS):
- It is one of the most important stages in PnR. CTS QoR decides timing convergence & power. In most of the ICs clock consumes 30-40 % of total power. So efficient clock architecture, clock gating & clock tree implementation helps to reduce power.

![Image](https://github.com/user-attachments/assets/938c389f-8f8b-4a7d-b4a3-d6f43a1820d0)

### Routing:
- It is the stage after Clock Tree Synthesis and optimization where- Exact paths for the interconnection of standard cells and macros and I/O pins are determined. Electrical connections using metals and vias are created in the layout, defined by the logical connections present in the netlist.

![Image](https://github.com/user-attachments/assets/a8491f8d-ed18-4cc5-8793-36d746fab607)

### Signoff:
- This is the final step before the design is sent to manufacturing. Here, all of the critical parameters that will impact the performance or manufacturability of the chip are verified.

### (a)	Physical Verifications:

  (i)	Design Rules Checking (DRC)
  
  (ii)	Layout vs Schematic (LVS)
    
### (b)	Timing Verification:

  (i)	Static Timing Analysis (STA)

   </details>
  
### INTRODUCTION TO OPENLANE & STRIVE CHIPSET

  <details>
  <summary>
Expand or Collapse
  </summary>

- OpenLane is an innovative silicon implementation platform that supports open-source tools such as Yosys, OpenROAD, Magic, KLayout, along with other open-source and proprietary utilities.

![Image](https://github.com/user-attachments/assets/2d7b9323-fb2b-4748-8894-f902fcd64a94)

![Image](https://github.com/user-attachments/assets/1fc44260-f2b7-453a-a3d3-cd2acb8f7a6a)

### MACRO HARDENING FLOW:
- Hardening a design is the process of taking it from Hardware Description Language (HDL) model to the various views of the manufactural mask layouts. A hardened design (a soft macro) is usually then instantiated within another encompassing design. There are usually two purposes behind hardening a macro before using it in the context of a bigger design.

![Image](https://github.com/user-attachments/assets/96444ade-75e5-4d78-877d-6776d65883c3)

 </details>
  
### GOOD FLOORPLAN VS BAD FLOORPLAN 

  <details>
  <summary>
Expand or Collapse
  </summary>

### CHIP FLOOR PLANNING CONSIDERATION:

### Utilization Factor and Aspect Ratio:
- Width & Height of Core and Die

### Floor planning:
- Floor planning is the art of any physical design. A well and perfect floorplan leads to an ASIC design with higher performance and optimum area.
- It deals with the placement of I/O pads and macros as well as power and ground structure.
- Before we are going for the floor planning to make sure that inputs are used for floorplan is prepared properly.

### Inputs for floorplan:
1.	Netlist (.v)
2.	Technology file (techlef)
3.	Timing Library files (.lib)
4.	Physical library (.lef)
5.	Synopsys design constraints (.sdc)
6.	Tlu+

   ![Image](https://github.com/user-attachments/assets/e3e4d999-92d8-47b0-b3ca-ac7883bf29fd)

### Floorplan control parameter core area depends upon: 
### Aspect ratio:
- Aspect ratio will decide the size and shape of the chip. It is the ratio 	between horizontal routing resources to vertical routing resources (or) ratio of height and width. 

- Aspect ratio = width/height

![Image](https://github.com/user-attachments/assets/79b21f38-a118-4074-a180-7c8471b56ee9)

### Core utilization:
- Utilization will define the area occupied by the standard cells, macros, and other cells. If core utilization is 0.8 (80%) that means 80% of the core area is used for placing the standard cells, macros, and other cells, and the remaining 20% is used for routing purposes.
- Core utilization = (macros area + std cell area +pads area)/ total core area

### Location of Pre placed Cell:

![Image](https://github.com/user-attachments/assets/a651a4b3-4e96-44e4-a6ba-ca13fe46f6e2)

![Image](https://github.com/user-attachments/assets/90de745d-379e-4aea-9cce-328c2939e748)

- There are other IP’s also available
- The arrangement of these IP’s in a chip is referred as Floor planning.
- These IP’s/blocks have user-defined locations, and hence are placed in chip before automated placement and routing and are called as pre-placed cells.
- Automated placement and routing tools places the remaining logical cells in the design onto chip.

![Image](https://github.com/user-attachments/assets/1d4a064c-7626-4040-850c-675974b2d908)

### De-coupling capacitors:
- A decoupling capacitor is a capacitor used to decouple (i.e. prevent electrical energy from transferring to) one part of a circuit from another.

  ![Image](https://github.com/user-attachments/assets/508a85bb-4a4c-450d-b02d-fa3e7f9d6b7f)

  ![Image](https://github.com/user-attachments/assets/a1844775-8942-45ac-a05e-c4bfd27c5164)

### Power planning:
- Power planning means to provide power to the every macros, standard cells, and all other cells are present in the design. Power and Ground nets are usually laid out on the metal layers. In this create power and ground structure for both IO pads and core logic.

![Image](https://github.com/user-attachments/assets/48248512-0051-4df5-b756-21eebf531b40)

### Delivers Power Evenly:
- Every transistor receives the necessary voltage for consistent performance across the chip.

 ### Minimizes Voltage Drops:
 Power planning ensures sufficient voltage reaches all parts of the chip by minimizing resistance in the power delivery network.

 ### Avoid Electro migration: 
- we choose higher metal layers with less resistance to supply power to the block because they have lesser resistance and chances of Electro migration is lesser in higher metal layers, so during power planning width of the metal layer is decided based on EM limit.

 ### Prevents Overheating:
 - By controlling current flow, power planning reduces the risk of metal wires weakening due to excessive current.

 ![Image](https://github.com/user-attachments/assets/348bcca5-fa16-4c9b-b63e-3b30780ad156)

![Image](https://github.com/user-attachments/assets/f7b1d344-b0d0-4cb3-8e74-dc5472db365a)

 ### Pin placement and logical cell placement blockage:
 - Pin placement is an important step in the floor plan, which can be optimized based on pin placement requirements. The pin placement can be done based on timing, congestion, and utilization of the chip. Pin placement in macros utilizes M3 layers most of the time, so the macro needs to be placed logically. library binding and palcement

![Image](https://github.com/user-attachments/assets/e0317c19-7db1-4e6f-ab7b-0483081a5694)

![Image](https://github.com/user-attachments/assets/94f2c5fc-7179-424c-9f22-91b4fe5dedc0)


  
  </details>
  
### Library and Binding Placement

  <details>
  <summary>
Expand or Collapse
  </summary>
  
### Netlist binding and initial place design:
- Netlist binding is the process of mapping the logical representation of a digital design onto standard cell shapes from a library. Each component in the netlist is mapped to a specific shape defined in the library.
  
 ![Image](https://github.com/user-attachments/assets/aaa0d645-e3ef-4de9-9de8-530d0e93cbbd)

![Image](https://github.com/user-attachments/assets/c78244d8-767c-47da-b46d-00b9b7f1b7df)

### Placement:
- It is an essential step in electronic design automation the portion of the physical design flow that assigns exact locations for various circuit components within the chip's core area. An inferior placement assignment will not only affect the chip's performance but might also make it non-manufacturable by producing excessive wire-length, which is beyond available routing resources. A placer takes a given synthesized circuit netlist together with a technology library and produces a valid placement layout. The layout is optimized according to the aforementioned objectives and ready for cell resizing and buffering a step essential for timing and signal integrity satisfaction.

![Image](https://github.com/user-attachments/assets/c98b159a-c1b4-434a-9659-8865e6dbe065)

### Optimize Placement:
- It involves assigning exact locations to circuit components within a chip's core area. The goals of placement are to minimize the total interconnect length and costs while meeting timing requirements.

![Image](https://github.com/user-attachments/assets/7852effa-6c40-4a4e-80f0-d80f0a29b004)

### Library Characterization and modelling:
- Cell library characterization is a process of analzing a circuit using static and dynamic methods to generate models suitable for chip implementation flows.
- Part-I: Concepts and Theory – NLDM, CCS timing, and power and noise characterization.
- Logic Synthesis   -->       Floor Planning    -->     Placement   -->       CTS   -->      Routing

  ![Image](https://github.com/user-attachments/assets/a3b0ca45-1a70-444c-b184-83749307133e)

### Static Timing Analysis:
- Static timing analysis (STA) is a method of validating the timing performance of a design by checking all possible paths for timing violations.

![Image](https://github.com/user-attachments/assets/6a868906-05d9-4b75-b1fb-d45dede92a65)

 </details>
  
### CELL DESIGN AND CHARACTERIZATION FLOWS
  <details>
  <summary>
Expand or Collapse
  </summary>
### Cell Design Flow:
- These stages include system specifications, architectural design, functional design, logic design, circuit design, physical design verification, and manufacturing.

![Image](https://github.com/user-attachments/assets/0d26360f-2d23-4491-a347-65d977f119ca)

![Image](https://github.com/user-attachments/assets/3b8a056d-d863-4832-870a-d4120be11402)

### Time Characterisation:

![Image](https://github.com/user-attachments/assets/9b9e5551-89dc-4333-8d62-e0e0de4591f3)

### Propagation Delay:

![Image](https://github.com/user-attachments/assets/2660d398-2205-44c0-aaf0-1f8481aad16a)

</details>
 </details>
 

  
  
  
## GETTING FAMILIAR TO OPENSOURCE EDA TOOLS
<details>
  <summary>
Expand or Collapse
  </summary>
  </summary>

### RUNNING OPENLANE IN INTERACTIVE MODE:
<details>
<summary>
Expand or Collapse
  </summary>

### The code which will be used to open the intreactive mode of openlane is as:
    # Change directory to openlane directory
     vsduser@vsdsquadron:~$ cd Desktop
     vsduser@vsdsquadron:~/Desktop$ cd /work/tools
     vsduser@vsdsquadron:~Desktop/work/tools$ cd openlane_working_dir
    vsduser@vsdsquadron:~Desktop/work/tools/openlane_working_dir$ cd openlane
    vsduser@vsdsquadron:~Desktop/work/tools/openlane_working_dir/openlane$
    # run command docker
    vsduser@vsdsquadron:~Desktop/work/tools/openlane_working_dir/openlane$ docker
    bash-4.2$
    #give command to run in interactive mode
    bash-4.2$ ./flow.tcl -interactive
    # program starts running in interactive mode
    
![Image](https://github.com/user-attachments/assets/4efbb4ab-1638-46e5-89e1-4a6bc1331a52)


</details>

### Commands to Run Synthesis In Openlane:
<details>
<summary>
Expand or Collapse
  </summary>

 ### Command to run synthesis as:
 - but first we have to do preperation
 - For it the code is as:

       # In openlane interactive mode we will write these commands
         % package require openlane 0.9
         0.9
         # Now the OpenLANE flow is ready to run any design.
         # Initially we have to prep the design creating some necessary files and directories for running the 'picorv32a'
         % prep -design picorv32a 

  - After writing the command it will show us this screen:

    ![Image](https://github.com/user-attachments/assets/b3371617-3eb0-4e71-82a1-ac92cd59b46f)

 - Now we write the code written below to run synthesis
      
        % run_synthesis
        # Synthesis starts
 - It will show the below screen when we write this command

   ![Image](https://github.com/user-attachments/assets/53a09232-9072-4844-80ce-db2c62561eea)

   ![Image](https://github.com/user-attachments/assets/7c3b96d7-fa43-412d-b41e-56935fe623f0)

   </details>

### Section 1 Task
<details>
<summary>
Expand or Collapse
  </summary>

### Find The Flop Ratio
- It is the number of 'd' flipflops divided by the number of cells

  ![Image](https://github.com/user-attachments/assets/1f0a678a-7087-4c49-aeef-78637ee938fd)
  
- You can see here the synthesis statistic report in which the 'd' flipflop are 1613 and the number of cells are 18036
- So, Flop ratio = 1613/18036 = 0.0894322466
- In percentage it is 0.0894322466 * 100 = 8.94322466
- Here, flop ratio is 8.94322466
  


</details>

### RUNNING FLOORPLAN IN OPENLANE 
<details>
<summary>
Expand or Collapse
  </summary>

### Commands to run floorplan are as follows:

    # Change directory to openlane flow directory
    cd Desktop/work/tools/openlane_working_dir/openlane
    # Run the docker command
    docker


     # Now that we have entered the OpenLANE flow contained docker sub-system we can invoke the OpenLANE flow in the Interactive mode using the following command
     ./flow.tcl -interactive

     # Now that OpenLANE flow is open we have to input the required packages for proper functionality of the OpenLANE flow
     package require openlane 0.9

     # Now the OpenLANE flow is ready to run any design and initially we have to prep the design creating some necessary files and directories for running a specific design 
     which in our case is 'picorv32a'
     prep -design picorv32a

     # Now that the design is prepped and ready, we can run synthesis using following command
     run_synthesis

     # Now we can run floorplan
    run_floorplan

 
![Image](https://github.com/user-attachments/assets/5287506e-52fa-470e-b053-775ee18c2878)

![Image](https://github.com/user-attachments/assets/7a744cba-cfd2-40a4-ae8f-2a7faee94bae)


### Floorplan.def in MAGIC :-

### The code to open floorplan.def in magic is as follows:

    # Change directory to path containing generated floorplan def
    cd Desktop/work/tools/openlane_working_dir/openlane/designs/picorv32a/runs/28-01_13-06/results/floorplan/

    # Command to load the floorplan def in magic tool
    magic -T /home/vsduser/Desktop/work/tools/openlane_working_dir/pdks/sky130A/libs.tech/magic/sky130A.tech lef read ../../tmp/merged.lef def read picorv32a.floorplan.def &

![Image](https://github.com/user-attachments/assets/db0958ea-362f-4fde-a564-15b832afab1a)

### After you write the code this screen will appear

  ![Image](https://github.com/user-attachments/assets/56090529-3093-43db-be61-9e7267652a29)

 ###  Equidistant placement of pins:

 ![Image](https://github.com/user-attachments/assets/0dbc3076-fcd0-4a39-abd5-b114fa6ecd6c)


</details>

### Finding dimension of the chip in micrometer
<details>
<summary>
Expand or Collapse
  </summary>
  

![Image](https://github.com/user-attachments/assets/6234777e-d912-4b42-ada4-228026be37e7)


- As you see in die area there are two 0
- First Zero is lower left x value
- second Zero is lower left y value

- The number 660685 is the upper right x value
- The number 671405 is the upper right y value

- Units distance microns is the database unit per micron that is 1 micron equals to 1000 database units

- If you divide these numbers by 1000 it will give you the dimensions of the chip in micrometer.

- So, dimensions = upper right x value/1000
- Same as here dimensions =  upper right y value/1000

- Which equals to 660685/1000
  = 660.685 micrometer

- Same as here which equals to 671405/1000
  = 671.405 micrometer


</details>

### Running placement in openlane
<details>
<summary>
Expand or Collapse
  </summary>

  
    # After floor planning, the next step is placement. run the following command
    % run_placement
    # The placement process starts

 ![Image](https://github.com/user-attachments/assets/ce7a5f54-7c37-41f4-b36d-20e8491247a0)
 

- After the placement is complete it will show the following screen:
  

  ![Image](https://github.com/user-attachments/assets/6e1c5607-b022-4df5-948f-76951b2018bc)

  
</details>

### Steps to git clone
<details>
<summary>
Expand or Collapse
  </summary>
  
### The code is as follows:

     # Change directory to openlane
    cd Desktop/work/tools/openlane_working_dir/openlane

    # Clone the repository with custom inverter design
    git clone https://github.com/nickson-jose/vsdstdcelldesign

    # Change into repository directory
    cd vsdstdcelldesign

    # Copy magic tech file to the repo directory for easy access
    cp /home/vsduser/Desktop/work/tools/openlane_working_dir/pdks/sky130A/libs.tech/magic/sky130A.tech .

    # Check contents whether everything is present
    ls

    # Command to open custom inverter layout in magic
    magic -T sky130A.tech sky130_inv.mag &
  


![Image](https://github.com/user-attachments/assets/b749efa7-4aa2-45dc-93a4-d268fb450420)

</details>

### Identification for pmos and nmos
<details>
<summary>
Expand or Collapse
  </summary>

  ### Nmos:

  ![Image](https://github.com/user-attachments/assets/db2b40f5-4934-4d5e-8a2f-fc3b03b59641)

  ![Image](https://github.com/user-attachments/assets/b4e3ed6f-2731-4ca0-990d-ff24b65c058b)


   ### Pmos:

   ![Image](https://github.com/user-attachments/assets/e4316d32-a79b-41ff-8164-db2ceeb8e881)

![Image](https://github.com/user-attachments/assets/942af933-c337-46d7-a6cd-009010de779f)



</details>

### Steps to extract spice netlist
<details>
<summary>
Expand or Collapse
  </summary>

### the code is as follows

![Image](https://github.com/user-attachments/assets/b062c450-2e60-455a-8d2c-f6c2e7b99511)

![Image](https://github.com/user-attachments/assets/7eef710e-b27c-4b16-8699-96fea5209489)



































