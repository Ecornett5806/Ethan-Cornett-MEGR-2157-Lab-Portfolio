# LAB #3 Design Something Small: 

## Starting Questions:
How does percentage infill affect mechanical properties?

Infill percentage determines the density of the internal structure and the ratio of solid material to air space inside the part. A higher percentage results in a stronger, heavier component that requires more filament and a longer print duration.

How do different infill patterns affect mechanical properties?
Different patterns determine how much force and distributed load the part can take. For example, a honeycomb is extremely strong because of its ability to distribute loads across the entire surface area. 

Why use different wall thicknesses?

Wall thicknesses determine how much structural load and stress a part can handle, as the outer shells bear the majority of external forces. Increasing wall thickness significantly boosts a part's overall strength and makes it watertight or airtight, while fewer walls save material and print time for lightweight designs.

## Design Process: 

I initially considered designing an arrowhead, but after reviewing the project constraints that prohibited weapons, I abandoned the idea during the early brainstorming phase.
My second idea was a Celtic knot, but it proved to be overly complex for the current scope, so it did not progress past the initial planning stage.

While looking at the cross necklace around my neck, I realized it was the ideal subject. The cross features a clean, simple geometry that translates well to 3D design, and it holds deep personal significance as a reflection of my Christian faith.

The following is the rough sketch I used to make my cross: 
I had to redesign to allow myself to extrude the cross but the general shape looks very similar to this.

<img width="552" height="406" alt="Screenshot 2026-09-05 142923" src="https://github.com/user-attachments/assets/3f4b0768-6b42-4c8e-a56c-c3d005ea3175" />

This is a picture of my final design after making the necessary adjustments in CAD and preparing it for printing. For the final print, I used infill throughout the inside of the part to provide additional strength while also reducing the amount of material needed compared to making the entire part solid. I also added a skirt around the outer edge of the print. The skirt does not connect to the part itself; instead, it helps prime the nozzle before the actual print begins and allows me to visually check that the filament is extruding properly. Overall, the combination of the final CAD design, infill, and skirt allowed me to prepare the part for a successful print while keeping the design within the requirements of the assignment.

<img width="595" height="1248" alt="IMG_1461" src="https://github.com/user-attachments/assets/56891faf-c2c1-4b2e-bb9c-edea29415f2e" />

## Researching Infills and Mechanical properties: 

Research three infills not shown in class to describe the geometry and why each infill is used.

Triangle infill is made from lines printed in three different directions, creating a repeating triangular structure. The triangular geometry creates a rigid internal pattern because the intersecting lines provide support in multiple directions. Triangle infill is useful when a part needs additional internal strength and support while still using less material than a completely solid part. It is also relatively similar to Grid infill in terms of material usage and print time.

<img width="256" height="192" alt="image" src="https://github.com/user-attachments/assets/738f9c93-7209-41b8-9189-8d7923a839e4" />

Lightning infill uses a branching, tree-like geometry rather than filling the entire inside of the part with a uniform pattern. The branches become denser near the top surfaces, where they are needed to support the upper layers. This pattern is primarily used when internal structural strength is not the main concern. Its main purpose is to support the top of a print while using as little material and printing time as possible. This makes it useful for decorative models, prototypes, and parts where reducing filament usage is more important than maximizing strength.

<img width="400" height="300" alt="image" src="https://github.com/user-attachments/assets/ac3b03a5-204f-496a-846d-f49eaa9f7ae9" />

Stars infill is based on the triangular pattern, but the paths are shifted to create repeating six-pointed star shapes. The lines cross within each layer, creating a more complex internal geometry than the basic triangle pattern. Stars infill is useful when a printer needs a structured internal pattern while maintaining similar material usage and print time to Triangle infill. Its geometry also gives the printed part internal support without requiring the entire interior to be solid.

<img width="256" height="192" alt="image" src="https://github.com/user-attachments/assets/da080cda-275b-4576-8afe-a5415d869d95" />

I used https://help.prusa3d.com/article/infill-patterns_177130 for the information reguarding these infills.
Used for information regarding the Triangle, Stars, and Lightning infill patterns, including their geometry, material usage, and printing characteristics.)

how does infill percentage affect mechanical properties, and how do different infill patterns affect mechanical properties?

Infill percentage has a significant effect on the mechanical properties of a 3D-printed part. As the infill percentage increases, more material is placed inside the part and the amount of empty space decreases. This generally increases the part's strength and stiffness while also increasing its weight, material usage, and print time. However, increasing the infill percentage is not always the most efficient way to strengthen a part because the number of outer walls can also have a major effect on strength.

The infill pattern also affects the mechanical properties because it determines how the material is arranged inside the part. Different patterns distribute forces differently and can provide different levels of strength, stiffness, flexibility, and resistance to deformation. For example, Triangle infill creates a rigid triangular structure, while Lightning infill uses a branching structure that prioritizes saving material and print time rather than maximizing strength. Therefore, selecting an infill pattern depends on the intended use of the part and the type of loading it will experience.

Overall, infill percentage determines how much material is used inside the part, while infill pattern determines **how that material is arranged**. Both factors can affect the final mechanical performance of a 3D-printed component.

## Preprocessor and Printing

After completing the CAD model, I exported the cross as an STL file and imported it into PrusaSlicer. From there, I prepared the model for printing by selecting the appropriate printer and material, choosing the build orientation, setting the infill, adjusting the wall thickness, and checking the estimated print time.

## Build Orientation

I chose to print the cross flat against the build plate. This orientation was selected because the cross has a large, flat surface that can sit directly on the print bed. Printing it flat also reduced the need for supports because there were no significant overhangs that required additional material underneath the model. This orientation also allowed the cross to be printed within the height restrictions of the assignment.

