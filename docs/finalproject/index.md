# Final Project – Multilevel jewelry Holder 

## Objectives

Choose a problem that can be addressed with 3D printing/laser cutting and develop an initial design concept.

## Problem to Solve

The problem I am trying to solve with this project is that my sister needs more space to store her jewelry because she has run out of room on her current jewelry holder. Her existing holder does not provide enough storage or organization for all of her accessories. To solve this problem, I plan to design and manufacture an all-in-one jewelry holder that can store multiple types of jewelry, including earrings, bracelets, necklaces, and other small accessories. The design will focus on maximizing storage space while keeping everything organized, accessible, and easy to use. I also want the holder to be visually appealing so that it can serve as both a functional storage solution and a decorative piece for her room.

## Part 1

## Research: 

### 1.1 Spiral Design Process

The Spiral Design Process is an iterative engineering design approach that focuses on developing, testing, and improving a product through multiple design cycles. Rather than expecting the initial design to work perfectly, the process allows potential problems to be identified early and addressed through repeated evaluation and refinement.

The process consists of four main categories:

1. **Planning:** Establish the project's objectives, requirements, and design goals. Determine what needs to be accomplished during each design cycle.
2. **Risk Analysis:** Identify potential design and manufacturing problems that could affect the final product. Evaluate possible solutions before committing to a specific design.
3. **Engineering:** Develop the design through CAD modeling, material selection, prototyping, and manufacturing.
4. **Evaluation:** Test the prototype against the original requirements. Analyze the results, identify areas for improvement, and determine what changes should be made during the next design cycle.

**Application to My Project:**

I will use the Spiral Design Process to develop my jewelry holder through multiple design iterations. The initial design will focus on establishing the overall structure and determining how the different jewelry storage components will fit together.

After manufacturing the first prototype, I will evaluate potential issues such as insufficient storage space, structural weakness, and difficulty installing or removing the laser-cut jewelry bars. These findings will guide improvements to subsequent versions.

For example, if the laser-cut bars fit too loosely inside the FDM-printed frame, I can adjust the slot dimensions and manufacture another test piece before producing the entire holder. This approach will help reduce wasted materials and improve the functionality of the final design.

### 1.2 FDM Anisotropy

Fused Deposition Modeling (FDM) is an additive manufacturing process that produces parts by depositing melted thermoplastic filament in individual layers. Because the material is deposited in specific directions and bonded to previously printed layers, FDM parts do not have identical mechanical properties in every direction. This behavior is known as **anisotropy**.

FDM-printed parts are generally stronger along continuous filament paths than they are across layer boundaries. This is because the bonding between individual layers can be weaker than the filament material itself. As a result, parts may be more susceptible to separating or fracturing when loads act perpendicular to the printed layers.

**Application to My Project:**

The FDM-printed frame will support the weight of the jewelry and hold the removable laser-cut bars in position. Therefore, print orientation and layer adhesion will be important considerations when designing the frame.

For example, the slots that support the removable bars will experience forces from the weight of the jewelry and from repeatedly inserting and removing the bars. If these areas are not designed properly, the printed layers could separate over time.

Several strategies can be used to improve the strength of FDM components:

- **Print Orientation:** Position the part to minimize loads acting perpendicular to layer boundaries.
- **Infill Density:** Increase infill where additional internal support is needed.
- **Wall Thickness:** Add perimeter walls around slots and connection points to improve structural strength.
- **Material Selection:** Consider materials such as PLA for general structural and decorative components or PETG when additional toughness and flexibility are beneficial.
- **Layer Adhesion:** Use appropriate printing temperatures and settings to improve bonding between layers.

Understanding anisotropy will help me determine the best print orientation and manufacturing settings for producing a durable jewelry holder.

### 1.3 SLA Shrinkage

Stereolithography (SLA) is an additive manufacturing process that uses light to cure liquid photopolymer resin into solid layers. Although SLA printing can produce highly detailed parts with good dimensional accuracy, shrinkage can occur as the resin cures and undergoes post-processing.

Shrinkage occurs because the chemical reactions involved in converting liquid resin into a solid polymer cause the material to contract. Additional dimensional changes can occur during UV post-curing as the material continues to polymerize.

**Important Considerations:**

- Shrinkage varies depending on the resin formulation.
- Some photopolymer resins report approximately 3–10% volumetric shrinkage, although this is not a universal value.
- Post-curing can cause additional dimensional changes.
- Part geometry, orientation, and curing conditions can influence dimensional accuracy.
- Different resin formulations have different shrinkage characteristics.

It is important to distinguish between volumetric and linear shrinkage. For example, 5% volumetric shrinkage does not mean that every individual dimension will decrease by 5%.

**Strategies for Managing Shrinkage:**

1. Select a resin with suitable dimensional stability.
2. Follow the manufacturer's recommended washing and curing procedures.
3. Measure parts after post-processing rather than relying entirely on their original CAD dimensions.
4. Manufacture test pieces to determine the actual dimensional changes.
5. Apply dimensional compensation when consistent shrinkage has been measured.

**Application to My Project:**

My primary design will use FDM printing for the main structure and laser cutting for the removable jewelry bars. However, understanding SLA shrinkage is important when comparing different manufacturing processes and considering alternative ways to manufacture components.

If SLA printing were used for any components requiring precise connections, shrinkage could affect the dimensions of slots and mating surfaces. This could cause parts to become too tight or too loose during assembly.

For this reason, any SLA components would need to be measured after washing and curing to ensure that the final dimensions meet the design requirements.

### 1.4 Laser Cutting Kerf

