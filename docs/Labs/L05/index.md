# A5 – SNAP FIT 

## Calulating values: 

<img width="4284" height="5712" alt="IMG_1634" src="https://github.com/user-attachments/assets/6d634f9d-df13-43a2-b27a-88af8660c32f" />

### Flexure Design values and reasoning 
Material Selection

PLA was selected for the snap-fit assembly because it is readily available for FDM printing and provides sufficient stiffness for the application. Published Prusament PLA data reports a tensile modulus of approximately 2.3 GPa and a horizontal tensile yield strength of approximately 36 MPa.

Because of that your allowed normal stress of 10.29  Mpa

### Initial Flexure Dimensions

The initial flexure width and thickness were selected as 12 mm and 4 mm, respectively. These dimensions were selected to provide a compact flexure while maintaining sufficient cross-sectional area for the printed component.

### Flexure Length

The flexure was modeled as a cantilever beam with a concentrated load at its free end. A transverse design load of 1.5 lbf was selected. A target deflection of 1.5 mm was selected so that the flexure could clear the 1.3 mm snap lip.

### Bending Stress

The maximum bending stress occurs at the fixed end of the cantilever. The calculated bending stress was 9.65 MPa, compared with an allowable normal stress of 10.29 MPa after applying the required safety factor of 3.5. The calculated safety factor was 3.75, so the flexure satisfies the strength requirement.

### Axial Stress

A 7 lbf axial load was selected because it falls within the required 5–10 lbf range. Assuming the load is shared equally between the two flexures, each flexure carries 3.5 lbf. The resulting axial stress was 0.649 MPa.

### Shear Stress

The average shear stress at the flexure protrusion was calculated using the 3.5 lbf reaction at each side. The resulting shear stress was 0.973 MPa, which is below the allowable shear stress of 7.29 MPa using a Tresca-based yield check with the required safety factor.

### Design Iteration

The initial calculation produced a flexure length of approximately 46.3 mm. The length was rounded to 46 mm for the CAD model and checked using the cantilever deflection equation. The calculated bending stress remained below the allowable stress, while the resulting deflection was greater than the 1.3 mm snap-lip height. The design therefore met the calculated strength and deflection requirements and was carried forward to the CAD stage.

## First unparameterized design print: 

<img width="1024" height="2032" alt="IMG_1635" src="https://github.com/user-attachments/assets/bf8f5344-b103-4001-ac4a-beca32c0f76f" />


## Secound Parameterized design:

<img width="1024" height="2032" alt="IMG_1632" src="https://github.com/user-attachments/assets/df6c9838-2420-4640-8790-c3570b94a44b" />

## PARAMETRICALLY DESIGNED PORTIONS 

The snap-fit assembly was created using parametric modeling so that the main dimensions of the design could be changed without rebuilding the geometry. The parameters were selected based on the flexure calculations and the dimensions needed to control the interaction between the two printed components.

I had to limit the amount of the design that was parametrically designed due to time constraints and because of this my design is not a parametrically driven as much as I would like them to be, However I got the general geometry down parametrically specifically the width and height of the design both top clip and bottom clip being 12 and 46 mm. 

Below are the pictures of my CAD design when it was finished Aswell as the parameter and relations I used in the design process. 

## Design Parameters: (some went unused) 
<img width="1370" height="608" alt="Screenshot 2026-09-22 110151" src="https://github.com/user-attachments/assets/c03de809-1603-4fd5-87d8-f339e2648930" />

<img width="1388" height="574" alt="Screenshot 2026-09-22 110202" src="https://github.com/user-attachments/assets/9a03a74d-d238-472d-98a5-e4ad04d7d931" />

## Design Relations: 

<img width="1384" height="142" alt="Screenshot 2026-09-22 105350" src="https://github.com/user-attachments/assets/aae377e9-1b0f-43cf-8d6a-c05036b00040" />

