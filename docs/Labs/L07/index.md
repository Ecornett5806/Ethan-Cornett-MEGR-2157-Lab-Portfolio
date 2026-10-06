# A7 Linkage Mechanism:


## Research:

Patent 1: Linkage Mechanism, Robotic Finger and Robot
https://patents.google.com/patent/US20230415355A1/en (Linkage mechanism, robotic finger and robot)

Patent: US20230415355A1
Inventor(s): Zhongkui Huang, Hongyu Ding, Xixiang Luo, Ming Chen, and Wenhua Fan
Assignee: UBTECH Robotics Corp.
Publication date: December 28, 2023

How it works:

This patent describes a robotic finger that uses a four-bar linkage to create controlled bending and straightening motion. The mechanism consists of a base, two main finger links, and a connecting link. A linear actuator pushes a transmission member, which causes the first link to rotate around the base. The connecting link transfers this motion to the second link, causing the finger to flex. An elastic member helps return the finger toward its original position.

The important idea is that the four links and four pivot connections constrain the motion. Instead of having the actuator directly control every finger joint, the linkage creates the desired finger motion mechanically. The patent also describes the mechanism as allowing both active flexion/extension and passive movement when an outside force is applied.

<img width="300" height="600" alt="US20230415355A1-20231228-D00001" src="https://github.com/user-attachments/assets/297f97e7-22e3-4ca6-bdbf-23e4f12ad814" />

Industry 1 — Robotics and Automation

This mechanism can be used in industrial and service robots that need controlled finger or gripper motion. A four-bar linkage can produce repeatable motion while reducing the number of independently controlled joints. Four-bar linkages are also used in robotic hands because they can provide predictable finger trajectories and mechanical coupling between joints.

Industry 2 — Medical Devices and Prosthetics

The same principle can be used in prosthetic hands and other assistive devices. A 3D-printed robotic hand study used four-bar linkages to reproduce finger movement and reported that the mechanism could be fabricated using 3D printing. Four-bar mechanisms have also been studied for prosthetic fingers because they can provide controlled flexion and extension with relatively simple mechanical structures.


Patent 2: Four-Bar Linkage Mechanism for a Tillage Machine

https://patents.google.com/patent/DE102022111301A1/en (Four-bar linkage mechanism for a tillage machine)

Patent: DE102022111301A1
Inventor: Paul Treffler
Priority date: May 7, 2021
Publication: 2022

How it works

This patent describes a four-bar guide mechanism used to move tools on agricultural equipment. The mechanism has four links connected by four joints. One link is attached to the machine frame while another link carries the agricultural tool. As the linkage moves, the tool follows a controlled path rather than simply moving straight up or down.

The patent describes several possible configurations and motions. The tool can be raised and moved into an excavation or transport position while maintaining a desired orientation. Different tools can be attached to the linkage, including soil-working and weed-control tools.

<img width="200" height="400" alt="DE102022111301A1_0003" src="https://github.com/user-attachments/assets/2ff1d358-f9d6-4ec2-88b7-2c91689f8c81" />

Industry 1 — Agriculture

The most obvious application is agricultural equipment. The patented mechanism can position tools for tillage, cultivation, and weed control while controlling how the tool moves relative to the soil. A 2022 engineering study also investigated optimized four-bar mechanisms specifically for mechanical weed control, showing that four-bar mechanisms can be designed to produce useful agricultural tool paths.

Industry 2 — Construction and Heavy Equipment

A similar linkage concept could be applied to construction equipment where an attachment needs to follow a controlled path. Examples include positioning small digging, grading, or material-handling attachments. The same basic engineering principle applies: fixed pivot locations and link lengths constrain the output tool to a predictable motion.

Sources: 

https://patents.google.com/patent/DE102022111301A1/en (Four-bar linkage mechanism for a tillage machine)

https://patents.google.com/patent/US20230415355A1/en (Linkage mechanism, robotic finger and robot)

https://www.nature.com/articles/s41467-021-27261-0?utm_source=chatgpt.com
[3] Kim, U., et al. “Integrated linkage-driven dexterous anthropomorphic robotic hand.” Nature Communications, 2021. This paper analyzes robotic fingers using four-bar linkages and discusses the kinematics and resulting finger motion.

https://www.nature.com/articles/s41467-021-27261-0?utm

