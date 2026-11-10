# A11 – Motor Selection

## Objective

The objective of this project is to design and 3D print a small clip-on shelf using the Form 4 SLA printer. The shelf will attach to an existing platform using two integrated C-shaped snap-fit clips. These clips will flex during installation and securely grip the platform, allowing the shelf to be attached and removed without additional hardware. The design focuses on creating a functional snap-fit mechanism while considering material properties, dimensional tolerances, flexibility, and durability.

## Research:

Selected Snap-Fit Type: Annular (Cylindrical):

The snap-fit mechanism used in this project is an annular-style snap fit. The design consists of a cylindrical socket with a section removed, creating a C-shaped opening, and a separate cylindrical beam that fits inside the opening.

During assembly, the C-shaped socket expands outward as the cylindrical beam is pressed into it. Once the beam passes the opening, the socket returns toward its original shape and grips the beam. The connection relies on the flexibility of the cylindrical socket rather than a traditional cantilever arm.

The main design principles include:

Radial deflection: The C-shaped socket must expand enough to allow the cylindrical beam to enter.

Retention: The opening must be smaller than the effective diameter of the beam so the socket can grip it after assembly.

Wall thickness: The socket wall must be thin enough to flex but thick enough to maintain structural strength.

Rounded edges: Sharp corners around the opening should be avoided to reduce stress concentrations.

Material flexibility: The resin must tolerate the expansion required during installation without cracking.

Deflection and Undercut Geometry:

Deflection occurs when the C-shaped socket expands outward to allow the cylindrical beam to pass through. The amount of expansion depends on the difference between the beam diameter and the socket opening.

The undercut is created by making the opening slightly smaller than the diameter of the cylindrical beam. This creates interference between the two components, allowing the socket to retain the beam after installation.

Increasing the difference between the opening and beam diameters increases the amount of expansion required. However, excessive interference can create too much strain and cause the resin to crack.

The design must balance the amount of interference with the flexibility of the socket. The goal is to allow the cylindrical beam to enter with reasonable force while maintaining enough retention to keep the shelf securely attached.

Stress Concentrations and Wall Thickness:

The areas surrounding the opening of the C-shaped socket are important because they experience deformation during assembly. Sharp edges or sudden changes in geometry can create localized stress concentrations, increasing the possibility of cracking.

Rounded transitions should be used around the opening to help distribute stress more evenly throughout the socket.

The socket was designed with a wall thickness of 0.025 inches (0.635 mm). This relatively thin wall allows the C-shaped section to expand outward during installation. However, reducing wall thickness also reduces stiffness and structural strength.

A thicker wall would increase the force required to expand the socket, while a thinner wall would allow greater flexibility but could become more susceptible to damage. The selected thickness is intended to balance flexibility and strength.

Mechanical Principles Governing Performance:

The performance of the snap-fit mechanism depends on the relationship between the socket opening, cylindrical beam diameter, wall thickness, and material properties.

Deflection and permissible strain: The socket must expand enough to allow the beam to enter without exceeding the permissible strain of the resin. Excessive deformation can cause permanent damage or fracture. The amount of allowable expansion depends on the material and the geometry of the socket.

Undercut and mating force: The smaller the socket opening is compared to the beam diameter, the more the socket must expand during installation. Greater interference generally increases the force required for assembly. However, insufficient interference can result in a loose connection that does not securely retain the shelf.

Stiffness and geometry: Wall thickness directly affects how much force is required to expand the socket. A thicker wall increases stiffness, while a thinner wall allows more flexibility. The C-shaped geometry provides an opening that allows the socket to expand rather than requiring the entire cylinder to stretch equally.

The final design must balance these properties to provide a secure connection that can be assembled and removed without damaging the components.

SLA Resin Material Considerations:

The components were designed for printing on the Formlabs Form 4 using Grey V5 resin. SLA printing uses light to cure liquid photopolymer resin into solid parts. Unlike FDM printing with PLA, SLA produces parts through a photochemical curing process.

