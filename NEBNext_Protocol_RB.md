#Protocol for use with NEBNext Ultra DNA Library Prep Kit for Illumina (E7370)

[toc]

Starting material is RAD library prep, 55.5ul

##1.1 NEBNext End Prep  

1. Mix the following in a sterile tube:
	
	|Color| Component | Volume | 
	|:---:|:---:| :---:|
	Green | End Prep Enzyme Mix | 3.0 μl   
	Green |  End Repair Reaction Buffer (10X) |  6.5 μl
	na | Fragmented DNA | 55.5 μl
	Total volume: 65 μl

2. Mix by pipetting followed by a quick spin to collect all liquid from the sides of the tube.
3. Place in a thermocycler, with the heated lid on, and run the follwing program:  

	|Time| Temp |  
	|:---:|:---:|
	|30 minutes | 20°C |
	|30 minutes | 65°C |
	| hold |  4°C |

	 
## 1.2 Adaptor ligation	
Because DNA input is < 100 ng, dilute the NEBNext Adaptor for Illumina (provided at 15 μM) 10-fold in 10 mM Tris-HCl to a final concentration of 1.5 μM, use immediately. ie, 1 ul adaptor into 9ul tris  

1. Add the following components directly to the End Prep reaction mixture and mix well:  
	
	|Color| Component | Volume |    
	|:---:|:---:|:---:|  
	|red|Blunt-TA Ligase Master Mix| 15 μl|
	|red|NEBNext Adaptor for Illumina* |2.5 μl
	|red | ligation enhancer | 1μl|
	Total volume 83.5 μl  
	*the NebNext Adaptor for Illumina is in the Multiplex kit  

2. Mix by pipetting followed by a quick spin to collect all liquid from the sides of the tube.
3. Incubate at 20°C for 15 minutes in a thermal cycler.
	- Protocol: "NEB_DNA" ->"Adaptor" 	
4. Add 3 μl of USER enzyme to the ligation mixture from Step 3. (found in the multiplex kit)
5. Mix well and incubate at 37°C for 15 minutes.
	- in heat block

#1.3 Size Selection of Adaptor-ligated DNA 

The following size selection protocol is for libraries with 200 bp inserts only. For libraries with different size fragment inserts, refer to Table 1.1 for the appropriate volume of beads to be added. The size selection protocol is based on a starting volume of 100 μl.  

1. Vortex AMPure XP Beads to resuspend.  
2. Add 13.5 μl dH2O to the ligation reaction for a 100 μl total volume.  
3. Add 55 μl of resuspended AMPure XP Beads to the 100 μl ligation reaction. Mix well by pipetting up and down at least 10 times.  
4. Incubate for 5 minutes at room temperature.  
5. Quickly spin the tube and place the tube on an appropriate magnetic stand to separate the beads from the supernatant. After the solution is clear (about 5 minutes), carefully transfer the supernatant containing your DNA to a new tube **(Caution: do not discard the supernatant)**. Discard the beads that contain the unwanted large fragments.    
6. Add 25 μl resuspended AMPure XP Beads to the supernatant, mix well and incubate for 5 minutes at room temperature.  
7. Quickly spin the tube and place it on an appropriate magnetic stand to separate the beads from the supernatant. After the solution is clear (about 5 minutes), carefully remove and discard the supernatant that contains unwanted DNA. Be careful not to disturb the beads that contain the desired DNA targets **(Caution: do not discard beads)**.
8. Add 200 μl of 80% freshly prepared ethanol to the tube while in the magnetic stand. Incubate at  room temperature for 30 seconds, and then carefully remove and discard the supernatant. 
9. Repeat Step 8 once.
10. Air dry the beads for 5 minutes while the tube is on the magnetic stand with the lid open.                                   **Caution: Do not overdry the beads. This may result in lower recovery of DNA target.**
11. Remove the tube/plate from the magnet. Elute the DNA target from the beads into 17 μl of 10 mM Tris-HCI or 0.1 X TE. Mix well on a vortex mixer or by pipetting up and down. Incubate for 2 minutes at room temperature. 
12. Quickly spin the tube and place it on a magnetic stand. After the solution is clear (about 5 minutes), transfer 15 μl to a new PCR tube for amplification. 
13. Proceed to PCR Amplification in Section 1.4.

![](/Users/reidbrennan/Documents/Lab Methods/SizeSelection.png)  

##1.4 PCR Enrichment of Adaptor Ligated DNA

1. Mix the following components in a sterile nuclease-free tube:

	|Color| Component | Volume |    
	|:---:|:---:|:---:|  
	|blue | NEBNext Q5 Hot Start HiFi PCR Master Mix | 25 μl|
	|blue | Index Primer | 5 μl |
	|blue| Universal PCR Primer | 5 μl|

2. PCR Cycling Conditions:
	
	![](/Users/reidbrennan/Documents/Lab Methods/PCRCycle.png)

3. Proceed to Cleanup of PCR Amplification Section 1.5.

## 1.5 Cleanup of PCR Amplification

1. Vortex AMPure XP Beads to resuspend.
2. Add 45 μl of resuspended AMPure XP Beads to the PCR reactions (~ 50 μl). Mix well by pipetting up and down at least 10 times.
3. Incubate for 5 minutes at room temperature.
4. Quickly spin the tube and place it on an appropriate magnetic stand to separate beads from supernatant. After the solution is clear (about 5 minutes), carefully remove and discard the supernatant. Be careful not to disturb the beads that contain DNA targets(Caution do not discard beads).
5. Add 200 μl of 80% ethanol to the PCR plate while in the magnetic stand. Incubate at room temperature for 30 seconds, and then carefully remove and discard the supernatant.
6. Repeat Step 5 once.
7. Air dry the beads for 5 minutes while the PCR plate is on the magnetic stand with the lid open. ***Caution: Do not overdry the beads. This may result in lower recovery of DNA target.***  
8. Remove the tube/plate from the magnet. Elute DNA target from beads into 33 μl 0.1X TE. Mix well by pipetting up and down at least 10 times. Quickly spin the tube and incubate at room temperature for 2 minutes.
9. Place the sample on an appropriate magnetic stand to separate beads from supernatant. After the solution is clear (about 5 minutes), carefully transfer 28 μl supernatant to a new PCR tube. Libraries can be stored at –20°C.
10. Dilute 2-3 μl of the library 5 fold with 10 mM Tris-HCl or 0.1X TE and check the size distribution on an Agilent Bioanalyzer® (high sensitivity chip).


	
	