The parameters were chosen based on the calculations from the design stage and the geometry required for the snap-fit assembly.

The three primary flexure parameters were FLEX_L, FLEX_W, and FLEX_T. These dimensions control the size and stiffness of the cantilever flexure. The calculated flexure length was approximately 46.3 mm, so FLEX_L was set to 46 mm for the CAD model. The width and thickness were set to 12 mm and 4 mm, respectively, based on the initial flexure design.

The snap features were supposed to be controlled using LIP_H and LIP_T. The lip height was going to be set to 1.3 mm because the flexure was designed to deflect approximately 1.5 mm, allowing it to pass over the lip during assembly. The parameters were ultimately not used to drive the final geometry because the dimensions were established during the CAD development process and did not require additional iteration. 

The FILLET_R parameter was set to 2 mm to control the rounded transition at the flexure. This avoids using an unnecessarily sharp corner at the beginning of the flexible section. I ended up not needing to use a fillet, so this parameter was just in case. 

The base dimensions were controlled using BASE_W and BASE_H. These parameters control the overall size of the rigid component and allow the base to be resized without manually rebuilding the sketch. Because the base and the flex values were the same, I decided that they were unnecessary. 

Finally, CLEARANCE was set to 0.3 mm to provide an engineered allowance between the mating components. This prevents the two printed parts from being modeled as an exact interference and provides space for normal dimensional variation from FDM printing. The parameter was ultimately not used to drive the final geometry because the mating dimensions were established directly during CAD development.

Final CAD model:

<img width="826" height="954" alt="Screenshot 2026-09-22 105312" src="https://github.com/user-attachments/assets/aa634571-e235-4b4c-82f9-e05184d1a7d0" />

## Design Changes and Iteration

The only major design change I had to do was changing the base from a super wide 30mm to matching the other parts 12mm width. Outside of that my initial design was the final design. 

## 3D Printing and Build Orientation

### Build Orientation Research

FDM printed parts are anisotropic, meaning their mechanical properties can change depending on how the part is oriented during printing. A study investigating FDM-printed PLA found that print orientation has a significant effect on flexural performance. The study found that, for bending, the orientation of the deposited layers should be considered carefully. In particular, when the deposition direction is parallel to the bending plane, longer continuous layers are produced and the printed part has greater resistance to bending. When the raster orientation is angled relative to the bending plane, the effective fiber length is reduced and separation between layers becomes easier.

For my design, the flexures were oriented so that their length and bending direction remain primarily within the printed layers rather than relying on the weaker bond between layers. This aligns with the research because the flexure is being loaded in bending along the direction of the deposited material. This orientation should allow the individual printed layers to carry more of the bending load instead of placing the majority of the load across the layer interfaces. Therefore, the selected orientation is consistent with the research recommendation for improving the bending resistance of an FDM-printed PLA flexure.

### Preprocessor 

After completing the CAD model, I imported both components into PrusaSlicer to prepare them for printing. The preprocessor was used to determine the amount of filament required, estimated print time, infill, material, printer settings, and final placement of the parts on the print bed. These settings were checked before printing to make sure both components could be produced as designed.

## Total filament used and the total time for print to finish. 

The first screenshot shows the estimated material usage and total time required to complete the print. The slicer calculates these values after generating the toolpath for the models. This information was used to confirm that the print could be completed within the available printing time while also estimating how much PLA would be required.

<img width="444" height="320" alt="Screenshot 2026-09-22 111801" src="https://github.com/user-attachments/assets/d1f4c602-9f6a-423a-9845-467b47edfa9e" />

## Infill used: 

The second screenshot shows the infill settings selected for the parts. Infill provides internal structure while reducing the amount of material compared to printing the parts completely solid. The selected infill was used to provide additional internal support while keeping the print time and material usage reasonable.

<img width="1016" height="292" alt="Screenshot 2026-09-22 111753" src="https://github.com/user-attachments/assets/a80f533e-689a-49d9-b667-6931782cc022" />