Grey V5 is a relatively rigid resin, so excessive expansion of the C-shaped socket could cause cracking. For this reason, the design must limit the interference between the cylindrical beam and socket while maintaining enough engagement to prevent the shelf from becoming loose.

The socket uses a wall thickness of 0.025 inches (0.635 mm). This thickness was selected to allow the C-shaped section to expand during installation while maintaining enough material to grip the cylindrical beam.

Material properties, including tensile strength, elongation at break, and elastic modulus, influence how much the socket can deform before failure. Post-curing can also affect the final mechanical properties of the resin. Therefore, the finished components must be evaluated after washing and curing to determine whether the design provides sufficient flexibility and durability.

Application of Research to the Design:

The research on annular snap fits influenced several aspects of the clip-on shelf design. The C-shaped cylindrical socket was selected to provide radial flexibility around the cylindrical beam. The 0.025-inch wall thickness was used to allow the socket to expand during installation without making the entire component excessively thick.

The opening size and beam diameter determine the amount of interference and therefore the amount of expansion required. These dimensions are important because excessive interference could damage the resin, while insufficient interference could result in a loose connection.

The design also considers stress concentrations around the opening and the importance of maintaining smooth transitions between surfaces. These features help improve the durability of the socket during repeated installation and removal.

The completed design will be evaluated through physical testing to determine whether the socket securely retains the cylindrical beam, provides reasonable installation force, and withstands repeated assembly without cracking.

## Design:

CAD DESIGN CLIP:

<img width="736" height="380" alt="image" src="https://github.com/user-attachments/assets/bf1133b7-4342-4e10-bf84-29b76b04cd8e" />

<img width="1082" height="460" alt="image" src="https://github.com/user-attachments/assets/1abf4470-6a39-463b-90fd-c0843c156cbd" />

<img width="128" height="992" alt="image" src="https://github.com/user-attachments/assets/efc32b54-850b-481c-b7d3-f767ef8f04ad" />

<img width="556" height="756" alt="image" src="https://github.com/user-attachments/assets/7a82ab74-3322-46fc-8ea7-9df770772daa" />

<img width="746" height="710" alt="image" src="https://github.com/user-attachments/assets/4fb4f810-9ae3-4b0b-a69b-79815da2ed75" />

<img width="430" height="538" alt="image" src="https://github.com/user-attachments/assets/5838ad58-fe7f-46cc-a9e7-697bba143e9c" />

CAD DESIGN PILLERS AND BASE: 

<img width="1244" height="510" alt="image" src="https://github.com/user-attachments/assets/fb028b3e-7415-418f-b7d2-bfc073eefb71" />

<img width="1150" height="672" alt="image" src="https://github.com/user-attachments/assets/4f2eba69-6d89-4190-b3e4-e4aee536197e" />

<img width="862" height="868" alt="image" src="https://github.com/user-attachments/assets/310fea34-2c34-4439-a1ea-0fa295295433" />

<img width="946" height="744" alt="image" src="https://github.com/user-attachments/assets/7ec67c74-834e-4545-8164-1e5e81d065e4" />

## Preprocessing and 3D Printing:

Machine and Material Selection:

The snap-fit shelf components were prepared for printing using the Formlabs Form 4 SLA printer. The selected material was Formlabs Grey V5 resin. This resin was used to produce dimensionally accurate components with a smooth surface finish.

The printer was configured with a layer thickness of 0.100 mm and the default Grey V5 print settings.

Build Orientation and Layout:

The components were imported into PreForm and arranged on the build plate. The parts were tilted at an angle rather than positioned completely flat against the build platform. This orientation allowed support structures to be generated underneath the models and helped reduce unsupported geometry during printing.

The build contained four model files, including the snap-fit components, clip, and platform. The parts were arranged to fit within the available build area while allowing space for support structures.

