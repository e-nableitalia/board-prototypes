# enable-it Board Prototypes - Second iteration

**This project is part of e-Nable.it Bionic Platform**

An open-source project for developing prosthetic and assistive devices through frugal innovation, designed to be part of e-Nable's open-source prosthetics. The project focuses on building electronic solutions that enable mechanical devices to achieve advanced functionalities, enhancing the community's designs with sophisticated, human-integrated electronic control while maintaining simplicity, affordability, and accessibility.

This project is developed and maintained by the volunteers of the e-Nable Italia community. Our group consists of passionate individuals, including biomedical engineers, mechatronics engineers, and makers, who collaborate to create innovative and accessible solutions. Through our collective efforts, we aim to empower users with open-source, affordable, and customizable assistive devices.

Additional details and information about the **e-nable.it Bionic Platform** can be found in [e-nable.it Bionic Plaform Wiki](https://dev.e-nableitalia.it/wiki/spaces/enableit/pages/2195549/e-Nable.it+bionic+platform).

# Project roadmap

The project unfolds in three development iterations, each aimed at validating, prototyping, and engineering innovative solutions for low-cost bionic devices.

1. Ideas Validation
The first phase involves conducting experiments and tests to validate initial ideas. This phase focuses on identifying the most promising solutions, exploring various options for controlling actuators and sensors, and collecting data to establish guidelines for the prototype.

2. Prototyping & Custom Solutions
During the prototyping phase, custom solutions are developed using commercial components integrated with specialized electronic boards. The most promising ideas are implemented into physical prototypes to validate architectural and structural concepts. The focus is on simplicity and reliability, ensuring the solutions can be easily replicated and adapted for various bionic devices.

3. Frugal Innovation Engineering
The final phase focuses on engineering the solutions based on frugal innovation principles. Prototypes are optimized to make them accessible, scalable, and practical, with a strong emphasis on cost-effectiveness and real-world applicability. The engineering process also involves creating an open-source hardware platform that enables the creation of modular systems easily combined to build bionic devices.

This repository relates to Iteration #2.

The objective of this iteration is to develop the prototypes useful to validate ideas and concepts developed in the previous step.

**The boards developed in this iteration are only for technological validation and are not designed for real use.**

## Boards
### Controllers - controller boards with a general purpose CPU, exposing a standard bus interface (see B2BCB specifications)
* ESP32 Wroom board Rev. B - ESP32 S3 based 

### Debug - debug, testing boards
* Debug Board Rev. A, mating board useful for debug and testing purposes

## Project directory layout
- docs, contains general documents
- schematics,  contains schematics in PDF format
- build, contains CAM Output files for board production
- EAGLE, contains project EAGLE files

## Project updates
220913 - repo init, added project doc & rev. 0.9 of ESP32 controller board

220922 - added debug board, added Rev. B of control board

220927 - updated debug board to Rev. A (added bottom connectors to allow tests of stacked boards)

230305 - added EMG Module - Rev B, changed name to enable-it

## KNOWN ISSUES

- ESP32 Controller board flash programming problem, rework required to fix this issue 
- Power connectors are not correctly aligned in all the boards, rework required to fix this issue
- Wrong height of 40pin connectors (4mm instead of 3mm)
- EMG Module power issue: short circuitt between AVDD & AVSS (PS$32 AVSS connected to V+ instead of V-)

## Authors

Alberto Navatta - alberto@e-nableitalia.it / alberto.navatta@gmail.com

e-Nable Italia - info@e-nableitalia.it 

Check for further information, updates and information on this and other e-Nable Italia’s projects on our website: [https://e-nableitalia.it/](https://e-nableitalia.it/)

## License

This material is released under *Creative Commons - Attribution - Non-Commercial - Share Alike license*

## LIMITATION OF LIABILITY.
UNDER NO CIRCUMSTANCES AND UNDER NO LEGAL THEORY, WHETHER TORT (INCLUDING NEGLIGENCE), CONTRACT, OR OTHERWISE, SHALL YOU, THE INITIAL DEVELOPER, ANY OTHER CONTRIBUTOR, OR ANY DISTRIBUTOR OF COVERED CODE, OR ANY SUPPLIER OF ANY OF SUCH PARTIES, BE LIABLE TO ANY PERSON FOR ANY INDIRECT, SPECIAL, INCIDENTAL, OR CONSEQUENTIAL DAMAGES OF ANY CHARACTER INCLUDING, WITHOUT LIMITATION, DAMAGES FOR LOSS OF GOODWILL, WORK STOPPAGE, COMPUTER FAILURE OR MALFUNCTION, OR ANY AND ALL OTHER COMMERCIAL DAMAGES OR LOSSES, EVEN IF SUCH PARTY SHALL HAVE BEEN INFORMED OF THE POSSIBILITY OF SUCH DAMAGES. THIS LIMITATION OF LIABILITY SHALL NOT APPLY TO LIABILITY FOR DEATH OR PERSONAL INJURY RESULTING FROM SUCH PARTY'S NEGLIGENCE TO THE EXTENT APPLICABLE LAW PROHIBITS SUCH LIMITATION. SOME JURISDICTIONS DO NOT ALLOW THE EXCLUSION OR LIMITATION OF INCIDENTAL OR CONSEQUENTIAL DAMAGES, SO THIS EXCLUSION AND LIMITATION MAY NOT APPLY TO YOU.
