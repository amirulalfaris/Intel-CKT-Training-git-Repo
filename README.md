# Test

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
   [CMOS Fabrication Process in Deep-Submicron (DSM) and Ultra Deep- Submicron (UDSM) Technology}(https://github.com/amirulalfaris/Intel-CKT-Training-git-Repo#day-3)
    </details>
    <details><summary> Lab </summary>
     [Assignment day 3 ](link)
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
 
 
 
