# 1) IT IS BEST TO USE BAMBU PRINTER TO MAKE 3D PRINTS, 5-06-25: 
Added note in stl files indicating that the lids for the Blue Buzzah tactors and enclosures rely on a precise friction fit that was designed using a Bambu P1S printer with ABS filament.  Using a different type of printer and/or filament may result in enclosure lids and tactor caps that ending up being too tight or too loose.  The Etsy vendor listed in our parts list has verified proper fit of a test print of our STL using his Bambu X1C printer.  

# 2) POSTED UPDATED 3D PRINT FILES, 6-2-25:  
- Made lid 2mm higher to make sure the PCB module doesn’t bump the inside ceiling
- Removed cosmetic artifact that upsets some 3D print vendors in the wire exit window
- Made larger window for USB connector to pass
- Still need to make hole to view yellow charging light!
- Relocated bottom brace in tactor cap so LRA wires don’t touch brace when the button is depressed potentially conducting a small amount of vibrations to case.  
- Open bottom of cap now allows tactor to be removed from LRA without desoldering wires from PCB.   This is important if you ever need to swap tactors out.

# 3) UPDATED BLUE BUZZAH CODE, 7-10-25: 
The June 24, 2025 version of our Blue Buzzah code includes the following fixes to the earlier code:
- Hybrid Pattern mode now works within specs allowing jitter to be added with mirroring off which is essentially Tass's Regular and Noisy patterns combined together (including independent finger randomization along with jitter)
- Randomized frequency is now tested and in specs - allowing randomized frequency for every buzz sequence within a range set by the user (for example the frequency range may be set to range from 220 Hz and 260 Hz in which case you might have frequency of 225 Hz one sequence, then 253 Hz the next, then 237 Hz and so on. It is an feature to help prevent habituation to the buzzing)
- **IMPORTANT: It is no longer necessary to change the pattern type when adjusting default parameters.  Please now disregard the section on pattern type on page 67 of build instructions version 1.2.  Instead, users should leave PATTERN_TYPE = "RNDP"  for all settings.**

# 4) BE CAREFUL SOLDERING BAT CONNECTION, 7-27-25:   
![soldering BAT connection4](https://github.com/user-attachments/assets/42566705-f391-449e-af5e-26177d48cfab)
- The BAT pin is awkward to solder due to its close proximity to the battery socket as shown here.  In one build, I accidentally put too much solder on this pin and the solder overflowed on to a grounding plate for the battery socket.  Since the plastic socket blocks easy access, it was very difficult getting the solder back out.  I ended up needing a desoldering tool to remove the excess solder.   

# 5) UPDATE TO SOLDERING RECOMMENDATIONS, 7-27-25: 
- In Step 2.1 g of the build pdf version 1.2,  we previously recommended that builders solder all of the pins from the headers on the underside of the PCB.
    ![sold rec 1](https://github.com/user-attachments/assets/354dc7b3-edcd-46b4-b100-584c277a320b)
- However, since only the 9 pins we identified on the top of the PCB are active in our design in step 2.2e, we are now changing this recommendation.   In order to minimize the potential for novice builders making an error during soldering, especially in areas where traces run near to connections as shown above, we now recommend that builders only solder the nine active pins under the PCB.
  ![sold rec 2](https://github.com/user-attachments/assets/ac5a2b52-e328-4438-ae99-2fb801e1cbae)

# 6) WE ARE TESTING BLUE BUZZAH SHOES, 7-27-25: 
![bb shoes2](https://github.com/user-attachments/assets/06aa9b5b-3bff-41fe-bd4b-18d34a031c4c)

# 7 NOTE: THE BB GLOVE IS CHALLENGING TO FIT PERFECTLY:
To be clear, the Blue Buzzah was not designed to maximize ease of construction for novice builders and provide for foolproof operation for novice users.  These admirable qualities be found in some other DIY designs, but not with ours.  Instead, we designed our gloves to meet our needs which are (in order of importance): 
- 1) Closest possible adherence to Tass glove specifications (See detailed review and bench tests at, https://github.com/TactileDesign/Reviews-of-Vibrating-Gloves-for-Parkinsons )
- 2) Ease of putting on and taking off (See video of first prototype at, https://www.youtube.com/watch?v=fcnbQDe73uA)
- 3) Highest level of dexterity to promote active lifestyle while using tactors
- 4) Relatively normal aesthetic appearance when using gloves in public situations  
- Not this: Maximum ease of construction for novice builders… No.
- Not this: Foolproof operation for novice users…  No.
- As you can see in the images below, as per our design choices, our fingertip tactors are somewhat smaller, less conspicuous, lighter, and easier to put on than the original Tass tactors.  That said, these advantages come with a greater required level of awareness from users.  Specifically, since each tactor is held in place on a user’s by the elasticity of the glove fingers rather than an individually adjusted Velcro lash, the choice of glove size is critical. Our gloves then require a bit more time to fit properly and a continual low level of “buzz awareness” to make sure that the fingertip placement of the tactors remains ideal.  Users who decide to replicate our design need to be aware of these issues in order to ensure that the tactors provide the proper vibration characteristics to the user’s fingertips.  The entire vCR therapy Dr. Tass has described depends on the tactor’s ability to reproduce the very detailed vibration characteristics.  If any issue arises that interferes with the administereation of the buzzes, the potential efficacy of therapy can be compromised. 
![7 - comparison](https://github.com/user-attachments/assets/acafecd8-c0f0-46cf-9d17-5c94c372d394)