### Material used: printer used:

The third screenshot shows the material and printer configuration used in PrusaSlicer. The print was prepared using PLA because the flexure was designed and analyzed using PLA material properties. The printer profile was selected to match the printer being used so that the slicer could generate the appropriate toolpath and printing parameters.

<img width="840" height="770" alt="Screenshot 2026-09-22 111737" src="https://github.com/user-attachments/assets/08d77f0e-da8f-443d-9766-c4322aa79c3a" />

## Supports: 

I didn't use any supports because my print laid flat on the table 

### final design on the plate and sliced:

The final screenshot shows both components positioned on the build plate after being sliced. The orientation of the parts was selected so that the flexures could be printed in an orientation appropriate for the expected bending load. The completed slice also allowed the toolpath to be inspected before printing, including the outer walls, infill, and support regions. This step helped verify that the entire model would be printed and that the snap-fit features were included in the generated toolpath.

<img width="1510" height="1040" alt="Screenshot 2026-09-22 111744" src="https://github.com/user-attachments/assets/d2f23412-9b33-451c-8a7d-0f6443e3e455" />

### Preprocessor Summary

The preprocessor stage converted the completed CAD models into a printable toolpath. Before starting the print, I checked the estimated material usage, print time, infill, material and printer selection, and final model orientation. Reviewing these settings before printing helped catch potential problems before material was used and provided a final check that the printed parts matched the intended design.

## Mistakes made 

1: was not set on a design till late which lead to not being able to parametrically design as much as I would have liked:

2: Didnt set up the width of the top section correctly in the first print.

3: The printing process also showed that small snap-fit features require more attention than larger features. The hooks and flexures have to fit together while still having enough material to withstand repeated bending. This reinforced the need to check clearances and feature dimensions before printing the final version.

# Lessons Learned: 

## Parametric Modeling

The project also gave me more experience with parametric CAD. Instead of treating every dimension as an independent number, I created parameters such as FLEX_L, FLEX_W, and FLEX_T so that important dimensions could be changed without rebuilding the entire model.

For example, changing the flexure length through the parameter allowed the geometry to update without manually changing every related dimension. This demonstrated why parametric modeling is useful for engineering design. If testing showed that the flexure needed to be longer, shorter, thicker, or wider, the model could be adjusted much faster.

I also learned that creating a parameter does not automatically make a model fully parametric. A parameter needs to actually control a dimension or feature in the model. Some of the parameters I created were ultimately not used to drive the final geometry. This helped me understand the difference between having parameters in a model and actually using parameters to control the design.

## Designing Around the Function

One of the biggest lessons I learned was that the dimensions of a part should be based on how the part is expected to function. The flexure in this design is not simply a thin piece of plastic; it acts as a cantilever beam that has to bend when the two components are assembled. Because of this, the length, width, and thickness of the flexure directly affect how much it bends and how much stress develops in the material.

I originally focused more on making the parts fit together physically. After working through the beam calculations, I understood that the flexure dimensions also had to satisfy the stress and deflection requirements. This made the engineering calculations useful during CAD instead of treating them as a separate part of the assignment.

## Testing Is Part of the Design

I also learned that calculations and CAD cannot completely replace physical testing. The calculations use assumptions about material properties, loading, geometry, and how the load is distributed. The actual printed part introduces additional factors such as layer adhesion, print defects, dimensional variation, and surface finish.

Printing the components provides a way to see whether the assumptions made during the design process actually produce a functional part. If the snap fit is too tight, too loose, too difficult to assemble, or breaks during testing, the CAD model can then be modified.

This also stems from me printing a part I know was going to fail so I could see what needed to be fixed. 

## Resources and actual time it took from start to finish

Actual time it took to fully do the calculations make the cad and print was about 4 hours. I started at 8 pm and finished the design at 12 am. 