[4] Hosseini, H., Farzad, A., Majeed, F., Hensel, O., & Nasirahmadi, A. “Multi-Objective Optimal Design and Development of a Four-Bar Mechanism for Weed Control.” Machines, 2022. This paper examines a four-bar mechanism specifically for agricultural weed-control applications.

https://www.mdpi.com/2075-1702/10/3/198?utm

## Design

### Purpose

The purpose of this mechanism is to demonstrate the basic idea of how a robotic limb can use multiple connected segments to produce controlled movement. The design was developed as a simplified version of the type of articulated motion used in the robotic finger mechanism described in the referenced patent.

The mechanism uses three 3D-printed segments connected by removable pins. Each joint allows the segments to rotate, while mechanical stops limit the amount of movement. The design was intentionally kept simple so the basic motion of a robotic limb could be demonstrated without adding unnecessary complexity.

### Components: 

### Components

| Component | Function | Material | Manufacturing |
|---|---|---|---|
| Base segment | Supports the mechanism and connects to the first moving joint | PLA | Printed |
| Middle segment | Rotates relative to the base segment | PLA | Printed |
| End segment | Rotates relative to the middle segment | PLA | Printed |
| Flathead Printed Screw | Connects the segments and allows rotational movement | PETG | Printed |

1. Three segments instead of a more complex multi-link system

I chose three because the goal was to demonstrate the basic concept of articulated robotic-limb motion rather than recreate the full patent mechanism.

2. Rounded ends with pin holes

This allows the segments to rotate around the pins while keeping the parts simple to print.

3. Mechanical stops

These limit the rotation of the joints and make the movement controlled rather than allowing the segments to rotate freely.

Images of CAD: 

<img width="850" height="380" alt="Screenshot 2026-10-05 235240" src="https://github.com/user-attachments/assets/3be794b6-911c-4d91-bb4c-5dd61e0f67ee" />

<img width="724" height="256" alt="Screenshot 2026-10-05 235254" src="https://github.com/user-attachments/assets/9fc72c00-7c2b-4ed5-af8e-80acdbf29be6" />

<img width="816" height="540" alt="Screenshot 2026-10-05 235310" src="https://github.com/user-attachments/assets/d09efbff-2751-4226-a6c3-5d016544b9f8" />

<img width="810" height="494" alt="Screenshot 2026-10-05 235317" src="https://github.com/user-attachments/assets/f6d1d860-f142-4d45-9aa8-57c33a118118" />

<img width="874" height="796" alt="Screenshot 2026-10-05 235403" src="https://github.com/user-attachments/assets/3689bb93-a695-4496-b2a8-9cdf5372a47e" />

<img width="778" height="258" alt="Screenshot 2026-10-05 235415" src="https://github.com/user-attachments/assets/5a471693-eb98-43f9-abd4-390aeb845518" />

<img width="838" height="504" alt="Screenshot 2026-10-05 235441" src="https://github.com/user-attachments/assets/238a96f4-0a4f-48b4-9368-18e57f3e05f2" />

<img width="998" height="860" alt="Screenshot 2026-10-06 104351" src="https://github.com/user-attachments/assets/2d856820-cb80-433c-8d9d-320063f2ba70" />


Final Assembly: 

<img width="696" height="686" alt="Screenshot 2026-10-06 000736" src="https://github.com/user-attachments/assets/386eedff-5040-4956-a0ff-cbfba1b9c24a" />



## 3D Print

### Purpose

The purpose of this mechanism is to demonstrate the basic idea of how a robotic limb can use multiple connected segments to produce controlled movement. The design was inspired by the basic articulated motion of the robotic finger mechanism described in the referenced patent. The mechanism was intentionally simplified to three 3D-printed segments so that the basic motion could be demonstrated without unnecessary complexity.

The three segments are connected with removable pins. The pins allow the segments to rotate relative to each other, while mechanical stops limit the range of motion at each joint.


### Components

Base segment- Supports the mechanism and connects to the first moving segment	PLA	Printed
Middle segment- Rotates relative to the base segment	PLA	Printed
End segment- Rotates relative to the middle segment	PLA	Printed
Joint pin- Connect the segments and allow rotational movement	PETG	Printed

Tolerances

The main moving interfaces in the mechanism are the two pin-in-hole joints. The PETG pins need enough clearance inside the PLA holes to allow the segments to rotate without excessive friction.

The initial pin diameter was designed as 3.0 mm. The holes were designed slightly larger than the pins to provide clearance. A starting hole diameter of 3.2 mm provides 0.2 mm of diametral clearance, or 0.1 mm of radial clearance.

