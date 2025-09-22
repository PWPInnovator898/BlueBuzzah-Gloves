# TABLE OF CONTENTS
- (1) IT IS BEST TO USE BAMBU PRINTER TO MAKE 3D PRINTS, 5-06-25: 
- (2) POSTED UPDATED 3D PRINT FILES, 6-2-25:  
- (3) UPDATED BLUE BUZZAH CODE, 7-10-25: 
- (4) BE CAREFUL SOLDERING BAT CONNECTION, 7-27-25:   
- (5) NEW RECOMMENDATION: DONT SOLDER UNUSED PINS, 7-27-25: 
- (6) WE ARE TESTING BLUE BUZZAH SHOES, 7-27-25: 
- (7) PICTURES OF DIY GLOVES SENT IN FROM BLUE BUZZAH USERS
- (8) THE BB GLOVE IS CHALLENGING TO FIT PERFECTLY:
- (9) SOME USERS ARE GETTING FINGER FIT TOO LOOSE
- (10) I MADE A SET THAT WAS TOO TIGHT
- (11) ELEGANT CUSTOM DESIGN FROM A BB USER FOR FINGERTIPS
- (12) SOME BUILDERS ARE MAKING GLOVES WITHOUT GLOVES
- (13) DEALING WITH A JAMMED BUTTON  
- (14) AMPLITUDE NEEDS TO BE SET LOWER
- (15) NOTE ABOUT USING AMPLITUDE RANDOMIZATION
- (16) SEEK EXPERT HELP IF YOU ARE NEW TO SOLDERING 
- (17) USING AN APPLE COMPUTER TO FORMAT FEATHER MODULES
- (18) RECOMMENDATION CHANGE: INSTALL SOCKETS ON PCB 
- (19) TENDONITIS REPORT FROM EXCEEDING 2 HOUR SESSIONS    
- (20) RIGHT AND LEFT DEFAULTS FILES MUST BE IDENTICAL
- (21) RARE BLUETOOTH INTERFERENCE PROBLEMS REPORTED
- (22) START BOTH GLOVES TOGETHER TO AVOID TIMEOUT ERROR
- (23) HOW TO PURCHASE SPRINGS INSTEAD OF WINDING DIY, 9-21-25
- (24) GET A SPARE BATTERY, 9-22-25
- -----------------------------------------------------------------------------
# 1) IT IS BEST TO USE BAMBU PRINTER TO MAKE 3D PRINTS, 5-06-25: 
Added note in stl files indicating that the lids for the Blue Buzzah tactors and enclosures rely on a precise friction fit that was designed using a Bambu P1S printer with ABS filament.  Using a different type of printer and/or filament may result in enclosure lids and tactor caps that ending up being too tight or too loose.  The Etsy vendor listed in our parts list has verified proper fit of a test print of our STL using his Bambu X1C printer.  
![01 bambu](https://github.com/user-attachments/assets/8610dfcf-fe1f-40ab-b48d-7b67145a6be7)

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

# 5) NEW RECOMMENDATION: DONT SOLDER UNUSED PINS, 7-27-25: 
- In Step 2.1 g of the build pdf version 1.2,  we previously recommended that builders solder all of the pins from the headers on the underside of the PCB.
    ![sold rec 1](https://github.com/user-attachments/assets/354dc7b3-edcd-46b4-b100-584c277a320b)
- However, since only the 9 pins we identified on the top of the PCB are active in our design in step 2.2e, we are now changing this recommendation.   In order to minimize the potential for novice builders making an error during soldering, especially in areas where traces run near to connections as shown above, we now recommend that builders only solder the nine active pins under the PCB.
  ![sold rec 2](https://github.com/user-attachments/assets/ac5a2b52-e328-4438-ae99-2fb801e1cbae)

# 6) WE ARE TESTING BLUE BUZZAH SHOES, 7-27-25: 
![bb shoes2](https://github.com/user-attachments/assets/06aa9b5b-3bff-41fe-bd4b-18d34a031c4c)

# 7) PICTURES OF DIY GLOVES SENT IN FROM BLUE BUZZAH USERS
![09 usders ex 1](https://github.com/user-attachments/assets/ac1fae92-d7b1-4174-b18e-63fe5d02945a)
- more to come...

# 8) THE BB GLOVE IS CHALLENGING TO FIT PERFECTLY:
To be clear, the Blue Buzzah was not designed to maximize ease of construction for novice builders and provide for foolproof operation for novice users.  These admirable qualities be found in some other DIY designs, but not with ours.  Instead, we designed our gloves to meet our needs which are (in order of importance): 
- 1) Closest possible adherence to Tass glove specifications (See detailed review and bench tests at, https://github.com/TactileDesign/Reviews-of-Vibrating-Gloves-for-Parkinsons )
- 2) Ease of putting on and taking off (See video of first prototype at, https://www.youtube.com/watch?v=fcnbQDe73uA)
- 3) Highest level of dexterity to promote active lifestyle while using tactors
- 4) Relatively normal aesthetic appearance when using gloves in public situations  
- Not this: Maximum ease of construction for novice builders… No.
- Not this: Foolproof operation for novice users…  No.
- As you can see in the images below, as per our design choices, our fingertip tactors are somewhat smaller, less conspicuous, lighter, and easier to put on than the original Tass tactors.  That said, these advantages come with a greater required level of awareness from users.  Specifically, since each tactor is held in place on a user’s by the elasticity of the glove fingers rather than an individually adjusted Velcro lash, the choice of glove size is critical. Our gloves then require a bit more time to fit properly and a continual low level of “buzz awareness” to make sure that the fingertip placement of the tactors remains ideal.  Users who decide to replicate our design need to be aware of these issues in order to ensure that the tactors provide the proper vibration characteristics to the user’s fingertips.  The entire vCR therapy Dr. Tass has described depends on the tactor’s ability to reproduce the very detailed vibration characteristics.  If any issue arises that interferes with the administereation of the buzzes, the potential efficacy of therapy can be compromised. 
![7 - comparison](https://github.com/user-attachments/assets/acafecd8-c0f0-46cf-9d17-5c94c372d394)

# 9) SOME USERS ARE GETTING FINGER FIT TOO LOOSE
- The BB tactors have a spring loaded button which needs to be completely depressed by the fingertip such that the user can feel their finger making contact with the entire area on top of the tactor case surrounding the button.  Finger contact with the non-vibrating case is essential to keep the vibrations from the button localized to the 5 mm circular button area.  Depressing the button fully also affords a secondary function of providing the required 0.50 mm preload indentation of the button into the user’s skin as called for in Tass specifications.  Finally, if the button is not fully depressed, the button’s internal flange may come in contact with the ceiling of the internal cavity and limit the intended vibrations. 
![8 - too loose](https://github.com/user-attachments/assets/61dd849d-4d7c-4aaa-b9ae-789d6f380419)
- This all sounds very complicated, but if tightness of the glove fingertip fit is simply adjusted so the user can feel contact with the top of the case in the complete area surrounding the button, all the details will take care of themselves.  If the fit is too loose, it can be tightened using elastic sports ankle wrap or Velcro straps around the fingertips.  Finding the proper size glove is key if builders seek to avoid the need for tightening straps.  We have recently been experimenting using stretchy fabric gloves from Lowes that fit more snugly without providing too much pressure.

# 10) I MADE A SET THAT WAS TOO TIGHT
When fitting gloves, a user must also take care not to get the fit so tight that blood circulation is impeded.  This issue has not come up in any user feedback, but did with me when I made the glove prototype shown below with very tight fitting fingers in order to achieve maximum dexterity.  It seemed to work at first, but after an hour of therapy, my fingertips would start throbbing due to the impeded circulation.  The key is to find a set of gloves where the tactors fit snuggly in fingertips, but not too tight.  (As I will show next, some users have avoided this challenge by redesigning their gloves to make the fit easier to achieve at the expense of aesthetic appearance and ease of putting on). 
![9 too tight](https://github.com/user-attachments/assets/5cd06ec3-d2e7-42b4-a049-b78d7d649029)

# 11) ELEGANT CUSTOM DESIGN FROM A BB USER FOR FINGERTIPS
- Here is a very detailed design from one DIY builder who adapted our BB glove design to use custom finger cots tailored to be precisely adjustable with Velcro to the length and diameter of each of the user’s fingers:
- https://github.com/MDBalen/PD-Glove-Design/blob/main/Tactor%20archery%20glove%20housing%20construction%20final.pdf
- While this custom design requires some additional work to make the finger cots, it elegantly avoids the need for builders to bring a tactor to the glove store to try out the fit of numerous gloves to get a perfect fit.   
![11 user fingers 2](https://github.com/user-attachments/assets/e83a945f-6d16-4c77-abf4-50a53765dbb2)
![11 user fingers assemby](https://github.com/user-attachments/assets/502624f7-95df-46a0-8a56-0c68439e4f5a)

# 12) SOME BUILDERS ARE MAKING GLOVES WITHOUT GLOVES
- Some builders who wanted to forgo the considerable hassle of fitting the tactors into glove fingertips, have connected tactors to fingers in novel ways.  
- Such arrangements make the apparatus harder to put on and off, and create limits to dexterity, but reduce building effort without compromising therapy efficacy.
- ![12 no glove small 5](https://github.com/user-attachments/assets/11a10ebe-f44b-4838-a60b-28cb5c10316b)
![12 no glove small 2](https://github.com/user-attachments/assets/f1eb4e5b-a2a4-4d60-88b2-c661fab77662)
- ![12 no glove small 3](https://github.com/user-attachments/assets/f5bc16a5-d9cb-4e2e-bea4-45f03a4ba3eb)

# 13) DEALING WITH A JAMMED BUTTON  
- If the spring inside the tactor is not centered under the button flange, the off-center force from the spring can cause the button to become lodged sideways in the button hole of the case.  If this happens, the user will feel greatly reduced vibrations since the button’s motion is impeded. 
- If a tactor develops this problem, the button can usually be freed up by slapping the side of the case on a table top.  To keep the jam from reoccurring, the button must be taken apart and reassembled with the spring properly centered under the button flange.  (Note that we have found that the springs do not “wander” from their positions inside the case once in place, even though they are not glued.)
![13 Jammed Button](https://github.com/user-attachments/assets/fb0d0a34-cad8-4883-a86e-3212b762b702)

# 14)  AMPLITUDE NEEDS TO BE SET LOWER
- A number of users who have changed from foam tactors to our spring tactors have commented that the buzzes feel much more point-focused.  This is because the weak tactor springs more effectively decouple the LRA vibration from the case.  However, with less energy going into the case, more energy ends up going into the button, leading to higher amplitude vibrations being transmitted to the fingertip.  
- Tass specifications call for the lowest amplitude that can provide noticeable point-like vibrations.  
- Accordingly, most users will typically need to adjust the right and left default amplitude settings downward during initial set up in order to achieve the smallest amplitude setting that still provides an easily noticeable and localized vibration to the fingertips as called for in Tass specifications.  If amplitude is set too high, efficacy of the therapy may be compromised.
- I use an amplitude setting of 40 and it seems plenty strong
![14 amplitude 40](https://github.com/user-attachments/assets/04557ee5-8053-4977-8bc6-c76c3a2309c6)

# 15) NOTE ABOUT USING AMPLITUDE RANDOMIZATION
- The Blue Buzzah system has an AMPLITUDE RANDOMIZATION feature that can be activated in the defaults file by setting the MIN level lower than the MAX level.  
- We here at the Blue Buzzah development team disagree about whether to use this feature in our own therapy sessions.  I do not use this feature because I feel a need to have a continual level of awareness of whether I am getting the proper vibrational strength from all my buzzers during therapy.  If I have amplitude randomization active and I get accustomed to feeling varying buzz amplitudes on my fingertips, I fear a misaligned fingertip placement that happens as a result of hand movement might go unnoticed.  In other words, I worry that I might mistake a weak buzz from a misaligned tactor for a normal randomized dip in amplitude,  For me, the potential enhancement of therapy afforded by amplitude randomization is outweighed by the danger of compromised therapy that could be caused by a diminished awareness of finger vibrations that may come from having the intentional variability in amplitude.  
- In contrast, my fellow Blue Buzzah team member is less concerned about the potential of an unnoticed misaligned fingertip placement.  Accordingly, he always implements amplitude randomization in his sessions and feels it greatly enhances his therapy efficacy.  In any case, if a user to decides to engage the amplitude randomization feature, they must exercise extra caution to monitor finger vibrations occasionally during therapy to avoid having an unnoticed misaligned tactor placement.  

# 16)  SEEK EXPERT HELP IF YOU ARE NEW TO SOLDERING 
- I worked with a novice builder who had zero knowledge of electronics at the start of the project. I was truly surprised how quickly she was able to quickly master soldering technique to the point she was able to solder better than me!  Here joints looked like they were made by a machine!  
- However, since she had no basic understanding of electronics, she often made rookie errors that would have ended up causing problems if I had not been checking on her work from time to time.  For example, since she did not initially understand why wires have rubber insulation, she was initially careless about leaving long lengths of exposed wire near her solder joints.  
- Another concern for absolute electronics beginners attempting to build their own gloves is that they will have difficulties troubleshooting what is wrong if things don’t initially work when they turn their circuits on the first time.  
- So, for builders who have never tinkered with electronics, it would probably be best to hire a technician to do the electronics assembly which is very straightforward for someone with a bit of experience.  At the very least, someone new to electronics should take time to watch a YouTube video on beginner electronics and practice soldering a bit before jumping into this project.   

# 17)  USING AN APPLE COMPUTER TO FORMAT FEATHER MODULES
In one instance, an Apple computer user experienced problems while formatting a Feather module using an Apple computer (instead of a PC computer).   In this case the Feather modules would not properly format using the Apple computer.  The problem went away when the user switched to using a PC to format the Feathers.  This may be an isolated instance related to this particular Apple computer since one member of our Blue Buzzah team routinely uses a Mac to format his Feather modules.  I have only used a PC and never had any issues. 

# 18) RECOMMENDATION CHANGE: INSTALL SOCKETS ON PCB 
- This note makes no difference if you have already assembled your electronics since the original design works fine.  However, if you are starting a new build, you can make your box about 10% shorter if you adopt this change.  Many users would not notice this small difference in height.
- In our original design, we recommended mounting the hollow header sockets to the bottom of the Feather module, with the regular PCB headers mounted on the PCB board.  We now realize that this configuration leaves the long pins of the regular headers going into the sockets, causing about 2 mm of unneeded height to the Feather since the long pins bottom out in the sockets.  
- In recent set ups, we have switched to installing the regular headers on the Feather module with short pins sticking down toward the PCB.  
- By mounting the sockets on the PCB, the short pins of the headers end up mating perfectly with the sockets.  
- To avoid confusion, I have not posted the 3D print of the shortened lid that takes advantage of the 2 mm height savings.  However, I would be happy to provide the STL for the shortened lid upon request.  
 ![18 sock rec](https://github.com/user-attachments/assets/576275b1-9360-4c27-ac55-a901415c1573)

# 19)  TENDONITIS REPORT FROM EXCEEDING 2 HOUR SESSIONS    
- This usage note comes from this author’s own general experience with glove therapy and is not related to the Blue Buzzah specifically.
- Upon wondering if longer sessions would lead to better results with tremor, I decided to try doubling the length of one buzz session to 4 hours.  Dr. Tass recommendations call for 2 hour sessions.
- This turned out to be a very bad idea!!!  My initial results were immediately amazing – no tremor after my first evening session which lasted into the next morning!!!  I then continued the next 3 days to buzz 2 hours in the morning, then 4 hours in the evenings.  
- After only 3 days of extended therapy sessions, I noticed I was getting symptoms of trigger finger and tendonitis in ALL 8 buzz fingers.  I immediately stopped buzzing to let my hands recover.  For the first time in almost 2 years, I went 4 days with no vibrating glove therapy.  All my non-tremor symptoms which had been suppressed by the therapy happily remained unaffected by the pause, but I could immediately tell I was getting a bit more tremor without my glove therapy.  
-  After the 4 days with no therapy, my tremor started to get much worse so I started back on my glove therapy using only 1 hour sessions since my tendonitis had not healed.  Adjusting my therapy in this way, all my fingers eventually healed except my middle finger on my left hand which went into complete trigger finger.  I made a special glove that only buzzes on my left thumb, index finger, and pinky which I continue to use now, 10 weeks later.   
   
# 20)  RIGHT AND LEFT DEFAULTS FILES MUST BE IDENTICAL
- I don’t know if any other user has had this problem, but I once changed the defaults settings on one glove and forgot to make identical changes to the defaults settings on the other glove as is currently required by our system.  
- The gloves then behaved erratically and would not maintain sync.  (In other words, the slave glove kept stopping during therapy).  It took me quite some time to figure out that the gloves were having trouble because I had their defaults files set differently.  

# 21)  RARE BLUETOOTH INTERFERENCE PROBLEMS REPORTED
- I have occasionally experienced Bluetooth interference during therapy while using my iphone outdoors.  For me, this has only happened when I was hiking in an area where cell reception was poor (presumably because the iphone increases antenna gain in this circumstance).  
- The problem was also reported once by a user inside a house who was using an ipad during therapy.  
- This issue is on our to-do list to fix.  But, until this issue is resolved, be aware that you may lose sync if you are using a Bluetooth device near your gloves during therapy.  If this happens, simply discontinue using your phone during therapy and restart the gloves. 

# 22)  START BOTH GLOVES TOGETHER TO AVOID TIMEOUT ERROR
- We have had two users who thought their gloves were malfunctioning because they kept going into red light mode. 
-  In both cases, the problem turned out to be that they were simply taking too long to turn on the second glove after turning on the first.  
-  Both gloves need to start within 2 seconds.
-  To avoid this timeout error, simply turn on each glove at the same time before putting the gloves on

# 23) HOW TO PURCHASE SPRINGS INSTEAD OF WINDING DIY 
- The biggest challenge for some users has been making the tactor springs out of 0.012” guitar wire.  The winding technique requires some practice to consistently obtain springs with the proper coil pitch.  
- ![20 winding springs](https://github.com/user-attachments/assets/a83d4293-8e24-41a7-880f-244ee131c0d1)
- Happliy, a user in Germany found a set of 10 springs with the proper specifications can be purchased inexpensively on the German Amazon site: https://www.amazon.de/dp/B0DHCP9JJY .  Unfortunately, these German springs are not available in most locations around the world.
- ![20 guny](https://github.com/user-attachments/assets/8773cdc5-98af-4789-b6e8-5e7abb10d57a)
- Particularly, all springs available in the US-Amazon of the proper specifications are made of thicker wire and are much too stiff.  
![20 many springs](https://github.com/user-attachments/assets/bc57dd80-c67d-43e2-ba80-df2d48e7e842)
- Alternatively, as mentioned in our Tactor Design PDF:
- https://github.com/TactileDesign/DIY-Vibrating-Parkinsons-Glove/blob/main/Design%20Considerations%20for%20LRA%20Tactors.pdf , 
- there are suppliers online such as https://www.thespringstore.com/ who advertise having 70 trillion springs available.  Unfortunately, 99.999% of their springs are only available by special order and are outrageously priced at $4 -$10 per spring!  Ordering a special order set of 8 springs like this could cost $50 to $100.  
- However, users might obtain springs cheaper by purchasing a long single 100-120 mm spring made from diameter 0.012 inch wire, then cut it down to make the eight 11 mm length springs needed in our glove design.  If you decide to special order springs from an online site, make sure you order them with the proper specifications.  Below is a rough guide for users attempting to purchase springs.  (If anyone orders springs in this way, please let us know what kind of results you obtained with your purchase.)
- ![20 table](https://github.com/user-attachments/assets/5be15252-0b7b-49e2-80c2-fd7d90b1b531)

# 24) GET A SPARE BATTERY
- We have observed two new Adafruit batteries that stopped working within the first few hours of use, one in our own use and one from another DIY builder.  Otherwise, all other batteries we know of have continued to function perfectly, some now with over 9 months of 4-hour daily use.  
- Builders might consider ordering an extra battery to use as a spare.  This id the only battery we know of that is designed to fit under the feather module.  The feather module has internal circuitry to regulate the charging.
- One charge provides for more than 10 hours of buzzing.  They are supposued to last 500 charge cycles, which corresponds to 2-3 years of charging every other day.
- https://cdn-shop.adafruit.com/product-files/3898/3898_specsheet_LP801735_400mAh_3.7V_20161129.pdf
![battery](https://github.com/user-attachments/assets/1882e7d9-a641-41d0-85c5-c7685196e25a)