The models were positioned together to make efficient use of the build plate and reduce the need for separate print jobs.

Support Strategy and Wall Thickness:

PreForm automatically generated support structures underneath the models to help stabilize them during printing. Supports were used to maintain part positioning and reduce the possibility of print failures.

The build contained 329 support touchpoints and 11.42 mL of support material. A raft volume of 17.01 mL was also generated to provide a stable foundation for the printed components.

The C-shaped snap-fit socket was designed with a wall thickness of 0.025 inches (0.635 mm). This relatively thin wall allows the socket to expand outward when the cylindrical beam is pressed into the opening. The thickness was selected to balance flexibility and structural strength.

Print Resolution and Layer Settings: 

The Form 4 was configured with a layer thickness of 0.100 mm. Layer thickness determines the vertical resolution of the printed components. A smaller layer height generally produces finer surface details but can increase printing time.

The default Grey V5 print settings were used for this build. The selected resolution provides a balance between dimensional accuracy, surface quality, and production time.

Isotropic and Anisotropic Properties: 

The printed components are considered potentially anisotropic because their mechanical properties can vary depending on print orientation and layer formation.

SLA printing generally produces more uniform mechanical properties than typical FDM printing because it does not rely on the same type of deposited filament bonding. However, differences in layer formation, curing, and print orientation can still influence strength.

This is particularly important for the C-shaped snap-fit socket because it must expand during assembly. The print orientation should be considered when evaluating the socket's ability to withstand repeated deformation.

Snap-Fit Clearance:

The snap-fit connection uses a cylindrical beam that engages with a C-shaped cylindrical socket. The opening of the socket is designed to be smaller than the effective diameter of the beam, allowing the socket to expand during installation and grip the beam once assembled.

The socket has a wall thickness of 0.025 inches (0.635 mm). The dimensional clearance and interference between the cylindrical beam and socket opening must be considered to ensure proper engagement.

The opening and beam dimensions will determine the amount of expansion required during assembly. Excessive interference could cause the resin to crack, while insufficient interference could result in a loose connection.

The final clearance/interference will be documented using the CAD dimensions and evaluated during physical assembly testing.

7. PreForm Slicer Settings and Print Details

The following information was recorded from the PreForm software:

| Parameter | Recorded Value |
|:---|:---|
| Printer | Formlabs Form 4 |
| Resin | Grey V5 |
| Layer Thickness | 0.100 mm |
| Print Settings | Default |
| Estimated Print Time | Approximately 2 hours |
| Total Build Volume | 102.00 mL |
| Model Volume | 73.57 mL |
| Support Volume | 11.42 mL |
| Raft Volume | 17.01 mL |
| Total Layers | 811 |
| Support Touchpoints | 329 |
| Number of Model Files | 4 |

<img width="2560" height="1600" alt="image" src="https://github.com/user-attachments/assets/efd1966f-f0b2-4e34-b374-4fa40f1662f7" />

Preprocessing Summary

The preprocessing stage established the printing orientation, support structures, resin selection, and resolution settings for the snap-fit shelf. The Form 4 and Grey V5 resin were selected to produce accurate components with a smooth surface finish.

The final build was arranged with four model files, used a 0.100 mm layer thickness, and had an estimated print time of approximately two hours.

The main design consideration during preprocessing was maintaining the geometry of the C-shaped socket while ensuring that its thin 0.025-inch wall could be printed successfully. The printed parts would then be evaluated after washing and curing to determine whether the socket provided sufficient flexibility and retention during assembly.

## Post Processing: 

 1. Washing Process

After printing, the components were removed from the build platform and prepared for washing. Washing removes uncured resin remaining on the surfaces of the printed parts. This step is important because leftover resin can affect surface quality, dimensional accuracy, and the final curing process.

The components were washed for 5 minutes to remove excess resin from their surfaces. After washing, the parts were prepared for the curing stage.

