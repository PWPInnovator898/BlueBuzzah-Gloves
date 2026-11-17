# BlueBuzzah Gloves (v2)

NOTICE: RETIRED — BlueBuzzah Gloves (v2)
- The BlueBuzzah Gloves (v2) repository was retired effective November 17, 2026. 
- This repository is archived and retained for historical reference.
- Development, maintenance, and support for v2 have ended. 
- No further bug fixes, security patches, compatibility updates, technical support, or build assistance will be provided for the v2 materials in this repository.
- The archived files may contain unresolved defects or outdated instructions. Their continued availability does not indicate ongoing testing, validation, or support.
- For information about other BlueBuzzah projects and developments, visit [BlueBuzzah Website](https://bluebuzzah.com)
- Other BlueBuzzah projects may have separate support arrangements and do not imply v2 support or compatibility.

The BlueBuzzah Gloves system is an open-source, DIY platform inspired directly by the groundbreaking vibrotactile Coordinated Reset (vCR) research led by Dr. Peter Tass of Stanford University, and others.

An overview of the glove build process can be found in the attached video:
- [Watch Video](https://www.youtube.com/watch?v=fcnbQDe73uA)

![BlueBuzzah Gloves](https://github.com/user-attachments/assets/20ace566-87f9-4440-a684-799c48798668)

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
- Flexible, customize-able coordinated reset pattern and stimulation generation
- Coordinated left <--> right glove synchronization
- Innovative LRA tactor design
- Up to several hours operation on a single charge
- Built upon:
- Adafruit hardware: [Adafruit Industries](https://www.adafruit.com/)
- Adafruit CircuitPython libraries: [Adafruit CircuitPython](https://github.com/adafruit/circuitpython)
- Coordinated reset CircuitPython software from the [Original Buzzah Project](https://github.com/kriswilk/buzzah)

## Project Structure
- 3D PRINTS - STL design files for tactor housings and enclosures
- BUILD DOCUMENTATION PDFs - "how to build the gloves" documentation
- FILES FOR ORDERING PCB - PCB layout files
- FILES FOR PREPARING PCB - all CircuitPython code files
- `LICENSE` – MIT and GPL license texts, and custom hardware license
- `ATTRIBUTION.md` – Contributors and references
- README.md - Project overview

## Disclaimers
BlueBuzzah devices and related software are not FDA cleared or approved medical devices and not intended to diagnose, treat, cure, mitigate, or prevent any disease.
The contents in this repository are not FDA-approved and are not intended for clinical use.  
The information provided through BlueBuzzah is for experimental educational purposes only and not a substitute for professional medical advice, diagnosis, or treatment.

Important: People with implanted electrodes from deep brain stimulation (DBS), heart pacemakers, or other internal electronic devices should take special precautions around all electronic devices, including BlueBuzzah. Consult your physician before use.

All project files are provided “as is,” without warranty or support, subject to their applicable licenses. 
Software permissions and conditions are governed by the MIT or GNU GPL v3.0 license, as identified in the Multiple License Summary below.
The noncommercial restrictions in the custom BlueBuzzah Gloves Hardware License apply only to the hardware design files and related materials covered by that license. They do not apply to software released under the MIT or GNU GPL v3.0 licenses. Consult the applicable license for each component’s permissions, conditions, and restrictions.

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

## Security status
Since BlueBuzzah Gloves v2 is retired and unsupported, no security enhancements or fixes are planned. 
The archived materials are retained for historical and educational reference and should not be relied upon where authenticated device control or guaranteed safe shutdown is required.

## Attribution
See [Attribution](ATTRIBUTION.md) for contributor credits and scientific references.

## Multiple License Summary
This project uses multiple licenses: 

### Software
- **GPL-3.0:** `main_program_VCR.py` and applicable modifications derived from the original Buzzah project.
- **MIT:** Independently licensed software components, where applicable.
- **Third-party libraries:** Subject to their respective upstream licenses.
- Distribution of the combined CircuitPython firmware remains subject to applicable GPL-3.0 requirements.

### CircuitPython Firmware Licensing
- The BlueBuzzah Gloves v2 CircuitPython stimulation firmware was derived from the [Original Buzzah Project](https://github.com/kriswilk/buzzah), licensed under the GNU General Public License version 3.
- BlueBuzzah Partners subsequently developed substantial enhancements, including Bluetooth communication, bilateral synchronization, and additional firmware capabilities.
- See the [Attribution](ATTRIBUTION.md) document for additional details. 

### Hardware
- All PCB, enclosure, and glove design files:
- [Hardware License](https://github.com/PWPInnovator898/BlueBuzzah-Gloves/blob/main/LICENSE/Hardware-License)

## Changes to these terms
We may update these terms. Using the repository website after a change means you accept these terms.
