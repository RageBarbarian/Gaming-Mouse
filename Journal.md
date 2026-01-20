# DAY 1 12/16/25: 3D design first draft
MEMBERS: VARUN, ANIRV; AGNI WAS NOT AVAILABLE
TIME: 6:30-7:30pm
WHAT WAS ACCOMPLISHED: We have been able to develop the prototype design of our advanced gaming mouse. We added the functions decided on including the arrows keys and space bar along with the normal functions of a mouse. We designed a few parts in OnShape like the base of our mouse with an asthetic design and with the keys needed for WASD. We have also been able to go on KiCAD and download one of the necessary libraries needed for our PCB: the microcontroller. We have decided that our micrcontroller shall be the Seeed XIAO ESP32C3 chip due to its small structure and also being fast + reliable. It will fit into our 3D mouse base nicely but we might decide on something else otherwise. Our mouse PCB will be mainly inspired by the Bambu lab mouse kit. 
# Mouse Draft:
<img width="773" height="439" alt="image" src="https://github.com/user-attachments/assets/d33d1452-4b21-4efa-9d54-5a2027f51433" />

# DAY 2 12/23/25: SCRAPED INITIAL IDEA AND MADE THE 3D DESIGN(CASE) AS WELL AS LISTING THE ELECTRONIC/CIRCUIT PARTS WE NEED TO PUT INTO KiCAD
MEMBERS: VARUN, ANIRV, AGNI
TIME: 4:30-6:30
WHAT WAS ACCOMPLISHED: We scraped the initial idea and decided that most of the circuit components we are using in our mouse is going to be from the official Bambu Lab mouse kit. AGNI found these parts in the Bambu kit and listed them so we can later download them into KiCAD for our final PCB. ANIRV and VARUN worked on the journal as well as the 3D case that maps around the circuits. We are going to design the case through Onshape CAD. Our idea is to collect all the necessary components in the Bambu Lab mouse kit needed for a simple mouse and incorporate 4 seperate push buttons into it for WASD, so something like a mouse and keyboard in one. 
# Mouse Kit:
<img width="1600" height="1600" alt="image" src="https://github.com/user-attachments/assets/31a5f33f-94fe-4e39-a7a2-2fd0ddadb419" />

# DAY 3 12/29/25: FINALIZE A PLAN
MEMBERS: VARUN, ANIRV, AGNI
TIME: 4:00-7:00
WHAT WAS ACCOMPLISHED: We scarped the second idea and came up with a brand new one. We came up with the initial idea of combining a push-button keyboard with a mouse to handle WASD movement inputs. We decided that the four push buttons would be physically integrated into the mouse itself for ease of use and better ergonomics. However, due to space, wiring, and complexity constraints, the microcontroller could not be placed inside the mouse. Although we did not like the idea of having a separate external module at first, we compromised by designing a small module that would house the microcontroller and connect to the mouse via USB. This day was focused on brainstorming, discussing trade-offs, and finalizing the core concept so implementation could begin later.

# DAY 4 12/31/25: 
MEMBERS: VARUN, ANIRV, AGNI
TIME: 4:00-6:00
WHAT WAS ACCOMPLISHED: We made a new draft in OneShape with all the new componets added. First, we tested if the 4 pin buttons actually worked and they gave an outbut. After that, we tried to test if the bluetooth connection for the ESP32 was working and we got a Keyboard Output. (EX: the microcontroller typed "w" multiple times, proving there was a connection.)
This was so that we would have the code preuploaded or pre-ready for the 4 push buttons we will later incorporate into the whole mouse design for the WASD keys.
We had later found a breakthrough and had gotten our code so that if we press any of the 4 four pin push buttons, the computer will produce an output that matches the WASD formation. Although the design works, there were still some problems like the fact that a button is not consistant or the output comes differently. We had improved the code later after a few itterations and made it more reliable. 


