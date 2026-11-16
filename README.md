# BlueBuzzah Gloves (v2)

NOTICE: this repository has been archived as of 15-Nov-2026 and is no longer being maintained.
- Please visit https://github.com/BlueBuzzah/BlueBuzzah.com for follow up developments.

The BlueBuzzah Gloves system is an open-source, DIY platform inspired directly by the groundbreaking vibrotactile Coordinated Reset (vCR) research led by Dr. Peter Tass of Stanford University, and others.

An overview of the build process can be found in the attached video:
(https://www.youtube.com/watch?v=fcnbQDe73uA)

![pic small 2](https://github.com/user-attachments/assets/20ace566-87f9-4440-a684-799c48798668)  

## About the Project

The BlueBuzzah Gloves project was developed by an informal group of "citizen research" collaborators ("BlueBuzzah Partners") focused on advancing access to open-source DIY tools for people with Parkinson's.
- It is intended to be used as an experimental educational platform only.
- The design is inspired by published research on vibrotactile coordinated reset stimulation. That research used its own devices, settings and protocols, with participants under medical supervision.
- BlueBuzzah is not affiliated with, sponsored by or endorsed by Stanford University, the Tass Lab or any other institution, researcher or company.
- Nothing on this site or in the apps claims that a BlueBuzzah device will produce the same results. Everyone responds differently, and there is no guarantee of any outcome.
- Nothing here is medical advice. Do not stop or change prescribed medication, DBS settings or any other treatment because of something you read here or did with a device. Talk to your clinician.

## Features
- Wireless Bluetooth BLE-synchronized vibrotactile stimulation
- Electronics can be optionally paired with sevearal, LRA-based, open-source glove designs
- Flexible, customize-able coordinated reset pattern and simulation generation
- Highly precise  left <--> right glove synchronization
- Innovative LRA tactor design
- Up to 8+ hours on a single charge
- Built upon:
  - Adafruit hardware @ https://www.adafruit.com/
  - Adafruit CircuitPython libraries @ https://github.com/adafruit/circuitpython
  - Coordinated reset CircuitPython software from the Buzzah project: https://github.com/kriswilk/buzzah

## Project Structure
- 3D PRINTS - STL design files for tactor housings and enclosures
- BUILD DOCUMENTATION PDFs - "how to build the gloves" documentation
- FILES FOR ORDERING PCB - PCB layout files
- FILES FOR PREPARING PCB - all CircuitPython code files
- `LICENSE` – MIT and GPL license texts, and custom hardware license
- `ATTRIBUTION.md` – Contributors and references
- README.md - Project overview

## Disclaimers
This project and all its contents in this repository are not FDA-approved and are not intended for clinical use.  
All files are provided for personal use only and "as-is" with no warranty or implied support.  
BlueBuzzah devices are not FDA cleared or approved medical devices and not intended to diagnose, treat, cure, mitigate, or prevent any disease. 
The information provided through BlueBuzzah is for experimental educational purposes only and not a substitute for professional medical advice, diagnosis, or treatment.
Unauthorized cloning or redistribution of this project for commercial use is prohibited.

Important: People with implanted electrodes from deep brain stimulation (DBS), heart pacemakers, or other internal electronic devices should take special precautions around all electronic devices, including BlueBuzzah. Consult your physician before use.

## No warranty and limits on liability
To the extent the law allows, the BlueBuzzah materials are provided "as is" and "as available", with no warranty of any kind, including no implied warranty of merchantability, fitness for a particular purpose or non-infringement. To the extent the law allows, BlueBuzzah Partners and the volunteers who contribute to the project are not liable for any indirect, incidental, special, consequential or punitive damages, or for any loss of data, injury or other loss, arising from the BlueBuzzah materials or from any device built from them.
Some laws do not allow these exclusions. Nothing in these terms limits any right or liability that the law does not let us limit.

You build and use these devices and software at your own risk.
The developers, contributors, and documentation authors assume no liability for any injury, damage, or other consequences resulting from the construction or use of these devices and software.
Specific outcomes from the devices and software are not specified.
By proceeding with building devices as described by the documentation herein, you acknowledge that you understand and accept these risks.

## Safety
The devices described in this repository contain electronic components, including lithium batteries.
Improper assembly or use could result in electrical shock, fire, or burns.
Follow all safety precautions when handling electronic components and tools.
Use only the specified components from trusted suppliers

## Attribution
See `ATTRIBUTION.md` for contributor credits and scientific references.

## Multiple License Summary
This project uses multiple licenses: 

### Software
- Most files: [MIT License](LICENSE/MIT.txt)
- `main_program_VCR.py`: [GNU GPL v3.0](LICENSE/GPL-3.0.txt)

### Hardware
- All PCB, enclosure, and glove design files:
- https://github.com/PWPInnovator898/BlueBuzzah-Gloves/blob/main/LICENSE/Hardware-License

## Changes to these terms
We may update these terms. Using the repository website after a change means you accept these terms.