| Parameter | Recorded Information |
|:---|:---|
| Washing duration | 5 minutes |
| Washing method | Resin washing process |
| Material | Grey V5 |
| Printer | Formlabs Form 4 |

**Figure 1. Washing Process**

[Insert photograph of the components during washing.]

#2. Support Removal

After washing, the support structures were removed from the printed components. Supports were used during printing to maintain stability and prevent unsupported areas from shifting.

Extra care was taken when removing supports around the C-shaped cylindrical socket because its wall thickness is only 0.025 inches (0.635 mm). Applying too much force during removal could damage the thin walls or affect the dimensions of the snap-fit opening.

After removal, the components were inspected for remaining support marks and visible damage.

| Parameter | Recorded Information |
|:---|:---|
| Removal method | Spatula |
| Tools used | Spatula |
| Areas requiring extra care | C-shaped socket and cylindrical opening |

<img width="2284" height="3712" alt="IMG_1986" src="https://github.com/user-attachments/assets/7a782f9d-ab52-40f3-9271-c5d1b3861f3c" />

3. Curing Process

After washing and support removal, the components were placed in the curing equipment for 5 minutes. Curing uses additional light exposure to complete the polymerization process within the resin.

After curing, the material became slightly harder and less elastic. This change is important because the C-shaped socket relies on flexibility to expand around the cylindrical beam during assembly.

Although the curing process improved the rigidity of the components, the reduction in elasticity meant that the socket could tolerate less deformation before becoming susceptible to damage.

| Parameter | Recorded Information |
|:---|:---|
| Curing duration | 5 minutes |
| Material | Grey V5 |
| Observed change | Slightly harder and less elastic |
| Curing equipment | [Enter equipment used] |

<img width="2284" height="3712" alt="IMG_1987" src="https://github.com/user-attachments/assets/f01b2ced-f444-47d1-aca3-dea58a689287" />

<img width="2284" height="3712" alt="IMG_1988" src="https://github.com/user-attachments/assets/ef1e1104-0e90-42b5-afe5-14eb06b3392e" />

Pictures of the parts after 3D printing:

<img width="1024" height="2032" alt="IMG_1984" src="https://github.com/user-attachments/assets/d13074d3-1f83-434b-bb6b-09330614f789" />

<img width="2284" height="3712" alt="IMG_1985" src="https://github.com/user-attachments/assets/16a0568d-1d75-450c-9b70-9d3ed7074be2" />


## Validation:

 1. Snap-Fit Testing

The printed snap-fit components were tested to determine whether the C-shaped cylindrical socket could securely engage with the cylindrical beam. The intended function was for the socket to expand during installation and return toward its original shape to retain the beam.

During testing, the components did not successfully fit together. The cylindrical beam could not properly engage with the semi-circular socket, preventing the snap-fit mechanism from functioning as intended.

 2. Fit Evaluation

The primary issue observed during testing was that the socket geometry did not provide the intended engagement with the cylindrical beam.

The design used a semi-circular opening rather than a more complete circular retaining geometry. This may have contributed to the fitting issue by limiting the amount of contact and retention around the beam.

Additionally, the relatively rigid Grey V5 resin may have made it more difficult for the socket to expand enough during installation, particularly after the curing process reduced its elasticity.

The intended snap engagement was not achieved, so the connection could not be considered secure.

3. Design Limitations and Possible Improvements

Several changes could improve the design in a future iteration:

- **Socket geometry:** Modify the semi-circular clip into a more complete C-shaped circular socket to provide greater contact and retention around the cylindrical beam.
- **Opening diameter:** Adjust the socket opening to provide enough clearance for the beam to enter while maintaining sufficient interference for retention.
- **Wall thickness:** Reevaluate the 0.025-inch wall thickness to determine whether it provides enough flexibility for the selected resin.
- **Material flexibility:** Consider the effect of post-curing on the socket's ability to expand during assembly.
- **Rounded transitions:** Add or increase fillets around the opening to reduce stress concentrations during expansion.

