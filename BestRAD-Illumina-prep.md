## BestRAD Illumina library Prep

This method was developed by Mike Miller's Lab at UCD and described in the citation below:

Ali, Omar A., et al. "RAD capture (Rapture): flexible and efficient sequence-based genotyping." Genetics 202.2 (2016): 389-400.


### Part 1: Digestion, RAD adaptor ligation, and shearing.

1. Into each 96 plate well, pipete X ul genomic DNA (50 ng in less than or equal to 10 ul). Can use more than 50 ng (up to 250 ng) to decrease number of pcr cycles down the line.
2. Into each 96 plate well, pipet Y ul low TE (Y = 10 – X)
3. Into 1.5 ml tubes, make SbfI digestion master mix.
	1. Make sure to add SbfI LAST. 
	2. After SbfI is added, go quickly to next step
	3. Always keep SbfI cold and only bring out of freezer for very short periods. 
	4. To prevent evaporation, keep plate covered until right before adding master mix

	100X: 68 ul water, 120 ul  NEBuffer 4, 12 ul SbfI-HF (NEB R3642L).  
	____ X: _____ water; _____ NEB 4; _____ SbfI

4. To each 96 plate well, pipet 2ul SbfI digestion master mix
	1. Mix by pipetting a few times
	2. Seal plate and vortex to mix. respin.
5. Incubate samples, “Digest” Protocol
	1. 37 C for 60 min
	2. 80 C for 20 min
	3. Can store at 10 C (temporarily), or -20 C
6.	Add 2 ul annealed BestRad SbfI adaptors (50 nM)
7. Make ligation master mix:
	1.  Always add enzyme last, move quickly to step 9.
	
	100X: 128 ul water, 40 ul NEB4, 16 ul rATP (100 mM, Fermentas R0441), 16 ul Ligase (NEB M0202L)  
	____ X: _____ water; _____ NEB 4; _____ rATP; _____ Ligase
8. Into each 96 plate well, pipet 2 ul ligation master mix.
9. Incubate Samples, “Ligate” Protocol
	1. 20 C for 12h (note, this is for less concentrated ligase)
	2. 65 C for 20 min
		1. Can freeze at -20 after this step if necessary.
10. Into 1.5 ml tube, pipet 3-8ul each 96 plate well. Store plate for future multiplexing.
	1. Can use 4ul at this step to preserve more dna to reuse. If you’re going to renormalize, use 3-4ul so there’s enough left to renormalize.
11. Concentrate sample to 210 ul with ampure 1X. Divide sample into two Bioruptor tubes.
	1. For 1 X, add same volume as DNA in tube.
	2. 1x wash 2 times with Etoh
	3. bring up in low TE
12. Sonicate with BioRuptor NGS. Use 9 cycles: 30 sec on, 90 sec off. 
13. Run each tube on frag analyzer, bioanalyzer, or gel. Want 250-500 bp fragments. Reshear if necessary.

### Part 2: RAD tag physical isolation.

Trying to remove all DNA without adapters. The streptavidin binds biotin, which is in the adapter. Then you’re cutting the adapter from the beads with sbfI and freeing the fragments.

-2X Binding and Wash (B+W) Buffer: (10 mM Tris-HCL (pH 7.5), 1 mM EDTA pH 8.0, 2 M NaCl)

*Prepare Dynabead M-280 streptavidin magnetic beads*

1. Transfer 20 ul Dynabeads to a new 1.7 ml tubes
2. Place tube in magnetic rack and remove supernatant
3. Wash the beads with 100 ul 2X B+W buffer, mix 30”, quick spin, remove sup.
4. Repeat wash once.
5. Resuspend beads in 200 ul 2X B+W buffer
	1. Use same volume as DNA that was sonicated. May need to change this volume.

*Bead Binding*

6. Add resuspended beads to sonicated DNA. Incubate at RT for 20 min, mix every 2 minutes
7. Quick spin, place tube on magnetic rack. Remove sup, resuspend beads in 150 ul 1X B+W Buffer at Room temp.
8. Repeat wash step
9. Repeat wash Step (3 times total)
10. Wash with 56 C 150 ul 1X B+W (higher temp removes more)
11. Wash with 56 C 150 ul 1X B+W (two total at 56 C)

*Liberate DNA from Beads*

12.	Resuspend the final washed beads in 100 ul 1X NEB Buffer 4.
13.	Place on magnetic rack, remove sup.
14.	Repeat NEB 4 wash once.
15.	Resuspend beads and bound DNA in 40 ul 1X NEB Buffer 4
16.	Add 2 ul SbfI-HF (NEB R3642L)
	1. Then vortex. This cuts off biotin and frees dna from beads
17.	Incubate tube at 37 C for 60 minutes (can store at 4C overnight after this if necessary).
18.	Quick spin, place on magnetic rack. **KEEP SUP! This has the DNA.**
19.	Ampure 1X,
	1.	Add equal volume Ampure as Sup. Vortex, spin, incubate at RT for 5 min.
	2.	Place on magnet, remove Sup.
	3.	Add 190 ul fresh 80% etoh. Mix, Remove Sup
	4.	Repeat Etoh wash (2 total).
	5.	Spin down, remove etoh. Let dry COMPLETELY, until cracks.
20.	Resuspend in 55 ul low TE
	1.	Add TE, mix, incubate 5 min at RT. 
	2.	Place on magnet and **KEEP SUP**.

### Part 3:

Use full reactions NEBNext Ultra DNA Library Prep Kit for Illumina (NEB E7370S/L) with no modifications<sup>2,3</sup>. Use 1:10 diluted adaptor. 

In this kit, elute in 22ul low TE. Then take 20% of product and run PCR for 15 cycles. Back calculate to figure out how many steps necessary for the other 80% of sample. Keep the 80% of sample  

Once start kit, don’t stop before reaching PCR step. Can pause/ freeze sample before running PCR.

Additional Notes: 

<sup>1</sup> Genomic DNA quantity should be identical in each plate well. We have used between 50-250 ng.

<sup>2</sup> We use ~20% of the template to perform a test PCR using 15 cycles and run the product on a fragment
analyzer to determine yield. A second PCR is then performed with the remaining template using fewer
cycles informed by the fragment analyzer results (typically 8-12, depending on DNA quantity, quality,
and restriction enzyme choice).

<sup>3</sup> We have tested NEBNext Ultra II DNA Library Prep Kit for Illumina, but it produced poorer quality
libraries than the NEBNext Ultra DNA Library Prep Kit.





 






 	

 