## Scaling
I set my scale to 13% of the original size due to the amount of time the slicer said it would take to finish the cross, I believe the scaling was so dramatic because Creo was not set to inches so my dimensions were all off. 

## Infill 

For my final print, I used monotone lines at 30% infill. This was different from the default setting because I wanted to examine how the internal structure could affect the final part. I selected this pattern because I feel like it fir the idea that the cross is straight lines so having a simple, consistent internal structure while producing a clean surface finish.

The following Image shows the exact specifications for my infill. 

<img width="938" height="356" alt="image" src="https://github.com/user-attachments/assets/5880782c-ccb1-42a7-bf5b-b1c45b11162a" />

Wall Thickness:
I didn't change my wall thickness much because A cross is supposed to be constant thickness throughout. however I did scale it up a little given that the print had the cross super thin and I wanted it to have some layers. 

Here was my thickness specifications:

<img width="738" height="450" alt="Screenshot 2026-09-06 124045" src="https://github.com/user-attachments/assets/1926f1c9-8021-4dd5-aaf4-36dc1846207c" />

## Skirt

I added a skirt around the outside of the cross. The skirt does not physically connect to the part. Its purpose is to allow the printer to prime the nozzle before beginning the actual print. It also gives me an opportunity to visually check the first extrusion and make sure the filament is flowing properly before the cross begins printing.

I used a skirt with a 6 mm distance from the object. The skirt was printed around the cross without touching the actual part. I used the skirt to prime the nozzle and verify that the filament was extruding properly before the print began. I did not use a brim because the cross had a large flat surface in contact with the build plate, so additional adhesion from a brim was not necessary. The brim width was set to 0 mm.

<img width="820" height="306" alt="Screenshot 2026-09-06 124256" src="https://github.com/user-attachments/assets/e43095f2-ee29-4bdf-b9d7-3ac45516e485" />

## Print 

We used Printer PC-16 material with PETG

Video of our prints being made: 


<video controls width="640" src="https://github.com/user-attachments/assets/100210ac-6f99-4a26-ae80-2ef7fe75b4d8"></video>


## Mistakes made and Lessons learned: 

One mistake I caught during the project was an issue with the sizing of my model. I realized that the dimensions in Creo were not set correctly, which caused the model to be much larger than intended. I noticed the problem when I brought the model into PrusaSlicer and saw that the print would take much longer than expected. I corrected this by scaling the model down to 13% in PrusaSlicer so that it would fit within the project requirements and have a reasonable print time.

A mistake I could have easily missed was the uneven and asymmetrical shape of my cross. Because I rushed through the CAD portion, I did not spend enough time checking that each section was properly sized and symmetrical. Although the part was still printable, the uneven geometry affected the appearance of the final product. In the future, I would take more time to check the symmetry and dimensions of the CAD model before exporting it to PrusaSlicer.

In future projects, I will take more time during the CAD portion to make sure the final part is properly designed and meets all of the project constraints. I will also verify that my units are correct in Creo, especially making sure the model is being designed in inches rather than millimeters. Before moving the model into PrusaSlicer, I will double-check the dimensions and symmetry of the part.

I would also improve how I document my design process. Instead of only documenting the successful design, I would take screenshots of failed or unfinished designs and include images of similar designs that influenced my ideas. This would better show the progression from my original idea to the final product.

The total time I spent on this project was approximately 4 hours. About 10 minutes were spent brainstorming ideas, 10 minutes creating the CAD model in Creo, and approximately 5 minutes correcting CAD mistakes. Preparing the model in PrusaSlicer took approximately 2–3 minutes. Printing took approximately 20 minutes for all three of our prints. The largest amount of time was spent documenting the project, which took approximately 3–4 hours. This showed me that documentation can take significantly longer than the actual design and printing process, so I need to plan time for documentation throughout the project rather than completing it all at the end.

If I were to scale this design up and use it as a structural or safety-critical component, I would not consider my current design reliable enough. The uneven geometry and lack of symmetry could make the part less stable and cause it to deform or fail under a significant load. Although the cross shape has historical significance because crosses were used for crucifixion, the shape itself does not guarantee structural stability. Before using a 3D-printed component for a safety-critical application, I would need to carefully verify the dimensions, material, wall thickness, infill, loading conditions, and safety factor. I would also need to test the part before trusting it with an important load.

A real-world example that connects to this project is a house foundation. If a foundation is not designed or built properly, it may not be strong enough to support the rest of the house. Problems with the foundation can cause the structure above it to shift, crack, or become unstable. This relates to my 3D-printed cross because both situations show the importance of checking the overall design, dimensions, material, and structural requirements before relying on a component. In a safety-critical application, I would need to use proper engineering calculations, safety factors, material specifications, and testing rather than assuming that a part will be strong enough based only on how it looks.

<img width="1040" height="547" alt="Fixing-a-House-With-a-Bad-Foundation" src="https://github.com/user-attachments/assets/2b3dac8c-f020-4270-b633-5240a8f13763" />

Sources: 
Prusa Research – Infill Patterns
https://help.prusa3d.com/article/infill-patterns_177130?product=mk3-9s&utm_source=chatgpt.com
Used for information regarding the Triangle, Stars, and Lightning infill patterns, including their geometry and printing characteristics.

Fine Homebuilding – Fixing a House With a Bad Foundation:
https://www.finehomebuilding.com/1996/09/01/fixing-a-house-with-a-bad-foundation?utm_source=chatgpt.com
Used for the foundation image and as a visual example of how foundation problems can affect a house.
