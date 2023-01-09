# Test

# Intel-CKT-Training-git-Repo

## Table Of Content 
 
+ **[Day 1 - Day 1 Fundamentals of VLSI Design and overview of Sand-to-Silicon](https://github.com/amirulalfaris/Intel-CKT-Training-git-Repo#day-1)**
  <details><summary> Theory </summary>
  
   [Theory - Fundamentals of VLSI Design and overview of Sand-to-Silicon](https://github.com/amirulalfaris/Intel-CKT-Training-git-Repo#theory---fundamentals-of-vlsi-design-and-overview-of-sand-to-silicon)
   </details>
   <details><summary> Lab </summary>
   
   [Lab - Setup Labs](https://github.com/amirulalfaris/Intel-CKT-Training-git-Repo#lab---setup-labs)
   </details>
   
   + **[Day 2 - Analog VLSI Design Flow and CMOS Fabrication Process](link)**

  <details><summary> Theory </summary>
 [Analog VLSI Design Flow and CMOS Fabrication Process](link)
 
 </details>

## Day 1
## Theory - Fundamentals of VLSI Design and overview of Sand-to-Silicon

<details><summary> Overwiew of VLSI Design </summary>

### **Overview**
From system aprroach ( Ex. Motherboard ) --> Chip to Wafer (Ex Central of the chip called die (where all the fabricated components are inside)) --> Inside the die which containts all the components (Memory (RAM) ,Memory controller , Analog and RF(PLL,LDO,VCO .etc), Digital (decoder, register, fsm .etc ) seperate into each partition . 

![motherboard](https://user-images.githubusercontent.com/121993910/210926862-bf94c5c2-8f1f-47e7-b3f0-7225b1c5525d.png)

![Chip](https://user-images.githubusercontent.com/121993910/210927257-c5732d1f-3704-4009-8404-da69344cdff5.png)

<img width="499" alt="image" src="https://user-images.githubusercontent.com/121993910/210927824-b5e2c25f-4944-4010-a5ad-8bc93320051c.png">

</details>

<details><summary> History of VLSI Design </summary>

###  History of VLSI Design 

From the evolution of single transistor --> Very Large Scale Integration (> 20,000 transistor ) --> System on Chip (SOC -Multiple IP ) --> System in Package (SiP - Heterogeneous Integration )

* **Moore's Law** - Number of trasistor in an integated Chip (IC) will doubles about every two years. Size will be reduce to $1/sqrt{2}$

</details>

<details><summary> VLSI Design Methodology  </summary>

### VLSI Design Style 

* **FPGA** - Field Proramming Gate Array Design 
* **ASIC (application-specific integrated circuit)** - Standard cell base Design & Full custom Design 

 * **Standard Cell Base Design** -  standard cell library component are used to make the design .
     Ex.  half adder to make full adder
 
 * **Full Custom Design** - Designers intend to design their  own design itself ( Ex. orientation and placement of trasistor in layout design ) 
 
**FPGA VS ASIC **

| | FGPA | ASIC | 
|---| ----| ---|
| Time to Manufacture |Faster time to market - no layout , masks and manufacturing steps needed | Need longer design times to take care of all manufacturing steps |
|Reusability |Field programmability - Design Changes can be absorbed even in filed and FPGA reprogrammed | Once manufactured, need to spin again a new chips in case of bugs |
|Power/Performance | More power consumption and less performance because of programmable design and low clock speed | Custom design for an application helps in designing for power/performance efficiencies | 
|Production | Good for prototyping and low volume designs, as cost would be less | For larger volume of production , cost per unit is much less for an ASIC | 
|Analog and Mixed Signal | Not Possible | Supported | 
 
 </details>

<details><summary> Package Technology  </summary>
 
 ### Package Technology
 
 Package is where the die chip is being hold . This package is very important because failure can happen if the packaging is not being done properly 
 Ex . factor that affect package Length of bonding wire,lead length of the package,number of ground and power and the bonding pads . 
 


<img width="568" alt="image" src="https://user-images.githubusercontent.com/121993910/210962083-1d15852b-8314-4345-bb9d-9f1afd6fc52a.png">

</details>

### Lab - Setup Labs 

<details><summary> steps to enable labs </summary>
 
 [Set Up labs](https://docs.google.com/document/d/1_Qb8Xi2J0ZACvAwTW9h1-bFJzuUHAwnI/edit)

</details>


 ## Day 2
## Theory - Analog VLSI Design Flow and CMOS Fabrication Process

<details><summary> Analog VLSI Design Flow </summary> 
 
###  *Analog IC Design Process*
 
 The overview of the analog IC design Process can be seperated into 4 parts which is 
 + Electrical Design
 + Physical Design
 + Fabrication 
 + Testing and product Developement or Test Design 
 
 ![image](https://user-images.githubusercontent.com/121993910/211248780-f30b3cd2-e2b2-4db8-905e-5ecf18487aee.png)
*Diagram above shows how each part is contributing to the Analog IC design Process .*
 
 | Electrical Design | Physical Design  | Test Design | 
|---| ----| ---|
 | Electrical design is the process of going from the specification to a circuit solution | Physical design is the process of representing the electrical design in a layout consisting blocks at various levels | Test design is the process of coordinating , planning and implementing the measurement of the analog integrated circuit performance |
 | Required active and passive device models for <ul><li>Creating the design</li><li>Verying the design</li><li>Determining the robustness of the design</li></ul>| Requires <ul><li>Entering various geometries</li><li>Check DRC </li><li>Check LVS</li><li>Extract Parasitic</li></ul> | Type of test <ul><li>Functional</li><li>Parametric</li><li>Static</li><li>Dynamic</li><ul>| 
 
 *Analog IC Design Process Defination*
 
 **Relationship Between Design Process with CAD and PDK**
 In each Analog IC Design process ,Computer Aided Design(CAD) and Process Design Kit(PDK) play a role important to complete such process .
 + CAD - Much like a software that helps in creation , modification , analaysis of a design . Ex. Magic , Spice 2 , Mentor graphics
 + Process Design Kit - Set of files or library to a model a farbrication process generated by the foundary . The purpose of it is to defined a certain technology varitation for the process. 
 
 </details>

  <details><summary> CMOS Fabrication Process </summary> 
   
  ###**Overview** 
   
   *Circuit Designer need to have deeper understanding of CMOS manufacturing process and the role as a circuit designer itself due to*  
   + Physical implementation has a major impact on performance, power and cost.
   + Not rely based on the ideal circuit , instead base on practical circuit that have many limitations and constraint .
   + So that less iterations of the design can be implemented .
   + A good designer always discussed with each other for better understanding and efficiencies . 
   
   Why Cmos Technology is widely used ? 
   ![image](https://user-images.githubusercontent.com/121993910/211256980-95c4ddf3-4ff5-402e-b17f-1eb34d87f599.png)

   Cmos Technology 
   + Submircron Technlogy (DSM) > 0.35um
   + Deep Submicron Technology (UDSM) : 0.1um < Lmin < 0.35um 
   + Ultra-Deep Submicron Technology Lmin < 0.1min
   + BiCMOS Technology Lmin = 0.5um 
                                                  
   Submicron an object which is smaller than a micron < 0.5um . 
   
 **CMOS Fabrication Process .**
   
  ![image](https://user-images.githubusercontent.com/121993910/211259811-f6787da3-005f-423b-bf5a-1d8b9338ecf1.png)

  **1.Wafer Formation** 
   
<img width="205" alt="image" src="https://user-images.githubusercontent.com/121993910/211259878-77ecb7ba-47ea-4a32-82f1-cca90eed0a5a.png">

   + Pure silicon is melted on a very high degreem temperature . 
   + A small seed containing the desired cyrstal is inserted into the molten silicon and slowly pull out . 
   
   ![image](https://user-images.githubusercontent.com/121993910/211262375-2c88ba43-a768-4408-b625-3d326ccbe44b.png)

   + The silicon being pulled will be manufactured or form as cylidrical ingot . 
   + This cylindrical ingot will be slice into disc or wafers . 
   + The wafer is cut (diced) into many pieces, each containing one copy of the circuit. Each of these pieces is called a die.
   
   **2.Photolithography**
   
 + Photolitography is a technique used to pattering silicon wafer  and to protect it desired areas during echting, deposition or ion implantation . 
 + A layer of sensitive checmical called the photoresist is coated on the substrade will be selectively illuminate by the UV light through the photomask . 
 + A photomask is a mask that is constructed with chromium to prevent light to go through during the process . The gap or part that is not covered by the chromium will let the UV light pass through causing the photoresist dissolve and the desired shapep that we desired is implemented .
 + Ething of the layer is done afterwards to formed the pattern desired . 
   
![image](https://user-images.githubusercontent.com/121993910/211268935-e6c404c5-86bd-4547-b780-e778591b2118.png)

 [Reference taken from Wiki Page](https://en.wikipedia.org/wiki/Photolithography) 
 
 ### **Overview**
From system aprroach ( Ex. Motherboard ) --> Chip to Wafer (Ex Central of the chip called die (where all the fabricated components are inside)) --> Inside the die which containts all the components (Memory (RAM) ,Memory controller , Analog and RF(PLL,LDO,VCO .etc), Digital (decoder, register, fsm .etc ) seperate into each partition . 

![motherboard](https://user-images.githubusercontent.com/121993910/210926862-bf94c5c2-8f1f-47e7-b3f0-7225b1c5525d.png)

![Chip](https://user-images.githubusercontent.com/121993910/210927257-c5732d1f-3704-4009-8404-da69344cdff5.png)

<img width="499" alt="image" src="https://user-images.githubusercontent.com/121993910/210927824-b5e2c25f-4944-4010-a5ad-8bc93320051c.png">

</details>  
