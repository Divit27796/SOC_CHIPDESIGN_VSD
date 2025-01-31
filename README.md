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

    
  


  












































