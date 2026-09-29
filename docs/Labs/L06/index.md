# A6 Design Fits for an artifact

## Parametrically design

The two main parameters used for the base of the case were Length and Width. The initial values were 3 inches for the length and 2.5 inches for the width. These parameters controlled the overall size of the case base and provided a simple way to adjust the design as the dimensions were refined.

I chose Length and Width because they were the two main dimensions needed to create the base of the case. The initial values were based on an estimate of the size needed to fit the Arduino board. I then used the CAD model and physical measurements to determine the dimensions that were actually necessary for the case to fit correctly.

The Length and Width parameters were adjusted during the design process as I compared the CAD model to the actual dimensions of the Arduino. The changes were made to provide enough space for the board while avoiding unnecessary extra material around it. The final values were selected based on the fit of the printed part and the required clearance around the Arduino. I used the caliper to get the Length, Width and Thickness of the board so I could get a starting measurement of the case.

Hand Drawing: 

<img width="3024" height="4032" alt="IMG_1696" src="https://github.com/user-attachments/assets/c5b95652-acd2-4bd5-8b8b-1995eacd71b4" />

## CAD Model

<img width="836" height="578" alt="Screenshot 2026-09-29 112447" src="https://github.com/user-attachments/assets/b32c09a2-46f7-4f2c-9047-50fbfb6c6883" />

<img width="862" height="464" alt="Screenshot 2026-09-29 112455" src="https://github.com/user-attachments/assets/68e86419-fde1-491a-bdb5-bc62e22ae37b" />

<img width="852" height="544" alt="Screenshot 2026-09-29 112503" src="https://github.com/user-attachments/assets/8bb46da8-116b-4e35-9aa4-7bcba9ee1468" />

<img width="878" height="628" alt="Screenshot 2026-09-29 112511" src="https://github.com/user-attachments/assets/25306710-8724-4220-a656-20d748a10c2a" />

<img width="900" height="544" alt="Screenshot 2026-09-29 112519" src="https://github.com/user-attachments/assets/4b954300-b5f9-4ee9-8092-3a09d3644343" />

<img width="446" height="468" alt="Screenshot 2026-09-29 112527" src="https://github.com/user-attachments/assets/6485f403-6394-45f9-a34f-40e7d07582c9" />

<img width="352" height="400" alt="Screenshot 2026-09-29 112535" src="https://github.com/user-attachments/assets/ae888d3e-58a0-4229-ab27-1cdbc041a7cf" />

## Parameters and Relations used 

<img width="220" height="100" alt="Screenshot 2026-09-29 113020" src="https://github.com/user-attachments/assets/5d58cfaa-64b1-46d4-a2b8-9ef8ef56025c" />

<img width="1408" height="152" alt="Screenshot 2026-09-29 113010" src="https://github.com/user-attachments/assets/95b7996d-1128-44c7-9250-61d3592860f1" />

I determined the engineered allowance by comparing the measured dimensions of the Arduino to the dimensions of my CAD model. I added a small amount of clearance so the case could slide over the Arduino without being too tight, while still keeping the fit secure. The allowance was refined through trial and error by testing the printed part and adjusting the dimensions if the fit was too tight or too loose. Think of it as a phone case for the Arduino. 

Constraints were used to control the geometry of the case and maintain the relationships between features. This allowed the geometry to update consistently when the Length and Width parameters were changed.

## Final CAD design:

<img width="816" height="642" alt="Screenshot 2026-09-29 110928" src="https://github.com/user-attachments/assets/60298a2a-b8ab-4341-9274-2ce3bd80e6fe" />

## Documentation

The part was printed using a Prusa CORE One 3D printer. The CORE One was used to produce the snap-fit case for the Arduino Uno R3.

Design Specs: 

Length: 3in
Width: 2.5in
Indents: .12in
cutout: .13in 

Print Layout

I placed the case flat on the print bed to maximize the contact area with the bed and keep the part stable during printing. This also helped reduce the amount of support material needed.

Build Orientation

