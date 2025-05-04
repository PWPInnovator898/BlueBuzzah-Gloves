# BlueBuzzah Gloves

The BlueBuzzah Gloves system is an open-source, non-invasive neuromodulation platform inspired directly by the groundbreaking vibrotactile coordinated reset (VCR) therapy research led by Dr. Peter Tass and others.
(https://www.youtube.com/watch?v=fcnbQDe73uA)

![pic small 2](https://github.com/user-attachments/assets/20ace566-87f9-4440-a684-799c48798668)

## About the Project

The BlueBuzzah Gloves project was developed by an informal group of "citizen research" collaborators ("BlueBuzzah Partners") focused on advancing access to open-source DIY tools for people with Parkinson's.
Many people in the extended PD community have active DIY VCR platforms and/or experiments in development.

## Features
- Wireless Bluetooth BLE-synchronized vibrotactile stimulation
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
- `LICENSES/` – MIT and GPL license texts, and custom hardware license
- `ATTRIBUTION.md` – Contributors and references
- README.md - Project overview

## Disclaimer
This project is not FDA-approved and is not intended for clinical use.  
All files are provided for personal use only and "as-is" with no warranty or implied support.  
Hardware design files are released under a custom non-commercial license (see below).

See `ATTRIBUTION.md` for full credits.

## Multiple License Summary

This project uses multiple licenses:

### Software
- Most files: [MIT License](LICENSES/MIT.txt)
- `main_program_VCR.py`: [GNU GPL v3.0](LICENSES/GPL-3.0.txt)

### Hardware
- All PCB, enclosure, and glove design files:
- https://github.com/PWPInnovator898/BlueBuzzah-Gloves/blob/main/LICENSES/Hardware-License

Please refer to `ATTRIBUTION.md` for contributor credits and scientific references.