These changes would be evaluated through another CAD iteration and physical print to determine whether they improve engagement and retention.

4. Validation Results

| Test Criteria | Result |
|:---|:---|
| Snap engages securely | No |
| Cylindrical beam fits into socket | No |
| Connection provides sufficient retention | Not achieved |
| Repeated assembly testing | Not possible |
| Design adjustments required | Yes |
| Primary suspected issue | Semi-circular clip geometry |

5. Validation Summary

The initial snap-fit design did not achieve the intended connection between the cylindrical beam and socket. Testing showed that the semi-circular clip geometry did not provide the required engagement.

This highlighted the importance of designing the socket opening and retaining geometry around the actual dimensions of the mating cylindrical component. The results also demonstrated how material properties affect snap-fit performance, particularly when using a relatively rigid SLA resin.

Although the initial design was unsuccessful, the testing identified areas for improvement. A future iteration would focus on modifying the socket geometry, adjusting the opening dimensions, and evaluating the flexibility required for successful assembly.

## Lessons Learned:

Throughout this project, I learned that designing snap-fit parts for SLA printing requires more consideration than simply making two components fit together in CAD. The design must account for resin flexibility, dimensional accuracy, shrinkage, and clearance. My original design did not snap together successfully. This showed me that a design can look correct in CAD but still fail when it is printed and assembled.

One of the biggest challenges was designing the snap-fit around the flexibility of Grey V5 resin. Unlike a flexible plastic, the cured resin has limited ability to deform before it becomes damaged. The socket must expand enough for the cylindrical beam to enter without cracking or permanently deforming. My original design used a semi-circular socket, and the beam did not engage properly. In a future design, I would use a more complete C-shaped socket with a controlled entrance opening. I would also add more clearance and flexibility so the design does not rely on a perfect fit.

I also learned that SLA printing requires consideration of dimensional variation and shrinkage. The dimensions entered into CAD are not guaranteed to match the final printed dimensions exactly. Instead of designing the beam and socket with almost no clearance, I would include a small amount of additional space and test different clearances. I would print a small set of test pieces before printing the entire artifact. This would help determine how much adjustment is needed for the specific resin, printer, and orientation.

Print orientation is another important factor. The orientation of a part affects how supports are placed, the surface finish, and potentially the strength of the printed feature. Since snap-fit components experience repeated deformation during assembly, the socket should be oriented to reduce unnecessary support marks and avoid placing critical flexible areas in an unfavorable build direction. I would also consider how the part is positioned during printing and post-processing when designing thin sections.

SLA and FDM snap fits also have different design considerations. FDM parts are built from deposited layers of thermoplastic, so layer direction and bonding can affect how a snap-fit bends and where it may break. SLA parts are formed by curing liquid resin with light. They can produce smoother surfaces and finer details, but many standard resins are more rigid and less forgiving when repeatedly bent. Because of this, an FDM snap-fit may be able to tolerate more bending than a similar design made with a rigid SLA resin. The material must be considered when choosing the wall thickness, opening size, and amount of interference.

Finally, this project showed me that cost and print time are not the only resources that matter. The PreForm estimate for the print was approximately two hours, but the full process also required CAD modeling, preparing the print, washing, curing, and checking the final fit. The wash and cure stages each took approximately five minutes. Additional time was spent troubleshooting the design after the parts failed to snap together. A small test print could have used less resin and time than reprinting the entire design after discovering a fit problem.

Overall, my biggest lesson was to design for realistic manufacturing conditions instead of relying on perfect CAD dimensions. For future designs, I would account for dimensional variation, include extra clearance where needed, and make the snap-fit geometry flexible enough to accommodate small differences between parts. I would also test the beam and socket together before committing to the complete design. This would make the final product more reliable and reduce wasted material, time, and effort.
