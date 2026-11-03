# A10 RC2 Sliding fit 

## Objective
Design and fabricate a pair of parts (a hole/slot feature and a matching shaft/insert feature) that demonstrate an RC 2 sliding fit on a SLA print

## Research: 

An RC 2 sliding fit is commonly used in mechanical assemblies where components need to move while maintaining accurate alignment. One example is a pneumatic cylinder, where a piston moves inside a cylinder bore. The sliding fit allows the piston to travel smoothly while limiting excessive side-to-side movement. Similar fits are used in locating pins, manufacturing fixtures, sliding mechanisms, and adjustable machine components. For this project, the RC 2 fit demonstrates how controlled clearance allows two components to move relative to each other without excessive looseness.

### Research Summary

The selected design is a miniature pneumatic piston and cylinder that demonstrates an RC 2 running and sliding fit. The cylinder has an outer diameter of 6.00 mm and an inner bore diameter of 4.00 mm. The matching piston has a diameter of 3.90 mm.

According to *Machinery's Handbook*, Table 8a, an RC 2 fit uses an H6 tolerance for the hole and a g5 tolerance for the shaft. Since the selected nominal diameter is 4.00 mm (0.1575 in), it falls within the 0.12–0.24 inch size range in the table. The corresponding dimensions are:

| Component | RC 2 dimension limits |
|---|---:|
| Cylinder bore (H6) | 4.00000–4.00762 mm |
| Piston (g5) | 3.99111–3.99619 mm |

These limits produce a theoretical diametral clearance between 0.00381 mm and 0.01651 mm. This small clearance allows the piston to slide while maintaining accurate alignment.

The current CAD model uses a 4.00 mm cylinder bore and a 3.90 mm piston. This gives a designed diametral clearance of 0.10 mm. Although this provides more room for the parts to move, it is larger than the calculated RC 2 clearance range. The dimensions will need to be adjusted if the final parts are expected to meet the specified RC 2 tolerances.

A real-world example of this type of movement is a pneumatic actuator. In a pneumatic cylinder, a piston travels inside a cylinder bore to convert air pressure into linear motion. The sliding fit demonstrates how two components can move relative to each other while maintaining alignment. Actual pneumatic cylinders also use seals to prevent air leakage.

SLA resin printing can introduce dimensional changes during printing, washing, and post-curing. Additional curing can cause slight shrinkage, while excessive washing or uneven curing can cause dimensional changes or warping. To account for these effects, test coupons will be printed and measured before finalizing the CAD dimensions. The measured results will be used to adjust the model and evaluate the actual clearance between the piston and cylinder.

The final fit will be evaluated by measuring both printed components and testing how smoothly the piston moves inside the cylinder. The measured dimensions will be compared with the RC 2 tolerance limits to determine how closely the printed parts match the intended fit.

## CAD: 
Cylinder CAD:
First I made the base where the screw hole would go: and then extruded it by 5 mm

<img width="508" height="380" alt="image" src="https://github.com/user-attachments/assets/9dd088c9-b070-485b-9417-34805abd234f" />

<img width="472" height="396" alt="image" src="https://github.com/user-attachments/assets/a986094b-7067-4dea-a9fc-f0abed7aecdd" />

Then I add a small wall to have as a bade for the cyllinder the pin would go into and extruded it by 4mm:

<img width="648" height="526" alt="image" src="https://github.com/user-attachments/assets/49afa669-64b3-4bb0-a8d4-3d0aa2b4e5f4" />

<img width="1428" height="1080" alt="image" src="https://github.com/user-attachments/assets/0063608a-2030-43a8-bc1e-c74efe11d6f0" />

Then for the cylinder itself I made a 4mm and 6mm diameter circle to give the cylinder some thickness, then extruded it by 7.6mm

<img width="1282" height="794" alt="image" src="https://github.com/user-attachments/assets/ed711b86-b283-4d77-a43d-c409fb707aaa" />

<img width="1178" height="866" alt="image" src="https://github.com/user-attachments/assets/ea16bdde-e527-412f-afbe-8910d7aa52be" />