Kerf is the amount of material removed by a laser during the cutting process. Although the laser follows a specific path defined by the CAD drawing, it removes a small amount of material around that path. This causes the final dimensions of the cut component to differ slightly from the original design.

Typical laser kerf widths can range from approximately 0.1–0.3 mm, depending on the material, thickness, laser focus, and machine settings.

Kerf affects different features in different ways:

- **Outside Dimensions:** Material is removed from the edges, making the finished part slightly smaller.
- **Internal Cutouts:** Material is removed from the inside edges, making holes and slots slightly larger.
- **Tabs and Slots:** Components designed with identical CAD dimensions may not fit together as intended.

**Methods for Compensating for Kerf:**

1. **Kerf Measurement:** Cut a test pattern using the intended material and laser settings. Measure the resulting dimensions to determine the actual kerf.
2. **Offset Compensation:** Adjust the CAD drawing or laser software to account for the material removed during cutting.
3. **Test Fits:** Manufacture small test pieces with different slot widths to determine the dimensions that produce the desired fit.
4. **Tolerance Adjustments:** Include additional clearance when designing components that need to slide together or be repeatedly removed.

**Application to My Project:**

Kerf compensation will be especially important because I plan to use laser-cut bars that slide into openings in the FDM-printed frame. These bars will contain small holes for holding earrings, making dimensional accuracy important for both storage and assembly.

The connection between the laser-cut bars and the printed frame will require particular attention. If the slots are too large, the bars may move around or fall out. If the slots are too small, the bars may not fit into the frame.

To address this, I plan to manufacture a small test piece containing several different slot widths. I can then compare the fits and determine the appropriate clearance before manufacturing the final jewelry bars.

### 1.5 Research Conclusion

The research identifies several manufacturing considerations that will influence the design and development of my jewelry holder.

| Research Topic | Design Consideration |
|---|---|
| Spiral Design Process | Develop, test, evaluate, and improve the design through multiple iterations. |
| FDM Anisotropy | Select an appropriate print orientation and strengthen areas that experience repeated loading. |
| SLA Shrinkage | Account for possible dimensional changes when designing components that require precise fits. |
| Laser Cutting Kerf | Measure kerf and adjust slot dimensions to achieve a reliable sliding fit. |

The most important manufacturing consideration for my project will be ensuring that the FDM-printed frame and laser-cut bars fit together correctly. Since these components will be manufactured using two different processes, their original CAD dimensions may not produce the intended fit.

I will need to manufacture test pieces, measure the results, and adjust the design accordingly. Applying these research findings throughout the design process will help reduce manufacturing errors, minimize wasted materials, and improve the functionality of the final jewelry holder.

## 2. Problem Definition

I identified three everyday problems that could be addressed through product design and manufacturing.

### 2.1 Limited Jewelry Storage
My sister has run out of room on her current jewelry holder. She needs additional space to organize earrings, bracelets, necklaces, and other accessories.

### 2.2 Disorganized Desk Storage
Small items such as pens, tools, and USB drives can clutter a workspace when they do not have designated storage locations. A compact desk organizer could help keep these items organized.

### 2.3 Limited Accessory Storage
Smaller personal accessories, such as watches, hair clips, and rings, can easily become disorganized or misplaced. A dedicated storage solution could make these items easier to organize and access.

## 3. Problem Selection

### Selected Problem: Limited Jewelry Storage

I selected the jewelry storage problem because my sister needs a larger and more organized way to store her accessories. I want to create an all-in-one holder that accommodates earrings, bracelets, necklaces, and smaller items.

I plan to use FDM printing for the main structure and laser cutting for removable jewelry bars. This combination will allow me to create a functional design while exploring how different manufacturing processes can work together.

## 4. Concept Development

### Initial Design

My concept is a vertically oriented jewelry holder with multiple storage sections. The main structure will be FDM printed, while laser-cut bars will slide into openings in the frame to hold earrings.

Additional sections will provide storage for bracelets, necklaces, and smaller accessories.

Here were some pictures of my example images that I baised my design after:

<img width="1180" height="1572" alt="C673F42D-B97D-4A9C-8979-829D7ECF05A7" src="https://github.com/user-attachments/assets/cb2c4018-dd3d-4ebb-8867-f3e9f4ee87fd" />

<img width="603" height="1311" alt="Screenshot 2026-11-15 at 9 43 45 PM" src="https://github.com/user-attachments/assets/c68016c0-7fb9-4a09-8e62-9eb7fccd4b2d" />

<img width="2024" height="3032" alt="IMG_2006" src="https://github.com/user-attachments/assets/70a057fa-f995-456d-a42b-b23f92592835" />

My idea is to combine the staircase like design of the first image with the top bars for bracelets and necklaces from the 2nd and third images. The idea is to combine two great ideas into one. 

### CAD Development

I will develop the design in CAD and make adjustments based on peer feedback and manufacturing limitations. Important considerations include structural strength, print orientation, material thickness, and clearances between the printed frame and laser-cut bars.

Rough CAD design: 

<img width="922" height="796" alt="image" src="https://github.com/user-attachments/assets/64326dfb-70fb-4f68-a581-6e33149b4060" />

## 5. Testing Critical Features

The main feature I need to test is the connection between the FDM-printed base and laser-cut bars.

I plan to manufacture the base first and measure its actual openings using calipers. I will then use those measurements to design the laser-cut bars, accounting for material thickness and laser kerf.

After cutting the bars, I will test their fit to ensure they slide into the base without excessive force while remaining secure enough to support jewelry. If necessary, I will adjust the dimensions before manufacturing the final components.

## 6. Video Presentation

https://github.com/user-attachments/assets/24c330b1-11e5-4a51-bfb0-7d4c82b1594d

## Part 2