I oriented the case so that the bottom was facing the print bed. This orientation allowed the main base to print directly on the bed and kept the walls and snap-fit features oriented vertically. This reduced unnecessary supports and helped maintain the dimensions of the snap-fit features.

Supports 

No supports were used for this print. The case was oriented flat on the print bed so that the geometry could be printed without requiring additional support material. This reduced material usage and eliminated the need for post-processing to remove supports.

Wall Thickness

The wall thickness of the case was .16in Instead of making the walls separately I used a Shell. I used that so I didnt need to manually build 4 walls this thickness was selected to provide enough strength for the case while keeping the part relatively small and lightweight.

### Number of Layers

The print used 51 layers in total.

### Build Volume

The printed part had dimensions of 2.45 × 3.00 × 0.40 inches. This gives a bounding-box volume of approximately 2.94 in³. The slicer estimated the actual material volume at approximately 0.81 in³.

### Slicer Settings

The part was sliced using PrusaSlicer with the 0.20 mm Balanced print setting. Generic PETG was selected as the filament material. The print used 15% infill. Supports were set to "For support enforcers only," although no supports were needed for the final design. No brim was used. The estimated print time was approximately 28 minutes in normal mode.

### Support Removal

No supports were used for the final print, so no support removal was necessary.

### Print Layout and Orientation

The case was placed flat on the print bed with the bottom of the case facing the bed. This provided a large contact area with the print surface and allowed the case to be printed without supports. The orientation also kept the walls and snap-fit features in the intended orientation.

After completing and testing the CAD model, I exported the final part as an STL file and imported it into PrusaSlicer for preparation and printing.

### Fit Test

After printing, the case was tested on the Arduino Uno R3 to determine whether the dimensions and snap-fit features provided the intended fit.
Mine snaps into place and stays even when you shake it upside down. 

### Full Sliced Specs: 

<img width="1368" height="1070" alt="Screenshot 2026-09-29 114446" src="https://github.com/user-attachments/assets/c9299a41-b103-4923-991d-b06c548980fa" />

<img width="1040" height="354" alt="Screenshot 2026-09-29 114440" src="https://github.com/user-attachments/assets/ed579661-9593-4562-9662-e6da9243f62c" />

<img width="2560" height="1436" alt="Screenshot 2026-09-29 114432" src="https://github.com/user-attachments/assets/baf78bb9-a1f0-4723-af6a-1e28102db472" />

Video Of printer working: 

<video controls width="320" src="https://github.com/user-attachments/assets/313d81eb-29f4-4d4d-8647-631447d19af8"></video>

### Lessons Learned 

I learned that measurements taken with calipers are not always the final dimensions that should be used in a design. Calipers provide the physical dimensions of the artifact, but the CAD design may need additional clearance, spacing, or other adjustments depending on how the parts interact. The measured dimensions should therefore be treated as a starting point, followed by engineering decisions and physical testing to determine the final design dimensions.

I learned that using parameters made it much easier to modify the design. Instead of changing individual dimensions throughout the model, I could change the main parameters and update the case. This made the design process faster when adjustments were needed.

I learned that a snap fit needs a balance between clearance and retention. If the fit is too tight, the parts can be difficult to assemble or damage the part. If it is too loose, the part will not stay attached. Designing and testing the snap features helped me understand how small changes in dimensions affect the final fit.

I learned that the orientation of a part can greatly affect how it prints. By placing the case flat on the print bed, I was able to print the part without supports. This reduced material usage and eliminated additional post-processing.

One mistake I made was starting with estimated dimensions instead of having all of the required measurements finalized. I corrected this by comparing the CAD model to the actual Arduino and adjusting the parameters as needed. This helped me understand the importance of designing around measured dimensions rather than assumptions.


### Time and Resources

In total, this project took approximately 12 hours from the initial brainstorming and development of different design ideas through CAD development, multiple design iterations, 3D printing, and fit testing. A significant portion of the time was spent comparing different concepts and making changes between prints to improve the final design.