And finally, I added the screw hole and cut out 5mm of length, so the hole went completely through. 

<img width="900" height="962" alt="image" src="https://github.com/user-attachments/assets/c31230e4-d7ce-496b-81f3-6b15c344808c" />

<img width="994" height="932" alt="image" src="https://github.com/user-attachments/assets/f95cb8f4-6785-457a-bb13-eb824c44a8c9" />

Piston CAD: 
Started by making the diameter of the screw 3.9mm which is slightly smaller than the cyllinder and extruded it 7.6mm  
<img width="572" height="568" alt="image" src="https://github.com/user-attachments/assets/dde46088-1935-4315-b8ec-daa930b37d31" />

<img width="1146" height="770" alt="image" src="https://github.com/user-attachments/assets/0b81137f-5e47-4e5a-ac08-fd79e4044721" />

Then I made the base of the screw by putting a Flat head on the pin with a diameter of 6mm and then extruded it 2mm: 

<img width="1106" height="786" alt="image" src="https://github.com/user-attachments/assets/9f639cb4-eff8-43b7-913b-3763ea9a6bee" />

<img width="988" height="712" alt="image" src="https://github.com/user-attachments/assets/0fe439a3-7d81-4bdd-9bf3-8fbf1453850f" />

## Preprocessing 

Picture of my parts in Preform:

<img width="2560" height="1416" alt="image" src="https://github.com/user-attachments/assets/37af5532-5bce-49dd-9b6e-d130df293b9e" />

Picture of all of our parts in Preform:

<img width="1911" height="965" alt="image" src="https://github.com/user-attachments/assets/7fb81fe0-bf6d-428b-919d-3b1ed483b436" />

Final Part and Fit: 

<img width="3024" height="4032" alt="81535257520__033A0284-7987-4FE4-B7F0-537382A2CC6E" src="https://github.com/user-attachments/assets/feafc43e-7b70-46b6-a59d-9211fd1f733c" />

## Fit Test

After printing and post-processing the parts, I used digital calipers to measure the shaft and cylinder bore. The shaft measured 0.143 in, while the cylinder bore measured 0.148 in.

The diametral clearance was calculated by subtracting the shaft diameter from the bore diameter:

.148-.143 = .005

The pin slides into the cylinder relatively well, allowing the two parts to move against each other. However, the measured clearance of 0.005 in is larger than the theoretical RC 2 clearance range of approximately 0.00015–0.00065 in. Therefore, the printed parts demonstrate a functional sliding fit, but they do not meet the theoretical RC 2 tolerance requirements.

This result shows how the actual dimensions of an SLA-printed part can differ from the original design. If I were to revise the design, I would decrease the clearance between the shaft and cylinder to get closer to the RC 2 specification.
<img width="3024" height="4032" alt="81535258949__0E312E23-0B42-430B-B6AB-4B83B56E0458" src="https://github.com/user-attachments/assets/d8d304bf-2452-47a7-a446-1df782685166" />

## Lessons Learned

One of the main challenges during this project was achieving the tight tolerances required for an RC 2 sliding fit. The final shaft measured 0.143 in, and the cylinder bore measured 0.148 in, resulting in a clearance of 0.005 in. This was larger than the theoretical RC 2 clearance range. Even though the pin slides into the cylinder relatively well, the parts did not achieve the precision required by the specification.

Surface roughness and small dimensional differences from the SLA printing and post-curing process may have affected the final fit. These factors made it difficult to achieve the small clearance required between the two components.

If I were to complete this project again, I would print test pieces with different shaft and hole dimensions before printing the final design. I would also pay closer attention to the orientation, support placement, washing, and curing process to improve dimensional accuracy. Measuring the test pieces before making the final parts would help determine the correct CAD dimensions.

Total Time Spent: Approximately 4 hours.

Resources Used:

Machinery's Handbook, Table 8a, for RC 2 fit tolerances.

CAD software for designing the piston and cylinder.

SLA 3D printer and resin.

calipers for measuring the printed components.

Preform Slicer software for preparing the parts for printing.
