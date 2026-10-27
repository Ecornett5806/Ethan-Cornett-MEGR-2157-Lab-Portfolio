# A9 – Lazer Cutter: 

## Objective 

In a group of 2-3 Design, laser cut, assemble, and document a parametric construction kit that accounts for laser cutter kerf. What you build is up to your team.
The kit must include At least 3 unique part types. At least 8 total pieces. At least one press fit, slot fit, or tab fit connection. Evidence that you measured kerf and used it to set your fits and clearances. My group consisted of Morgan Gregory, Lexie Cox, and I. 

## Analyze: 

## Step 1: Measure your material:
We need to know what the thickness of the boards we are making our designs out of.  
Thickness: 
### Material Thickness Measurements

| Sheet | Thickness (in) | Thickness (mm) |
|:-----:|---------------:|---------------:|
| 1     | 0.1050         | 2.667          |
| 2     | 0.1080         | 2.743          |
| 3     | 0.1070         | 2.718          |
| **Mean** | **0.1067**  | **2.709**      |

## Step 2: Measure the kerf of a 20mm-by-20mm square:

### Kerf Measurements

| Measurement | X Direction (mm) | Y Direction (mm) |
|:------------|-----------------:|-----------------:|
| Nominal square size | 20.00 | 20.00 |
| Measured cut size | 19.90 | 19.98 |
| **Dimensional difference** | **0.10** | **0.02** |

### Kerf Calculation

| Direction | Calculation | Result (mm) |
|:----------|:------------|------------:|
| X | 20.00 - 19.90 | 0.10 |
| Y | 20.00 - 19.98 | 0.02 |


Step 3: 

### Fit Test Calculations

| Fit Type | Equation | Clearance Adjustment |
|:---------|:---------|---------------------:|
| Tight Fit | `D = t_average + x_0 - K_k - 0.05 mm` | -0.05 mm |
| Target Fit | `D = t_average + x_0 - K_k` | 0.00 mm |
| Loose Fit | `D = t_average + x_0 - K_k + 0.05 mm` | +0.05 mm |

Fit Test

<img width="417" height="206" alt="image" src="https://github.com/user-attachments/assets/1b84c188-337d-4bdd-8173-0323797612a7" />

## Step 4: Choose your clearance.
Choosing the Clearance
The fit test showed that the best clearance was between the 0 and .005 mm range. The chosen clearance was .002 in order to balance having too much clearance and too little. This will allow the parts to fall in with only minor pressure but will prevent them from falling apart easily.

Designing the Final Cut
To begin the final cut I decided to add my parameters into SolidWorks.

<img width="1342" height="342" alt="image" src="https://github.com/user-attachments/assets/81959fc8-715c-4f00-ad7f-c1e4955eb9f4" />


Next I created a sketch for the square shaped piece to be designed, which is shown below, after I put the parameters and equations in. I made sure all side lengths that needed to be equal were, and I used the x and y kerf differences when calculating the x and y widths. The x widths are slightly smaller because there was more kerf meaning more material will get burned away during the cutting process.

## Manufacturing, including Process Research:

1. Open all vents to allow proper airflow. Ensure the handles are parallel.
2. Turn on the pump beneath the printer.
3. Turn on the laser cutter.
4. Center the material and allow the machine to complete its automatic alignment.
5. Connect the machine to the computer.
6. Open the design in Inkscape and press `Ctrl + P` to open the print dialog.
7. Send the design to the Epilog laser cutter and select the appropriate material settings.
8. Press **Start** to begin cutting.
9. Allow the laser cutter to finish the job.
10. Wait for most of the smoke to clear while the exhaust system continues running.
11. Once it is safe to open the machine, retrieve the cut parts.

### Laser Process Record

| Setting | Kerf Coupon | Fit Coupon | Final Cut |
|:---|:---|:---|:---|
| Laser cutter (#4) | #4 | #4 | #4 |
| Material type |wood |wood | wood |
| Nominal thickness | 1/8th inch | 1/8th inch | 1/8th inch |
| Measured thickness (mean) | 2.709 mm | 2.709 mm | 2.709 mm |
| Speed | 20% | 20% | 20%|
| Power | 100% | 100% |100%|
| Frequency or PPI (if applicable) | 20% | 20% |20% |
| Number of passes | 1 | 1 | 1 |
| Focus method and how you confirmed it | Vector | Vector| Vector |
| Air assist on? Exhaust on? | Yes | Yes | Yes |
| How you set origin and alignment | Auto focus | Auto Focus | Auto Focus |

<img width="596" height="772" alt="Screenshot 2026-10-26 144114" src="https://github.com/user-attachments/assets/a8c7a498-c1f4-43dc-add3-fe71e7b73fb2" />

<img width="862" height="808" alt="image" src="https://github.com/user-attachments/assets/1e08a7de-4694-44a9-9987-c81d7834584e" />

<img width="875" height="643" alt="image" src="https://github.com/user-attachments/assets/4c5a94a9-edc6-4d63-99a7-a16e991589d8" />

<img width="813" height="603" alt="image" src="https://github.com/user-attachments/assets/97d9e136-e071-4bed-884a-d332890864ff" />

## Lessons Learned

10/23/26 - Completed Steps 1 and 2 and the documentation for these steps. This took roughly 2 hours.

10/26/26 - Completed Steps 3-4 and designed the pieces to be cut out and the documentation for these steps. This took roughly 3 hours.

10/27/26 - Performed final cut and finished documentation. This took roughly 1 hour.

I learned several lessons throughout this project.

Writing




## REFLECTION: Questions 

Reflection 1: Measured Values Versus Assumptions
The material was labeled with a nominal thickness, but my measurements showed that the actual thickness varied between sheets. The three measurements were 0.105 in, 0.108 in, and 0.107 in, giving an average thickness of approximately 0.1067 in (2.709 mm). My 20 mm kerf coupon also measured 19.90 mm in the X direction and 19.98 mm in the Y direction, producing dimensional differences of 0.10 mm and 0.02 mm, respectively. These results showed that the material and cutting process did not produce exactly the nominal dimensions. If I had relied on assumed values instead of measurements, my slots and tabs could have been too tight or too loose, making assembly more difficult or causing the joints to fit together unreliably.

Reflection 2: Taguchi's Quality Loss Function
Taguchi's quality loss function explains that a product can create a loss when its performance differs from the intended target, even if it still functions. In my construction kit, the tab-and-slot joint is an example of a feature that needs to fit close to its intended clearance. A joint that fits but requires more pressure than intended, or one that is slightly loose, does not achieve the target fit. If thousands of these parts were manufactured, small dimensional variations could lead to inconsistent assembly, increased labor, rework, and wasted material. Testing different clearances before the final cut helped reduce the chance of these problems.

Reflection 3: Real-World Application
Flat-pack furniture is a real-world example of a product that uses sheet parts joined through tabs, slots, and other fitted connections. The dimensions of these features affect how easily the furniture can be assembled and how securely the pieces connect. If the material is thicker than expected or the laser kerf is not properly accounted for, the slots may be too narrow or too wide. Customers could experience difficulty assembling the furniture, loose connections, misaligned panels, or reduced stability. Measuring the material and testing the fit before production helps prevent these problems.

Reflection 4: One More Cut
If I had one more cut, I would make another fit coupon with smaller clearance increments around the selected 0.002 in (0.0508 mm) clearance. This would allow me to compare the joint fits more precisely and determine whether a slightly tighter or looser fit provides the best balance between easy assembly and connection strength. I would measure and test each joint, record the results, and use the best-performing clearance in the final CAD model. This additional test could improve fit consistency and reduce the need for adjustments during assembly.
