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

* **Moore's Law** - Number of trasistor in an integated Chip (IC) will doubles about every two years. Size will be reduce to 1/(Square root of 2)

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


  

  

 
   