The clearance was selected as a starting value and can be verified with a test print. A small test piece with multiple hole sizes can be printed to compare the fit of the 3.0 mm PETG pin. The final hole size will be selected based on which fit allows the joint to rotate while keeping the segments stable.

### Design Decisions

Three-Segment Design

Alternatives considered:

A more complex multi-segment robotic finger
A four-bar linkage
A three-segment articulated limb

Decision: Three-segment articulated limb.

The three-segment design was selected because the goal was to demonstrate the basic motion of a robotic limb rather than reproduce the complete mechanism from the referenced patent. Using three segments reduced the number of parts while still providing multiple rotational joints.

### Rounded Pivot Ends

Alternatives considered:

Fully rectangular ends
Fully cylindrical segments
Rectangular segments with rounded pivot ends

Decision: Rectangular segments with rounded pivot ends.

The rectangular bodies were simple to model and print, while the rounded ends provided material around the pin holes and allowed the segments to rotate around the joints without the corners interfering with each other.

Printed PETG Flathead Pins

### Alternatives considered:

Screws
Metal pins
3D-printed PETG pins

Decision: 3D-printed PETG pins.

PETG pins were selected because they could be printed at the same time as the mechanism and could be removed if the design needed to be modified. Using removable pins also made it possible to assemble the mechanism after printing instead of requiring the joints to be printed as one piece.

### Mechanical Stops

Alternatives considered:

No rotation limit
External stops
Integrated stops

Decision: Integrated mechanical stops.

Mechanical stops were added to control the maximum rotation of each joint. This prevents the segments from rotating beyond the intended range and makes the motion more controlled.

Printed flathead Screw:

<img width="1024" height="2032" alt="IMG_1751" src="https://github.com/user-attachments/assets/488988f7-a347-4016-93bd-fd871c5d3445" />

"Fingertip Joint" 

<img width="1024" height="2032" alt="IMG_1750" src="https://github.com/user-attachments/assets/b56cb932-97ed-4c45-851e-b4554377c83c" />

"Knuckle joint"

<img width="1024" height="2032" alt="IMG_1748" src="https://github.com/user-attachments/assets/1e9bcc6c-c804-4854-bedd-47990f364189" />

"Middle Joint" 

<img width="1024" height="2032" alt="IMG_1749" src="https://github.com/user-attachments/assets/ad049864-d51b-4ec6-9379-abec0168246c" />

Full Printed Assembly: 

<img width="1024" height="2032" alt="IMG_1747" src="https://github.com/user-attachments/assets/e7e03439-ffa4-451c-8083-d21d6868fadc" />


## Lessons Learned:

Time:

The project took approximately 7 hours and 15 minutes from start to finish. I spent about 40 minutes on research, 30 minutes on CAD, 15 minutes on slicing, 3.5 hours printing, 2 hours on post-processing, and 20 minutes on assembly. Printing and post-processing took the most time, while the CAD and slicing stages were relatively short. The total time was close to what I expected, but the project could be completed faster in the future by reducing the size of the mechanism and using smaller screws to reduce print time.

Biggest Mistake:

My biggest mistake was not checking the physical size of the mechanism before completing the CAD model, which caused the final mechanism to be larger than I wanted. I also used the scale feature in PrusaSlicer to change the size instead of going back and modifying the CAD model, and I made the screws larger than necessary, which increased the print time. Another lesson was learning to use a STEP file instead of an STL file when creating images of the model, since the STEP file preserved the rounded geometry better and produced smoother-looking images. I would fix these problems by checking the model against a physical reference before printing, changing dimensions directly in CAD, using smaller screws, and using STEP files when high-quality CAD images are needed.

Tolerances:

The tolerances for the moving joints were applied only to the Flathead Printed Screw diameter and the corresponding hole diameter. The Flathead Printed Screws have a nominal diameter of 10 mm, and a 0.2 mm tolerance was used for the screw diameter and each matching hole diameter. This tolerance was selected to give enough space between the printed parts for the screw to fit into the hole without preventing the joint from moving.

The first print was used to check whether the 0.2 mm tolerance would allow the joints to assemble and rotate. The screws fit into the holes as intended, and the connected segments were able to move without the joints binding. Because the first print worked with this tolerance, no changes were made to the screw or hole diameters for the final version. The final design therefore uses a 10 mm nominal screw diameter with a 0.2 mm tolerance on both the screw diameter and corresponding hole diameter.
