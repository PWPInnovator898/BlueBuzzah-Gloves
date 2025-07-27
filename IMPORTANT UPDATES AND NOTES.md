# 05-06-25: NOTE FOR 3D print .STL FILES:
indicating that the lids for the Blue Buzzah tactors and enclosures rely on a precise friction fit that was designed using a Bambu P1S printer with ABS filament.  Using a different type of printer and/or filament may result in enclosure lids and tactor caps that ending up being too tight or too loose.  The Etsy vendor listed in our parts list has verified proper fit of a test print of our STL using his Bambu X1C printer.  

# 6-2-25: UPDATED 3D PRINT FILES FOR ENCLOSURES AND TACTORS:  
Enclosure changes:  - 2mm higher to make sure the PCB module doesnt bump the inside ceiling. - no more cosmetic artifact that upsets some 3D print vendors in the wire exit window.  - larger window for USB connector
Tactor changes: - relocates bottom brace in tactor cap so LRA electrical connections dont touch cap when the button is depressed (potentially conducting a small amount of vibrations to case).  - open bottom of cap now allows tactor to be removed from LRA without desoldering wires from PCB (this is important if you want to swap the 11 mm thick tactors for one of the new 9mm or 10 mm tactors that will be posted soon)?

# 7-10-25: UPDATED BLUE BUZZAH CODE
A new version of our Blue Buzzah code has been posted that includes:
- Hybrid Pattern mode now works within specs - allowing jitter to be added with mirroring off which is essentially Tass's Regular and Noisy patterns combined together (including independent finger randomization along with jitter)
- Randomized frequency is now tested and in specs - allowing randomized frequency for every buzz sequence within a range set by the user (for example the frequency range may be set to range from 220 Hz and 260 Hz in which case you might have frequency of 225 Hz one sequence, then 253 Hz the next, then 237 Hz and so on. It is an feature to help prevent habituation to the buzzing)
- **IMPORTANT: It is no longer necessary to change the pattern type when adjusting default parameters.  Please now disregard the section on pattern type on page 67 of build instructions version 1.2.  Instead, users should leave PATTERN_TYPE = "RNDP"  for all settings.**

# 7-27-25 NOTE ABOUT SOLDERING BAT CONNECTION  
![soldering BAT connection4](https://github.com/user-attachments/assets/42566705-f391-449e-af5e-26177d48cfab)
- Be careful when soldering the BAT connection on top of the feather.  It's proximity to the battery socket makes it difficult to solder. If you're not careful, it is easy to get too much solder on that connection and end up with a ball of solder going over to the battery nearby socket and grounding out your connection.

# 7-27-25 UPDATE TO SOLDERING RECOMMENDATIONS
- In Step 2.1 g of the build pdf version 1.2,  we previously recommended that builders solder all of the pins from the headers on the underside of the PCB.  ![sold rec 1](https://github.com/user-attachments/assets/354dc7b3-edcd-46b4-b100-584c277a320b)
- However, since only the 9 pins we identified on the top of the PCB are active in our design in step 2.2e, we are now changing this recommendation.   In order to minimize the potential for novice builders making an error during soldering, especially in areas where traces run near to connections, we now recommend that builders only solder the nine active pins under the PCB.
  ![sold rec 2](https://github.com/user-attachments/assets/ac5a2b52-e328-4438-ae99-2fb801e1cbae)
