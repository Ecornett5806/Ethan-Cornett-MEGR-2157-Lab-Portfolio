# A10 RC2 Sliding fit 

## Objective
Design and fabricate a pair of parts (a hole/slot feature and a matching shaft/insert feature) that demonstrate an RC 2 sliding fit on a SLA print

Research: 

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


## Communicate

