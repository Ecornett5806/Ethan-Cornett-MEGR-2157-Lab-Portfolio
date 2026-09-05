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

<img width="1052" height="906" alt="Screenshot 2026-09-05 142923" src="https://github.com/user-attachments/assets/3f4b0768-6b42-4c8e-a56c-c3d005ea3175" />

This is a picture of my final design after making the necessary adjustments in CAD and preparing it for printing. For the final print, I used infill throughout the inside of the part to provide additional strength while also reducing the amount of material needed compared to making the entire part solid. I also added a skirt around the outer edge of the print. The skirt does not connect to the part itself; instead, it helps prime the nozzle before the actual print begins and allows me to visually check that the filament is extruding properly. Overall, the combination of the final CAD design, infill, and skirt allowed me to prepare the part for a successful print while keeping the design within the requirements of the assignment.

<img width="1095" height="1748" alt="IMG_1461" src="https://github.com/user-attachments/assets/56891faf-c2c1-4b2e-bb9c-edea29415f2e" />

## Researching Infills and Mechanical properties: 

Research three infills not shown in class to describe the geometry and why each infill is used.

Triangle infill is made from lines printed in three different directions, creating a repeating triangular structure. The triangular geometry creates a rigid internal pattern because the intersecting lines provide support in multiple directions. Triangle infill is useful when a part needs additional internal strength and support while still using less material than a completely solid part. It is also relatively similar to Grid infill in terms of material usage and print time.

Lightning infill uses a branching, tree-like geometry rather than filling the entire inside of the part with a uniform pattern. The branches become denser near the top surfaces, where they are needed to support the upper layers. This pattern is primarily used when internal structural strength is not the main concern. Its main purpose is to support the top of a print while using as little material and printing time as possible. This makes it useful for decorative models, prototypes, and parts where reducing filament usage is more important than maximizing strength.

Stars infill is based on the triangular pattern, but the paths are shifted to create repeating six-pointed star shapes. The lines cross within each layer, creating a more complex internal geometry than the basic triangle pattern. Stars infill is useful when a printer needs a structured internal pattern while maintaining similar material usage and print time to Triangle infill. Its geometry also gives the printed part internal support without requiring the entire interior to be solid.

how does infill percentage affect mechanical properties, and how do different infill patterns affect mechanical properties?
