Lab 2:
the one design rule I researched, and saw was to limit Minimize Supports and Optimize Orientation:
My research along with personal expiernce while 3d printing has led me to learn that the more support you have to use the worst looking and more wasteful your design becomes. a way to fix this s orientating your part to be flat or use less supports will lead to your part being less warped. 

source: https://www.addmangroup.com/wp-content/uploads/2024/08/ADDMAN_DfAM-Guide2024.pdf

## FDM specific consideration
I chose overhangs because I think they are interesting and provide a challenge for designers. Some easy ways to work around overhangs are reducing steep angles, rotating the part, or adding supports when necessary. Basically, the designer can either make the overhang easier for the printer to build or orient the part so the overhang can be built up layer by layer instead of printing straight out into empty space.

Source: Prusa Research, Overhangs and bridges.
 ## Morgans/Lexies notes:
 Starting with nothing: need to optimize designs. Not using as much material.
 
 Bridging: connecting two points together with a connecting part together. Very similar to overhang just connecting the 2 points instead of having one side open.


## Lab #2 Make Something Small

## Download
<img width="700" height="700" alt="Screenshot 2026-08-28 210720" src="https://github.com/user-attachments/assets/d08f7c1f-3dc9-44d5-8f27-a2003b45cff2" />

The first print I considered was the model shown above. I ultimately decided against it because I thought it would be somewhat wasteful to print. In order to make the model a reasonable size, it would require a significant amount of material and would also take a long time to print.

The print I ultimately chose was a table hockey puck, which was similar to the first model but had a much flatter design.

<img width="700" height="700" alt="Screenshot 2026-08-28 210918" src="https://github.com/user-attachments/assets/9858ad2d-1fe2-49bc-b5b0-f4f2cdec204b" />

I chose this model for two main reasons. First, I am an avid hockey fan, so I thought it would be more interesting to print something related to one of my interests. Second, the flatter geometry required less material and resulted in a shorter print time. This made the hockey puck a more efficient choice and reduced the amount of time our group collectively needed to spend printing. I only considered two designs because we had limited time and needed the print to finish within the 40-minute constraint.

## Preprocessor

Since a hockey puck has a flat top and bottom, I decided to keep the puck flat against the build plate. This orientation made the most sense because it provided a stable base for the print and did not require the model to be rotated into a more complicated orientation.

I also scaled the puck down to around half of its original size. I did this because our prints had to fit within a 40-minute time constraint. Making the puck smaller reduced the amount of material needed and significantly reduced the print time. This also allowed enough space and time for Lexie's and Morgan's prints to be included in the same printing process.

<img width="700" height="700" alt="Screenshot 2026-08-28 211743" src="https://github.com/user-attachments/assets/dc5f228a-71bc-4167-8081-80324d5500a7" />

The bottom row in the screenshot above shows the scaling changes I made to the model. I adjusted the dimensions until the puck was small enough to meet the time requirement while still being large enough to function as a table hockey puck.

<img width="686" height="402" alt="Screenshot 2026-08-28 211952" src="https://github.com/user-attachments/assets/532e9e7c-459e-4eed-83a6-aff8ecfb086f" />

This is the Sliced Info for my puck:

After slicing the puck in PrusaSlicer, the estimated printing time was 19 minutes in normal mode and 21 minutes in stealth mode. The print used approximately 10.16 g of PETG filament, or 3.33 m of filament, with an estimated material cost of $0.28.

<img width="444" height="326" alt="image" src="https://github.com/user-attachments/assets/f1704d7d-b51c-46d8-af00-e40107bb6452" />

And the estimated time for each section: 

<img width="646" height="602" alt="image" src="https://github.com/user-attachments/assets/d5daffff-4096-4e5a-8155-60b649e675cc" />


Given that my design was flat and had no significant overhangs, supports were not needed. Therefore, I chose not to use supports for the print. This also helped reduce the amount of material used and kept the print time lower.

At the beginning of the process, I got confused about how to select the correct printer and material in PrusaSlicer. I had to spend some time figuring out which settings to use before continuing with the print. After figuring it out, I was able to continue with the rest of the process without any major issues. This taught me that selecting the correct printer and material is an important first step before preparing a model for printing.

## Print 

My group used Printer PL-05, which uses PETG filament.

My group consisted of Morgan Gregory and Lexie Cox. We printed our parts together to make the most efficient use of the printer and stay within the available printing time.

Video of our prints being created:

https://drive.google.com/file/d/1xxeeVpDYUkhXcl_19Z5VeJgylWNX0_UJ/view

<iframe src="https://drive.google.com/file/d/1xxeeVpDYUkhXcl_19Z5VeJgylWNX0_UJ/preview" width="100%" height="500" allow="autoplay"> </iframe>


<img width="3024" height="4032" alt="IMG_1390" src="https://github.com/user-attachments/assets/f7079f10-2689-41ed-a74b-f40c776b5ccb" />

My print did not come out quite as well as I originally expected. I believe this was partly because the model was essentially a disk with only a slight change in height, and I had scaled it down to a very small size. This made the small changes in height and geometry more difficult for the printer to reproduce clearly.

<img width="3024" height="4032" alt="IMG_1392" src="https://github.com/user-attachments/assets/4fb53ac7-8f77-4550-9391-62f4a3381c77" />

## What did I learn? 
I already had a basic understanding of how 3D printers worked before this lab, but I still learned some important things from the printing process. One of the biggest things I learned was that I need to be careful when designing small parts with small dips or changes in height. When a model is scaled down too much, these small features may not be reproduced clearly by the printer, which can cause the final print to look different from how I originally envisioned it.

I also learned how to download an STL file and import it into PrusaSlicer. This gave me more experience with the process of taking a model from an online source and preparing it for 3D printing.
