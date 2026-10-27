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
| Speed | 30% | 30% | 30%|
| Power | | | |
| Frequency or PPI (if applicable) | | | |
| Number of passes | | | |
| Focus method and how you confirmed it | | | |
| Air assist on? Exhaust on? | | | |
| How you set origin and alignment | | | |

<img width="596" height="772" alt="Screenshot 2026-10-26 144114" src="https://github.com/user-attachments/assets/a8c7a498-c1f4-43dc-add3-fe71e7b73fb2" />

Lessons Learned

10/23/26 - Completed Steps 1 and 2 and the documentation for these steps. This took roughly 2 hours.

10/26/26 - Completed Steps 3-4 and designed the pieces to be cut out and the documentation for these steps. This took roughly 3 hours.

10/27/26 - Performed final cut and finished documentation. This took roughly 1 hour.

I learned several lessons throughout this project.
