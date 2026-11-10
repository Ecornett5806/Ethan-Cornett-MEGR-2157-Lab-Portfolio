# A11 – Motor Selection

## Objective

The objective of this project is to design and 3D print a small clip-on shelf using the Form 4 SLA printer. The shelf will attach to an existing platform using two integrated C-shaped snap-fit clips. These clips will flex during installation and securely grip the platform, allowing the shelf to be attached and removed without additional hardware. The design focuses on creating a functional snap-fit mechanism while considering material properties, dimensional tolerances, flexibility, and durability.

## Analyze:

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

<img width="2560" height="1600" alt="image" src="https://github.com/user-attachments/assets/efd1966f-f0b2-4e34-b374-4fa40f1662f7" />
