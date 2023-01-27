# Intel-CKT-Training-git-Repo

## Table Of Content 
 
+ **[Day 1 - Day 1 Fundamentals of VLSI Design and overview of Sand-to-Silicon](https://github.com/amirulalfaris/Intel-CKT-Training-git-Repo#day-1)**
  <details><summary> Theory </summary>
  
   [Theory - Fundamentals of VLSI Design and overview of Sand-to-Silicon](https://github.com/amirulalfaris/Intel-CKT-Training-git-Repo#theory---fundamentals-of-vlsi-design-and-overview-of-sand-to-silicon)
   </details>
   <details><summary> Lab </summary>
   
    [Lab - Assignemnt](https://docs.google.com/presentation/d/1Cm7hb_-vpqZq_iwY7fwXAXaH0rOmg-2f/edit?usp=share_link&ouid=110064100622421144823&rtpof=true&sd=true)
   </details>
   
+ **[Day 2 - Analog VLSI Design Flow and CMOS Fabrication Process](https://github.com/amirulalfaris/Intel-CKT-Training-git-Repo#day-2)**
  <details><summary> Theory </summary>
  
   [Analog VLSI Design Flow and CMOS Fabrication Process](https://github.com/amirulalfaris/Intel-CKT-Training-git-Repo#theory---analog-vlsi-design-flow-and-cmos-fabrication-process)
     </details>
     <details><summary> Assignment </summary>
     
     [Assignment day 2](https://docs.google.com/document/d/1LUZd35zsOoNcMLgwo44L24rsoK-OZ_hb/edit?usp=share_link&ouid=110064100622421144823&rtpof=true&sd=true)
     </details> 
     
 + **[Day 3 - CMOS Fabrication Process in Deep-Submicron (DSM) and Ultra Deep- Submicron (UDSM) Technology](https://github.com/amirulalfaris/Intel-CKT-Training-git-Repo#day-3)**
    <details><summary> Theory </summary>
    
      [CMOS Fabrication Process in Deep-Submicron (DSM) and Ultra Deep- Submicron (UDSM) Technology}](https://github.com/amirulalfaris/Intel-CKT-Training-git-Repo#day-3)
      </details>
      <details><summary> Lab </summary>
    
     [Assignment day 3 ](https://docs.google.com/document/d/1KS7-OqJR2pCQjEW9CEIrYuPPZZmWkFAo/edit?usp=sharing&ouid=110064100622421144823&rtpof=true&sd=true)
     </details>     

 + **[Day 4 - Metal Oxide Semiconductor Structure](https://github.com/amirulalfaris/Intel-CKT-Training-git-Repo#day-4)**
    <details><summary> Theory </summary>
    
      [Metal Oxide Semiconductor](https://github.com/amirulalfaris/Intel-CKT-Training-git-Repo#theory---metal-oxide-semiconductor-mos-structure-)
      </details>
      <details><summary> Assignment </summary>
    
     [Assignment day 4 ](https://docs.google.com/document/d/1jf-B_N2NGeg1E98xbfFroVlpucC3Mob8/edit?usp=sharing&ouid=110064100622421144823&rtpof=true&sd=true)
     </details>     

+ **[Day 5 - Metal Oxide Semiconductor Field Effect Transistor](https://github.com/amirulalfaris/Intel-CKT-Training-git-Repo#day-5)**
    <details><summary> Theory </summary>
 
    [Metal Oxide Semiconductor Field Effect Transistor](https://github.com/amirulalfaris/Intel-CKT-Training-git-Repo#theory---metal-oxide-semiconductor-field-effect-transistormosfet-)
      </details>
      
     
+ **[Day 6 - MOSFET Intrinsic Capacitance](https://github.com/amirulalfaris/Intel-CKT-Training-git-Repo#day-6)**
     <details><summary> Theory </summary>
    
     [MOSFET Intrincsic Capacitance](https://github.com/amirulalfaris/Intel-CKT-Training-git-Repo#theory---mosfet-intrinsic-capacitance--)
        </details>
       
     <details><summary> Assignment </summary>
    
     [Assignment day 6 ]()
     </details>  

+ **[Day 7 - CMOS Inverter]()**
     <details><summary> Theory </summary>
    
     [MOSFET Inverter]()
        </details>
       
     <details><summary> Assignment </summary>
    
     [Assignment day 7 ]()
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
   
  **3.Well and Channel Formation**
   
  <img width="570" alt="image" src="https://user-images.githubusercontent.com/121993910/211452116-8f012552-2ae0-4c23-b338-6e64dccb493f.png">

   + **N-well / P-well Process** is where the n-type diffusion is done to a p-type subtrade or p-type diffusion is done on a n-type substrate respectively .
   + **The twin well process** is where NMOS and PMOS transitor are developed over the wafer by simulataneous diffusion over an epitaxial growth base rather than a substrate . This will allow the optimization of each transistor type . 
   + **Triple well process** NMOS formed by n+ on p-well, which sits inside a n-well, which further sits on the substrate. PMOS formed by p+ on n-well, which sits on the substrate. This allow a good isolation between analog and digital blocks in mixed signal chips and also to isolate high density dynamic memory from logic .
   
 **4.Silicon Dioxide** (SiO2) 
   
   + The purpose of this process is to create a silicon dioxide layer on top of the silicon surface . Can be done using : 
   
   |Wet Oxidation | Dry Oxidation |
   |---|---|
   |900-1000 Degree Celcius | In the region of 1200 Degree Celcius | 
   |Rapid Process | Form a better quality oxide |
   |Form a thick field layer oxide | Form a thin oxide , highly controlled gate oxide |
   
   + **Atomic Layer Deposition (ALD )** - Another method to deposite the silicon dioxide on top of the subtrate or surface . Think layer of Chemical A is introduce to a surface and chemical B is introduce afterwards to produce a thin layer of the required layer . 
   
   **5.Isolation** 
   
   + solation between two adjacent transistors in CMOS circuits is necessary to isolate n channel and p channel transistors in order to avoid the undesirable parasitic currents between the transistors.
   + Example process of isolation is Local Oxidation of Silicon(LOCOS) or Shallow Trench Isolation (STI)
   + STI is introdued due to some problem with LOCOS process which is the transition between thick and thin layer oxide require some extended so called bird beak .
   
  **6.Gate Oxide**
   
   + One of the common process to form the gate oxide in the transitor .
   + The gate oxide is a layer that seperate the gate termincal of Mosfet from the source and drain terminal as well the conductive channel that connect source and drain when the MOSFET is turned on . 
   
   **7.Gate and Source/Drain Formations**
   
+ Grow gate oxide wherever transistors are required (area = source + drain + gate)––elsewhere there will be thick oxide or trench isolation.
+ Deposit polysilicon on chip
+ Pattern polysilicon (both gates and interconnect)
+ Etch exposed gate oxide—i.e., the area of gate oxide where transistors are required that was not covered by polysilicon; at this stage, the chip has windows down to the well or substrate wherever a source/drain diffusion is required
+ Implant pMOS and nMOS source/drain regions through iom bombartment . 
   
   <img width="641" alt="image" src="https://user-images.githubusercontent.com/121993910/211474135-0a73b5ee-cdda-4aa4-ab92-5d1d589a8fdf.png">
   
   **8.Contact and Metallization**
   
   + Connections must be made to link the circuits together . This is how the metallization process comes into . So called the interconnects

   <img width="322" alt="image" src="https://user-images.githubusercontent.com/121993910/211474607-c86d1553-b633-43d7-94af-fe755ecd3086.png">
   
   *Metal Deposition is done to link all the trasnsitor together to form a circuit .*
   
   + Other important application of metallization is the top-level metal that provides a connection to the outside world. To reduce interconnection resistance and save area on a chip, multilevel metallization.
   + Metallization is also used to produce rectifying (Schottky barrier) contacts, guard rings, and diffusion barriers between reacting metallic films.
   + [Reference link for metallization ](https://www.circuitstoday.com/metallization-process)

   
   **9.Passivation**
   
   + After metellization process passivation is done afterwards, passivation is a process of where we add the protective glass layer to prevents the ingress of contaminants or to protect the internal semiconductor devices.
   + The overglass cuts which is the opening in the passivation layer is required to allow the connection of the I/O pads and test the probe points . 
   
   **10.Metrology**
   
   + Metrology is basically more to quality assurace methods by calibrate and measure the resulting parts in the procduction process .
   
   </details>
   
  </details>
 
 ## Day 3
## Theory - CMOS Fabrication Process in Deep-Submicron (DSM) and Ultra Deep-Submicron (UDSM) Technology 
<details><summary> Introduction to DSM </summary>

### **Overview**

+ As transistor size is getting smaller and smaller , more challanges is introduced  towards fabricating the cmos such as **Hot carrier injection**, **Punch Through Effect**, more noise and many more .This cause the submicron process is not realiable anymore and the Deep-Submicron process is introduced . 
 
+ One disadvatange of the submicron process is during the isolation process , as the transistor getting smaller , the used of reverse bias pn junctions for isolation  becomes impractical .
 
 <img width="454" alt="image" src="https://user-images.githubusercontent.com/121993910/211742121-70977f3e-188a-4db7-8ad8-5b4e4bb303d5.png">

 
+ LOCOS techniqued is used in the isolation process . The limitation of this technique is due to the bird beak effect which extend some distance literally on the transition of the thick and thin oxide . The surface area also is lost due to this enroachment .
 
+ The great things about LOCOS is it **takes a simple process flow**, **High oxide quality procduced** 
 
 <img width="251" alt="image" src="https://user-images.githubusercontent.com/121993910/211741488-56ac5923-5e25-44c9-9e95-b922b475e7dc.png">

 *LOCOS process step *

+ Due to the limitation from the LOCOS , Sallow Trench Isolation (STI) Technology is introduced. 
+ STI allows the closer spacing of transistor which eliminate the depletion region at the surface and the bird's beak effect .
+ STI process able to grow a think layer of oxide compare to LOCOS which create the bird's beak shape .'
+ Due to allowing a smaller isolation region, STI is suitable to be used on increase density in a small area .
+ But STI require more step process needed  and the oxide quality is not good compared to LOCOS . 

  <img width="493" alt="image" src="https://user-images.githubusercontent.com/121993910/211743541-bea7b9f2-28f2-4412-8a07-16bbed734c52.png">
  
*How STI able to solve LOCOS problem by allowing closer spacing transistor*
 
 <img width="238" alt="image" src="https://user-images.githubusercontent.com/121993910/211745178-b58e5f9e-7576-4161-b22b-5dbae49c6c13.png">

 *Illustration step by step of STI Process* 
 
 
</details>
 
<details><summary> Deep SubMircron CMOS Technology </summary>
 
 Due to the addition of NMOS and PMOS transitor , DSM provides : 
 
 + A deep n-well that can be used to lower down the substrade noise coupling . 
 + A MOS varactor , that can be utilized as voltage controlled oscillators .
 + Different type of resistor : 
   + Diffused and/or implanted resitor - Diffused resistors are resistors that are fabricated through p-type diffusion into an n-type background and the surface geometry such as the length, width and the diffused impurity profile determine the resistance value . Sheet resistance is the parameter to defining this resistance . 
   + Well resitors - The surface geometry such as the length, width and the diffused impurity profile determine the resistance value . Will give a very high resistance value .
   + Poly Resistor - widely used as an important device in CMOS analog circuit design . Would give a small amout of resitance .
   + Metal Resistor - due to the interconnection of metal . Typicaly has a very small among of resitance by still we can do it as resistor . The thicker the thickness of the metal the lesser the resistance will be . Metal thickness increases as the metal number increase . Ex . metal 1 will be less thicker compared to metal 6. 
 
  <img width="684" alt="image" src="https://user-images.githubusercontent.com/121993910/211750585-826981f0-684e-4788-aa4b-567928015f63.png">
 
 + Metals that can be used as inductors, capacitors and transmission line . 
 
 <img width="384" alt="image" src="https://user-images.githubusercontent.com/121993910/211754638-ec3f2194-127d-484e-9409-a225c03a650b.png">
 
 *Capacitor formed through poly-poly layer and metal instulator metal.* 
 + Capacitance formed is affected by the distance . The longer the distance less capacitance will be generated  .
 + The area also would affect the capactiance . 

Thin oxide  and there is a poly it will become a transistor. 
Thick oxide and there is a poly it will become a resistor. 

</details>
 
 <details><summary> Typical Deep Submicron CMOS Technology </summary>
  
 Steps for a DSM CMOS process . 
  **1.** p and n wells formation .
  **2.** Shallow trench isolation - Need isolation between nmos and pmos . Used STI instead of LOCOS 
  **3.** Threshold shift and anti punch through implant - doping/implantation that will alter the threshold voltage ( to avoid the punchthrough effect )
  **4.** Thin oxide and gate polysilicon - typicaly putting the gate oxide 
  **5.** Lightly doped drains and sources. - To avoid bad adjacent between the drain and source ( to reduce the depletion region )
  **6.** Sidewall spacer . ( Introduced in DSM to avoid unnesarry extension of source and drain ) 
  **7.** Heavily doped drains and sources 
  **8.** Siliciding ( Salicide and Polycide) - To increase the conductitivy between drain and source by achieving a good ohmic contact . 
  **9.** Bottom metal, tungsten plugs, and oxide - bottom metal = metal 1 , tungsten plug = tungsten contact  
  **10.** Higher level metals, tungsten plugs/vias, and oxide - metal 2,3 
  **11.** Top level metal, vias and protective oxide.

 
   **Starting Material.** 
 + Substrade is highly doped to get a good conductor . 
 
  **1. p and n wells formation.**
  <img width="606" alt="image" src="https://user-images.githubusercontent.com/121993910/211956519-f36b01fe-bb92-4876-b9bf-5f46dfa54197.png">
 
  + photolithography is done as usual to pattern the substrate . 
  + p-well implanct and  Diffusion and n-well implant and Diffusion is done to create the p well and n well respectively. 
  + Diffusion - process of adding impurities atoms from a region with high concentration to a region of low concentration. The dopants or impurity atoms are added to the silicon (semiconductor material), which changes its resistivity. The process of diffusion is highly dependent on the temperature.
  + Implantation - Heavy electric field is used to plan the atom/material . a process of adding dopant to the silicon substrate to enable the conductivity .
  
  **2. Shallow Trench Isolation**
 
  + Electrically isolates one region or transitor from another which prevents electric current leakage between adjacent semiconductor device components .
  
  <img width="583" alt="image" src="https://user-images.githubusercontent.com/121993910/211957232-b99fe089-d678-4cb2-a470-edc49c53f0c8.png">
  
  **3. Threshold shift and anti punch through implant**
 
  <img width="825" alt="image" src="https://user-images.githubusercontent.com/121993910/211958853-8bdd8259-9312-407b-958b-83f93b709f3f.png">
  
  + P thershold implant is used balance to the threshold voltage or control the threshold voltage . 
  + implantation also is used to create a highly doped region to avoid the punch through effect . By doing this the depletion region will become more smaller . 
  + Punch through effect is where the depletion region of the source terminal and the depletion region on the drain terminal is meet with each other .
  
  **4. Thin Oxide and Polysilicon Gate**
  
  <img width="591" alt="image" src="https://user-images.githubusercontent.com/121993910/211959978-41c9f5fd-cda0-4777-8c9f-3d94a3520d34.png">

  Same type of process in submicron .
  
  **5. Lightly DOpen Source and Drain**
  
  + Not being done in the submicron process .
  + Lightly dope is being done to control the deplettion region (less), Kinetic energy / Electric field (less) and to avoid the impact ionization .
  + Impact Ionization is where the hot electron impact the drain causing dislodging holes , these holes are swept towards negatively charged substrate causing a current flowing in the subtrate. 
  
  <img width="300" alt="image" src="https://user-images.githubusercontent.com/121993910/211962978-b006a732-d553-424a-a0c5-6866381a0180.png">
  
  **6. Sidewall spacer **
  
  <img width="600" alt="image" src="https://user-images.githubusercontent.com/121993910/211963731-97fdd5a7-67c9-42df-99d6-f82abef6877f.png">

  + typically is a Silicon Nitrade .
  + Prevent the drain and source next to the channel from becoming a heavily doped . 
  
  **7. Implantation of Heavily doped source and drain**
  
  <img width="585" alt="image" src="https://user-images.githubusercontent.com/121993910/211963901-a9680fc0-0bcc-4226-9d33-b50378cf6fb0.png">

  + at the spacer side we can see the heavily doped part is not extending towards the drain  and source near the channel thats helps to reducing the overlap capacitance and impact ionization . 
  + This also helps to able to get a good ohmic contact . 
  
  **8.Siliciding ( Salicide and Polyside) **
  
<img width="591" alt="image" src="https://user-images.githubusercontent.com/121993910/211965246-933e0c72-8030-49de-94af-83d23f9184e2.png">
  
   + To create a good ohmic contact between the contact-drain and contact-source . 
   + polyside helps to reduce the resistance of the poly 
   + Added or used in the Deep submicron process but no in the submicron . 
  
  **9. Intermediate Oxide Layer**
  
  <img width="591" alt="image" src="https://user-images.githubusercontent.com/121993910/211965300-70ce54bd-ccf7-4f1c-82b2-29b5f87f0f95.png"
       
   + Next step will be more on the back end process which where the connection from the drain and source towards the metal/outside . 
   + Oxide layer is used to cover the transitor and to planarize the surface .
   + A hole on the oxide will be done for contact purposes to the outside .
   
   **10 . First level metal**
   
   <img width="584" alt="image" src="https://user-images.githubusercontent.com/121993910/211969916-42405cf8-2553-4339-a88a-c9ec5e9c9305.png">

   + Through via of tungsten contact to connect the device,well and subtrade to the first metal layer . 
   + The tungsten oxide film produced by the target sputtering deposition method has the advantages of high density, good adhesion, and good corrosion resistance, so it is suitable for use in semiconductor chips. Has a good thermal characteristic .
   
   **11. Second Level metal **

  <img width="609" alt="image" src="https://user-images.githubusercontent.com/121993910/211971147-278b6cc3-f5ed-48b3-af0b-052b95374e3d.png"> 
  <img width="463" alt="image" src="https://user-images.githubusercontent.com/121993910/211971406-594db2cc-9694-4d8e-a939-d5a848aea47a.png">

  + The step 10 is repeated until the top metal layer . 
  + The top metal layer usually is thicker than the first or second metal layer due to the amount of current it need to bring . Usually is related to the power routing or transmission line purposes. The top metal layer also can be used as capacitor or inductor formation .
  + The proctective insulator layer act as a passivation to protect the top metal connection to outside  .
  
  **Summary**
  
  + Able to adress the excessive depletion region in junction isolation . 
  + metal levels is more when getting into the ultra deep submicron technology or getting into deeper technology .
  + Lightly doped helps to avoid impact ionization , junction capacitance hence improving analog performance . 
  
  
    
 </details>
 
 <details><summary> Ultra Deep (UDSM) CMOS technology </summary>
 
 **USDM Technology**
 
 + Lmin < 0.1 Microncs.
 + Minimum feature size less than 100 nanometers.
 + Specialized processing is used to increase drive capability and maintain low off currrents 
 
 
 <img width="462" alt="image" src="https://user-images.githubusercontent.com/121993910/211990892-44925d3d-a9bb-4648-a3ae-76734a71a762.png">

 + More level of metals - analog circuit are very sensitive , therefore by adding more levels of metals helps to reduce the interference between the top level metal and low level metal. 
 + Higher capacitance density - Can create more capacitance as more level of metals is introduced. 
 + More speed - use lower length/size of transitor to achive speed by doing a custom design in analog part . 
 
 
   </details>
 
   
</details>
 
  ## Day 4
## Theory - Metal Oxide Semiconductor (MOS) Structure . 

<details><summary> MOS structure </summary>

**MOS STRUCTURE**

+ Typically MOS structure is build base on the name itself which is Metal Oxide Semiconductor (MOS) . Which is the oxide layer will be sandwiched by metal at the top and semiconductor layer on bottom . 
+ Normally the metal itself is the high-conductivity polycrystalline silicon that has been deposited on the oxide . That's is the reason why we call metal due to its conductivity properties such as metal . 
+ Since the oxide is between two conductive layer . We can imagine the structure of a  MOS as capacitor itself . 
+ Due to this we have a C-V Characteristic of a MOS . 
+ Capacitance of metal to metal (MOM) structure is basically is constant - Co
+ For MOS , the capacitance will varied with respect to voltage change . 
+ The capacitance also is affected by the frequency . The relationship is inversely propotional to each other .
+ The flat-band voltage is defined as the applied gate voltage such that there is no band bending in the semiconductor  , as a result, zero net space charge in this region .
+ Due to fermi level of metal and semiconductor and is not balance during zero applied gate bias voltage

<img width="597" alt="image" src="https://user-images.githubusercontent.com/121993910/212260386-b8c0dfd1-bf53-4384-9a9d-fd42447613c9.png">

*Cmos structure , C-V Characteristic and relationship between capacitance and frequency.*

<img width="604" alt="image" src="https://user-images.githubusercontent.com/121993910/212264557-0d57e105-2bdd-45ad-b2fb-426bb1bcacf6.png">

+ Interface between the semiconductor and oxide is happen in non ideal case . where there is a trap charge in this interfaace . 
+ This is due to the fabrication chemical reaction or imperfection . 


</details>
 
<details><summary> Ideal MOS Junction or Capacitor </summary>

<img width="601" alt="image" src="https://user-images.githubusercontent.com/121993910/212271155-0df05cd7-b8b1-4c5a-bfed-dbf5ec1650c3.png">

*Parameters when ideal case of MOS is used*

+ In Ideal case we neglect all the parameters shown in the picture . The focus on ideal case will be on how it operate during these gate bias (**V<0** , **0<V<VT**, **V >VT**).

**1.Case 1 (V<0)**

![image](https://user-images.githubusercontent.com/121993910/212444928-e826fbf9-a3d9-482b-95e7-c2d50bd785e4.png)

+In this case v < 0 means we applied a reverse gate voltage .
+ This cause the neagtively charge to exist  in the metal plate whereas the positively charge exist in the semiconductor plate .
+ Because of these charges , an Electric field is induced bwtween this two plate causing the majority carrier in the substrate which is hole ( in this case we assume that the subtrate is P-subtrate )  experience a force toward the oxide– semiconductor interface .
+ This causes the accumulation of holes at the interface . 
 
**2.Case 2 (0<V<Vt)**

<img width="460" alt="image" src="https://user-images.githubusercontent.com/121993910/212447302-25d27d92-dda2-4f3a-a468-1bcbdea9cb68.png">

+ As we applied a positive bias ,  The metal plate will become positively charge where as the semiconductor plate will be more likely to be negatively chrage . 
+ The induced electric field will push or force away the majority caarrier which is hole from the interface .
+ This will induced the space charge region which mainly consist of negatively charge ion due to fact that p substrate is a acceptor atoms .
+ At a certain voltage point where the surface carrier concentration is the same as the bulk carrier concentration is called the weak inversion voltage or threshold voltage . This is the point where the inversion point started . Where p-type becoming more like a n type semiconductor . 
+ Inversion here means that since the substrate is a p type subtrate . The majority carrier is hold . But applying the positive bias gate voltage cause the holes at the subtrate is being filled with electrons and becomes negatively charge . This cause the carrier concentration of the bulk which is hole at the p-substrate is becoming less compared to the induced space charge region as it being filled with electrons . therefoe only near the interface of the oxide-semiconductor , the p-type inverted to the n-type . 
+ Energy band diagram with respect to positive gate voltage is shown below.
 
 
 <img width="243" alt="image" src="https://user-images.githubusercontent.com/121993910/212445628-10d5fb83-86d6-471e-b3db-75a497603db3.png">
 
 * The conduction band bend towards the fermi level due to the negatively charge ion is near the interface **
 
 **3.Case 3 (0 = and > Vt)**
 
 <img width="517" alt="image" src="https://user-images.githubusercontent.com/121993910/212445732-d839e2c3-169b-4209-967a-c3c390e91a39.png">
 
 + A channel is form at the threshold voltage . 
 + If we apply a large positive gate voltage , basically what will happen that the induced space charge region will become much larger/bigger in magnitude means more negatively charge .
 + The surface in the semiconductor adjacent to the oxide–semiconductor interface is becoming more n type . Inversion occurs .
 + This leads to more band bending . 

 <img width="282" alt="image" src="https://user-images.githubusercontent.com/121993910/212446546-a6b847ea-944a-44c5-937a-3a7cb8d65d54.png">
 
+ The conduction band close to the Fermi level, whereas the valence band is close to the Fermi level in the bulk semiconductor . 
+ Meaning at the oxide-semiconductor interface inversion happen form p type to n-type.

    </details>
 </details>   
 
 <details><summary> Q-V and C-V characteristic of MOS </summary>
 
 **Q-V**
 
 <img width="670" alt="image" src="https://user-images.githubusercontent.com/121993910/212448092-54280ab0-b18b-4f2c-94c6-6fe0d7d0de02.png">
 
 *Q-V characteristic*
 
 + Qcc = positive due to the accumulation of holes during reverse bias voltage .
 + 0V and onwards = negatively charge due to the induce space region witch consist of the negatively charge .
 + Qi = increase linearly after the Vt due to the mobile electron .
 + Threshold voltage is the summation of the potential acrros the oxide and voltage drop at the semiconductor circuit. 
 
 ** C-V Characteristic ** 

<img width="703" alt="image" src="https://user-images.githubusercontent.com/121993910/212448179-35559655-e1d7-4573-9425-27491daeeaa5.png">
 
 + Mobile carrier at the interface is the minority carriers. 
 + Minority carrier are thermally generated meanwhile the mamjority carrier is derived from the ionized impurity .
 + Therfore it takes time to generate minority carriers .
 + Therefore in the high frequency circuit , the minority carriers does not have suffienct times to be generated .

  </details>   
  
   <details><summary> Non Ideal Structure </summary>
 
 <img width="645" alt="image" src="https://user-images.githubusercontent.com/121993910/212459766-3cd0e7ec-73db-4a5f-90fd-dc2ec664c0b1.png">

 + In non ideal MOS structure some of the parameters/concept will take into account such as the Effect of fixed Charge (Qf) 
 + Fixed charge is basically charge that is being traped on the oxide layer . This will attract the negative charge to the oxide-semiconducter interface . Creating a negarive potential eventhough it is zero applied gate voltage.  
 + This is due to the imperfection of the fabrication process during the silicon dioxide deposition . At the interface might have some Silicon hydroxide and other chemical .  
 + To balance this voltage a negative voltage is required so that the surface charge at the silicon will be zero . 
 
 + Another effect that can be take into account when deal with non ideal MOS is the effect of the work metal-semiconductor work function difference .
 + In ideal case the work function difference is assume to be 0 but in real case or non ideal case it is difference .
 + Because the fermi energy level are difference between metal and semiconductor and the fermi level also is depends on doping . 
 + Since typically the evergy of the metal is higher than the semiconductor ( Means the fermi level is higher ) the electrons will be transfer to the semiconductor side .
 + This cause the semiconductor to be more like a n-type since it receive electron from the metal .
 + Also the conduction band near the interface also will bend due to this electron recieved .
 + Due to this effect . There is some voltage or potential eventhough when zero gate voltage is applied .
 
 <img width="740" alt="image" src="https://user-images.githubusercontent.com/121993910/212461281-c9640e0e-fa86-4002-82db-9c3d435772b0.png">

 **Summary**
 
 <img width="430" alt="image" src="https://user-images.githubusercontent.com/121993910/212461258-8325431b-b95a-4376-8675-716f6c132c5c.png">

 + In non ideal case the flat-band voltage is needed to balance the voltage across the surface of the oxide-semiconductor .
 </details>
 
  ## Day 5
## Theory - Metal Oxide Semiconductor Field Effect Transistor(MOSFET) . 

<details><summary> MOSFET </summary>

<img width="611" alt="image" src="https://user-images.githubusercontent.com/121993910/212818122-12db1e62-0c9c-4461-ad24-66ebf6477abd.png">

*Top, front view and symbol of N and P MOSFET*

+ N-MOSFET = N-channel MOSFET
+ P-MOSFET = P-channel MOSFET 

+ Enhancement Mode - Need a bias to form a channel - Can be N and P type channel .
+ Depletion Mode - Channel already form even without bias - Can be N and P type channel

<img width="605" alt="image" src="https://user-images.githubusercontent.com/121993910/212819642-01cc6858-d2b4-4e3d-acb7-04fef3aec815.png">

*Cross section and symbol for all the type of MOSFET P/N channel enhancement mode (LHS) and P/N channel depletion mode (RHS).*  
 
 Layout view - There is a rule of spacing and minimum voltage need to be followed when doing layout . 
 Extension of poly - Across PVT the poly will decrease as this will caus e short circuit between drain and source .

</details>

<details><summary> MOSFET OPERATION </summary>
 
 **N Channel Enchancement**
 
 + As the name goes enchancement , the channel is enchance or form through a positive gate voltage as we discuss in the MOS structure chapter(Day4). The induced space charge region is form. 
 + A positive gate voltage induces the electron inversion layer, which then “connects” the n-type source and the n-type drain regions. 
 + The source terminal is the source of carriers that flow through the channel to the drain terminal
 + Meaning that the electron will flow from source to drain and current will be flow vice versa .

<img width="452" alt="image" src="https://user-images.githubusercontent.com/121993910/212854257-1524ae97-0adc-491b-846c-f8ee324267f7.png">

 *N channel enchancement mode MOSFET operation*

 + When Vgs is less than the threshold voltage . No channel will be form and no drain current will be flow . We call this as cut off operation . (Ideally)
 + When Vgs is greather than the threshold voltage .  An electron inversion layer has been created so that when a small drain voltage is applied, the electrons in the inversion layer will flow from the source to the positive drain terminal. ( Linear region ) 
 + The conventional current enters the drain terminal and leaves the source  terminal.
 
 <img width="207" alt="image" src="https://user-images.githubusercontent.com/121993910/212834841-edc9d445-9c56-4976-afaa-39608eb3a6b2.png">

 *Id-VGS characteristic graph (Ideally)* No including the weak inversion part or subtreshold current .
 
 <img width="507" alt="image" src="https://user-images.githubusercontent.com/121993910/212828917-7c2c039a-be1a-4992-aaa0-4222f213f114.png">

 *The n-channel enhancement mode MOSFET with an applied gate voltage VGS<VT and with VGS>VT.*
 
+ When the VDS value increases. The voltage drop across the oxide near the drain terminal decreases, which means that the induced inversion charge density near the drain also decreases . ( Still linear region ) (Vgs-vt < Vds) 
+ When VDS increases to the point where the potential drop across the oxide at the drain terminal is equal to VT, the induced inversion charge density is zero at the drain terminal . The VDS at this point is called VDS(sat) ( Vgs-Vt = Vds ) (Vds = Vdsat)
+ When VDS becomes larger than the VDS (sat) value, the point in the channel at which the inversion charge is just zero moves toward the source terminal. 
+ In this case, electrons enter the channel at the source, travel through the channel toward the drain, and then, at the point where the charge goes to zero, the electrons are injected into the space charge region where they are swept by the E-field to the drain contact .
+ At this point then the drain current will be a constant ( Act as constant current source). We call it as saturation region .
+ Id is not depend on VDS anymore . 
 
 <img width="655" alt="image" src="https://user-images.githubusercontent.com/121993910/212832840-12b87993-14d3-493a-aded-f72fe2fdaf56.png">

 + MOSFET Operation and its application . 
 
 <img width="219" alt="image" src="https://user-images.githubusercontent.com/121993910/212831587-c63286d0-80e0-4717-82b7-3799e316c9c7.png">
<img width="407" alt="image" src="https://user-images.githubusercontent.com/121993910/212854707-0a7a6a63-4a23-4ba8-90fa-a7cccf353d83.png">

 *Id-VDS  and Id-Vgs characteristic* 
 
 **P-Channel Enhancement**
 
 <img width="411" alt="image" src="https://user-images.githubusercontent.com/121993910/212854858-79e81c39-d38f-4c6b-aa76-29297848eadc.png">

 + For P channel reverse of n-enhancement  concept is applied where we applied a negative gate voltage(VSG)  to attract the holes and induced the space region .
 + Holes flow from the source to drain and same goes to the current.
 
 
</details>
 
<details><summary> Body Bias and channel Length modulation effect </summary>
 
 **Body Bias Effect**
 
<img width="722" alt="image" src="https://user-images.githubusercontent.com/121993910/212838536-6af25c40-4674-41a3-a945-7e09703398c4.png">

  + In Ideal case the subtrate and source terminal is connected to ground .
  + In real case the substrate and source may not have the some potential .
  + Therefore to achieve the same potential , source-to-substrate pn junction must always be zero or reverse biased, 
  + So VSB must always be greater than or equal to zero.
  + Same concept as the flat band voltage to achieve balance voltage due to the non ideal effect. 
  + Why VSB ? Why not VBS ? - Since the substrate is p type and the source is n type , if we applied a VBS , it will be a diode since it is foward bias . Meaning that there is a current flow from the subtrate to source . 
 
 + The space charge region width under the oxide increases from the original value when Vsb is applied. 
 + With an applied VSB>0, there is more charge associated with this region. Qd is increasing . Surface potential Fi(s) also will increases .
 + The positive charge on the top metal gate must increase to compensate for the increased negative space charge in order to reach the threshold inversion point. So when VSB>0, the threshold voltage of the n-channel MOSFET increases .
 
 <img width="238" alt="image" src="https://user-images.githubusercontent.com/121993910/212842753-decdf21a-b461-4e28-8e1d-3b89daf0a0e8.png">

 *Effect of Body Bias to the drain current* 
 
 ** Channel Length Modulation**
 
<img width="421" alt="image" src="https://user-images.githubusercontent.com/121993910/212855483-96dd272d-d8ac-4019-82bb-f100c34ea9c5.png">
 
 + In Ideal case we assume that the current and channel Length is constant . But in real case it is change due to channel length modulation effect. 
 + When the applying the VDS voltage until the VDS > VDS(sat) the transistor operate in saturation region . 
 + The depletion region at the drain terminal extends laterally into the channel, reducing the effective channel length .
 +  some typical ID versus VDS curves with positive slopes in the saturation region due to channel length modulation . 
 + Vds increase L will be decrease and current will be increase . 
 

 **Fabrication**
 
   <img width="530" alt="image" src="https://user-images.githubusercontent.com/121993910/212855972-3be7b525-3328-465b-be7d-f5ac3164c997.png">
 
 **Voltage**
+ Across PVT the threshold voltage as will get affected .
+ Threshold voltage depends on voltage across oxide + voltage accross depletion region 
+ voltage across oxide depends on thickness on the oxide . 
+ Voltage across depletion region depedns on the doping concentration p-substrate  and depletion volt .
 
 **Fabrication**
 
+ For imperfection farbication process of oxide , the thickness of the oxide itself may be varied.
+ The greather the thickness of the oxide the higher will be the threshold Voltage .
+ As substrate doping increases , threshold voltage increases as well .
+ q=CV q = 2qEsiNaFi(t)
 
**Temperature**
 
 + Mobility decrease as temperature increase . the carrier does not move smoothly.
 + As temperature increase the thershold voltage also increase .
 + Current decreases as temperature increases. 

 </details>
 
  ## Day 6
## Theory - MOSFET Intrinsic Capacitance  . 
 
 <details><summary> MOSFET Intrinsic Capacitance </summary>
  
  + is like a  natural capacitance existense in the MOSFET itself . 
  + When two electrical conductors at different voltages are close together, the electric field between them causes electric charge to be stored on them; this effect is capacitance.
  
  ![image](https://user-images.githubusercontent.com/121993910/213375571-f0b43f34-dde3-4e20-a2b4-ea6709fb289c.png)
  
  *Intrinsic Capacitance During Cut Off region*
  
 + Depletion region  is formed due as the PN junction between the P from subtrate and N from the drain are given a bias which is Vds . This configuration act as reverse bias . 
 + Due to this depletion region . A capacitance is formed between the drain and bulk . We called it as junction capacitance or depletion capacitance . 
 + This junction/depletion capacitance depends on the Vds voltage and the distance between the depletion region itself . 
 + This concepet also can be apply on the Csb but the depletion region on source is much smaller or lesser as it does not control by any voltage .
 + The overlap/extension  of the source and drain under the gate create a capacitance as well . We called it as the overlap capacitance . 
 +  Cgb is capacitance formed between the poly and the bulk . 
  
 ![image](https://user-images.githubusercontent.com/121993910/213375614-c77ea2fa-3137-4d6f-aa22-cc95f02c0626.png)

  *Intrinsic Capacitance During Linear region*
  
  +  The vds increase to get into the linear region , means that the depletion region on the source also increase causing the cdb to decrease . 
  +  Overlap capacitance remain constant as it is depends on the fabrication process .
  +  Difference is the existense of the cgsdch and cch-b 
  +  cgsdch exists due to the channel form . Between the poly and the channel a capacitance will be form. 
  + cch-b is the capacitance from the channel to bulk. 
  
 <img width="569" alt="image" src="https://user-images.githubusercontent.com/121993910/213381518-9674b015-4081-42f5-a872-1f36850f73e3.png">

  *Intrinsic Capacitance During Saturation region*
  
  +  As the depletion region deplete the channel in saturation region . 
  +  The capacitance of chdch is minimize/negelected  and cgsch is still available.
  
   ![image](https://user-images.githubusercontent.com/121993910/213375255-f72c9cfc-c3db-4912-b080-605b8a0c681e.png)

  * Capacitance summary for all capacitance formed in MOSFET*
  
  + 

 </details>
 
  <details><summary> Schematic Design, Circuit Simulation , Layout Design and Post Layout Simulation  </summary>
   
   *Overview of the IC design Flow *
   
   ![image](https://user-images.githubusercontent.com/121993910/213382115-8ca89dd5-a957-4ccc-8c84-057e1dc3e4ea.png)
   
   *Schematic Drawing Phase*
   
   ![image](https://user-images.githubusercontent.com/121993910/213382133-04536082-018f-4933-92b7-b8bbcfdcad93.png)
   
   *Circuit Simulation Phase*
   
   ![image](https://user-images.githubusercontent.com/121993910/213382147-13ce3db2-042b-4722-81cb-5b2a9c4c3b68.png)
   
   *Circuit Simulation Phase ( AC and Transient Responce)*

![image](https://user-images.githubusercontent.com/121993910/213382167-5514ae01-1a9a-4e57-9bc7-2bb98a5857e3.png)
   
   *Layout Phase*
   
   ![image](https://user-images.githubusercontent.com/121993910/213382668-1d2e9367-bba1-4bb8-b75c-c700588e7f0c.png)
   

  
   </details>
 </details>
 
 ## Day 7
## Theory - MOSFET Inverter 
 
 <details><summary> Overview </summary>
 
![image](https://user-images.githubusercontent.com/121993910/214774913-10402b77-5195-4afc-bb4a-23fd24a6e0bb.png)

 + CMOS inverter is the most basic (nucleolus) of all digital design. ( concept can be apply to the other gate as well)
 + Due to its popularness in the digital design understanding the characteristic(static and drynamic) of cmos inverter would be a good benefical to us . 
 + In this case , we would analyze the cmos inveter aspect interm of **cost**, **Integrity and Robustness**, **Performance** and **Energy Efficiency** .
 
 + Cost - depends on complextity and area 
 + Integrity and Robustness - Depend on the static behaviour (leakage) . Ideally static current is 0 but in real case not 0 . 
 + Performance -  Performance related to freqeuncy . Also related to the dynamic responce .
 + Energy Efficiency - The higher the freqeuncy the higher will be the power consumption. swtiching/transiton , leakage related  . 
 
  </details>
  
 <details><summary> Static Characteristic </summary>
 
<img width="512" alt="image" src="https://user-images.githubusercontent.com/121993910/214774947-a2d8acba-af63-4b9a-92b6-ade94798988e.png">

 
+ Act as a switch . Practically there is an finite on resistance when the transitor is on and infinite off resistance when the transitor is off . Ideally would be 0 . 
+ Input 1 Output 0 (NMOS will turn on and the output will pull to the GND)
+ if Input 0 Output would be 1 (PMOS will turn on and the output will put to VDD)
 
 ![image](https://user-images.githubusercontent.com/121993910/214775400-3f36a55b-8b55-44fd-89fd-a524a1d5fa8d.png)

 + Rail to rail means always VDD or GND cannot be at the middle . Like peak to peak . Results in high noise margin .
 + It is independent to the size or rationless. Means it always 1 or 0 . 
 + Other technology such as NMOS technology would depend on size to get certain voltage . 
 + This means very small size of CMOS inverter would give VDD/GND .
 + This helps to reduce area and cost . 
 + there is always a finite resistance between the output and vdd or ground means rn or rp . causing it to be low output impedance .
 + The output impedance refers to the impedance, or opposition to current flow, of the component that often bears an electrical source to "drive" a load component .
 + means it is less sensitive to noise .
 + Imput impedance almost infinity meaning that no current flow and able to drive multiple or inifinite number of gate .
 + By driving multuple gate fanout capacitance will increase the propagation delay . 
 + Static power almost 0 means that there is very small current flowing from VDD to the GND . 
 
 ![image](https://user-images.githubusercontent.com/121993910/214780593-b4749a40-8d09-4c0e-83f6-2cf6290ddd9d.png)

 *Voltage Transfer Characteristic*
 
 + At the symmertical point , the resitance of rn and rp is the same . 
 + typicaly to get symmetrical , PMOS size is usually 2.5 to 3 size of NMOS . 
 
 ![image](https://user-images.githubusercontent.com/121993910/214780570-96fe2fa8-5756-450a-b40a-546262d84c84.png)

 *MOSFET Strength Variation*
 
 + Strength is related to the W of the Nmos and PMOS 
 + Strong means the W is larger while weak means the Width is smaller
 + Width is propotional to the current . Means more width more current and more conductive .
 + Ex . Strong NMOS means we increase the conductivity of the NMOS , means that the Nmos resistance will be decrease so that use less voltage to conduct . So the graph will shift to left .
 + Ex. Strong nmos will pull the graph to the right as it required more voltage to conduct . 
 
 ![image](https://user-images.githubusercontent.com/121993910/214780468-bface754-37f9-4ed7-9d9c-201112efd0c2.png)

 *Noise Margin CMOS inverter*
 
 + Noise Margin - How much noise can the inverter tolerate . 
 + VIH - Minimum input voltage so that the VOH is low . or consider as the minimum input voltage so that the inverter recognized the input voltage as 1 
 + VIL - Maximum input voltage so that the VIH is high . or consider as the maximum input voltage so that the inverter recognized the input voltage as 0 .
 + VOH - The maixumum output voltage so that the inverter recognized the voltage as logic 1 .
 + VOL - The minumum output voltage so that the inverter recognized the voltage as logic 0 . 
 + Less noise margin means the inverter is more sensitive to noise .
 + more noise margin means the inveter is less sensitive to noise .
 + 
 
   </details>
 
 <details><summary> Dynamic Characteristic </summary>

![image](https://user-images.githubusercontent.com/121993910/214783691-8e251c43-d30d-4bcc-aaf3-ef13d634090a.png)

 + Dyanmic is more related to time while static means more to steady state .
 + The CL is very crutial as it will affect the propagation delay , and rise/fall time of the inverter .
 + The finite resistance Rn and Rp plus the CL will give the responce to the delay . 
 
 ![image](https://user-images.githubusercontent.com/121993910/214784466-d3ec26c1-05ce-4604-ab22-257d2f149bb7.png)

 + The CL is consist of 

  **Instrinsic Capacitance** - Capacitance inside the cmos which is the junction capacitance .
  **Wiring Capacitance** - Capactiance due to the metal routing, interconnect .
  **Fanout Capacitance** - Capactiance due to the gate capacitance of next device or gate . 
 
 + The capacitance due to the wiring depends upon the length and width of the connecting wires, and is a function of the distance of the fanout from the driving gate and the number of fanout gates
 
 ![image](https://user-images.githubusercontent.com/121993910/214785221-9f2ce73b-9e38-4094-a05d-ddbfa1f8bfb1.png)

 *Rise Time Defination* Capactior need times to charge , not suddenly charging. 
 
 ![image](https://user-images.githubusercontent.com/121993910/214785400-7f656323-6908-4bb2-9ade-3ec098a88248.png)
 
 *Fall time Defination* capacitor need time also to discharge . 

 ![image](https://user-images.githubusercontent.com/121993910/214785593-a41fe647-662a-4028-b662-0452eaedddcf.png)

 *Propatgation Delay Defination* 
 
 + Hence, a fast gate is built either by keeping the output capacitance small or by decreasing the on-resistance of the transistor.
 + Aware that the on-resistance of the NMOS and PMOS transistor is not constant, but is a nonlinear function of the voltage across the transistor.
 + propagation delay of the CMOS inverter is determined by the time it takes to charge and discharge the load capacitor CL  through the PMOS and NMOS transistors
 
 ![image](https://user-images.githubusercontent.com/121993910/214981725-6b34b5d6-0793-4a52-8adb-fd1590878918.png)
 
 + layout helps to reduce the diffusion and interconnect capacitances .
 + This flexibility allows the designer to trade-off energy dissipation for performance .
 + Also, reliability concerns (oxide breakdown, hot-electron effects) enforce firm upper-bounds on the supply voltage in deep sub-micron processes.
 
 ![image](https://user-images.githubusercontent.com/121993910/214983608-c2ab18e0-6bd6-4017-9b7c-6987782e9085.png)

 *The effect of input transition with different output load*
 
 
   </details>
   
   <details><summary> Power Consumption </summary>
 
 + Another major factor for static CMOS is the almost complete absence of power consumption in steady-state operation mode .
 
 **Dynamic Power Consumption**
 
 ![image](https://user-images.githubusercontent.com/121993910/214983998-4e14c49d-7fe7-4138-832f-0065a78b99b3.png)

.+ switching activity will affect the power dissipation.
 + More switching will casue more power consumption. 
 
 ![image](https://user-images.githubusercontent.com/121993910/214984734-3915b0cd-c2cc-4ea8-ac00-4e6632610b83.png)

 + The finite slope of the input signal causes a direct current path between VDD and GND for a short period of time during switching, while the NMOS and the PMOS
transistors are conducting simultaneously .
 + peak current is also a strong function of the ratio between input and output slopes
 + short-circuit dissipation is minimized by making the output rise/fall time larger than the input rise/fall time .
 + making the output rise/fall time too large slows down the circuit and can cause short-circuit currents in the fan-out gates 
 
 **Static Cpnsumption**
 
 ![image](https://user-images.githubusercontent.com/121993910/214985837-1a1bc4e2-58f8-4d4f-8174-2f8c8a0b98e7.png)
 
 + Due to the reverse bias diode and the subthreshold current . 
 + Ideally would be 0 . 
 
 ![image](https://user-images.githubusercontent.com/121993910/214986375-9d18548f-1666-4180-95ae-dca2a3ccee78.png)
 
 *Summarry of the power consumption*
 
 + The PDP stands for the average energy consumed per switching event


  
 
 </details>
   
   
  </details>   