![IMG_1608 1](https://github.com/user-attachments/assets/cc8f2461-88ae-4baf-ae4f-069e39391c6f)
![IMG_1609 1](https://github.com/user-attachments/assets/106fabf1-e9f5-492c-8c6d-ab7b2a018f58)

# DAY 5 1/1/26: 
MEMBERS: VARUN, ANIRV, AGNI
TIME: 4:00-6:00
WHAT WAS ACCOMPLISHED: We mainly focused on cleaning up and finalizing our project journal. We went back through all previous days and polished the wording, fixed formatting issues, and made sure everything was clearly explained and consistent. We also added a proper list of parts (BOM), including the components taken from the Bambu Lab mouse kit and the additional push buttons and microcontroller-related parts. Most of the time was spent updating, organizing, and reviewing the journal to make sure it accurately reflects our progress and design decisions so far.

<img width="320" height="378" alt="Screenshot 2026-01-04 173712" src="https://github.com/user-attachments/assets/61e1715e-db23-42cc-ab88-ec0192d8c90d" />

# This was our initial Microcontroller, the SEEED XIAO, but we did some research and found out that it does not support the number of pins we need for the push buttons and other components.

<img width="357" height="335" alt="Screenshot 2026-01-04 173534" src="https://github.com/user-attachments/assets/5c6d90a1-6099-4898-a99e-c2878ba1c801" />

# This is our new Microcontroller, an ESP32 devkit C, and this can handle 10+ push buttons and supports all our other functions.

<img width="302" height="308" alt="Screenshot 2026-01-04 173337" src="https://github.com/user-attachments/assets/21575f86-ff5b-42b2-88de-c104ed322a0c" />

# This are the push buttons that we used. They are effective and useful for the WASD components on our mouse

<img width="326" height="339" alt="Screenshot 2026-01-04 173211" src="https://github.com/user-attachments/assets/30ed0631-a39e-4631-96a9-a5f868ee0c46" />

# The Bambu Lab Kit came with an optical tracking sensor but we could not connect it to our ESP32. Thus, we decided to buy a new lazer sensor, the PMW3901.

<img width="567" height="321" alt="Screenshot 2026-01-04 173017" src="https://github.com/user-attachments/assets/21f35678-db3b-422f-9029-360cdc7419bc" />
<img width="491" height="292" alt="Screenshot 2026-01-04 173007" src="https://github.com/user-attachments/assets/13bc5b1a-9223-4e64-8b7c-9a87a4dedbaa" />
<img width="520" height="355" alt="Screenshot 2026-01-04 172955" src="https://github.com/user-attachments/assets/d6c45c47-ca55-45e2-9e70-d948076eb2ad" />

# DAY 6 1/7/26:
MEMBERS: VARUN, ANIRV, AGNI
TIME: 3:00-5:00
WHAT WAS ACCOMPLISHED: As a group, we went over all the parts what what each one of them does. We also coded the basics of the mouse and the functions of the buttons from the Bambu Lab Kit. AGNI and VARUN tried to get a head start on the optical sensor component by trying to code it and see if it functions properly. Ufortunately we did not have enough time to code the sensor and have it actually working but we will in one of the next meetings. 

After the meeting VARUN took all the components we are using in our mouse and donwloaded their symbols into KiCAD for the final schematic:

<img width="994" height="590" alt="Screenshot 2026-01-16 214732" src="https://github.com/user-attachments/assets/5cfb684b-fa13-4dd6-ab9b-b3cb365ee5fe" />


We decided on making the schematic not so that we will buy a pcb board for the mouse, but for documentation and a guide for soldering later on. Instead of using a physical PCB for the mouse, we decided we will solder wires to each of the components from the ESP32 for more flexibility in the mouse. While soldering we will use the wiring in the schematic to succesfully connect all components to the ESP32. For now we will solder all components except the PMW3901 optical sensor. This is becuase we are unsure of it to  tally working due to how we were trying to code it the past meeting and failed. We want to be safe so we will be connecting eveyrything but that in the next meeting or Day 7. 

# DAY 7 1/17/26
MEMBERS: ANIRV, AGNI, VARUN
TIME: 4:00-7:00
WHAT WAS ACCOMPLISHED: Today we soldered all the the parts of the Bambu Lab Mouse Kit to our ESP32. ANIRV and AGNI learned how to do it in the proccess amd VARUN coached them, along with his dad. We took many safety precautions, including masks and goggles. This is to stop the entry of harmful substances to the body, including fumes from the solder. However, we wasted many buttons while practicing how to wire them up. We also had a major breakthrough in the coding of the optical sensor and managed to make it work.

