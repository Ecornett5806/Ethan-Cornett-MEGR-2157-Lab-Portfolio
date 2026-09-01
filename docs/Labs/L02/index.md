Lab 2:
the one design rule I researched, and saw was to limit Minimize Supports and Optimize Orientation:
My research along with personal experience while 3d printing has led me to learn that the more support you have to use the worst looking and more wasteful your design becomes. a way to fix this s orientating your part to be flat or use less supports will lead to your part being less warped. 

source: https://www.addmangroup.com/wp-content/uploads/2024/08/ADDMAN_DfAM-Guide2024.pdf

## FDM specific consideration
I chose overhangs because I think they are interesting and provide a challenge for designers. Some easy ways to work around overhangs are reducing steep angles, rotating the part, or adding supports when necessary. Basically, the designer can either make the overhang easier for the printer to build or orient the part so the overhang can be built up layer by layer instead of printing straight out into empty space.

Source: Prusa Research, Overhangs and bridges.

 ## Morgans/Lexies notes:
 Starting with nothing: need to optimize designs. Not using as much material.
 
 Bridging: connecting two points together with a connecting part together. Very similar to overhang just connecting the 2 points instead of having one side open.


## Lab #2 Make Something Small

## Download

This is the website that we were told to use: 

(https://www.printables.com/)

<img width="700" height="700" alt="Screenshot 2026-08-28 210720" src="https://github.com/user-attachments/assets/d08f7c1f-3dc9-44d5-8f27-a2003b45cff2" />

Link to the first print- https://www.printables.com/model/138235-hockey-puck

The first print I considered was the model shown above. I ultimately decided against it because I thought it would be somewhat wasteful to print. In order to make the model a reasonable size, it would require a significant amount of material and would also take a long time to print. Since our group had a 40-minute time limit and needed to print multiple designs, I decided that the amount of material and printing time required for this model would make it impractical. I therefore looked for a smaller and simpler design that could still be interesting to print while better fitting our time and material constraints.

The print I ultimately chose was a table hockey puck, which was similar to the first model but had a much flatter design. I finally decided to choose this print because it seemed like a better balance between something I wanted to print and something that would work within our time constraints. The flatter design meant that it would use less material and take less time to print. This was important because our group had a 40-minute limit and also needed to leave enough time for Lexie's and Morgan's prints.

Another reason I chose the hockey puck was because I am an avid hockey fan. I thought it would be more interesting to print something related to one of my interests rather than choosing a random model. Overall, the hockey puck seemed like the better option because it was both practical to print and personally interesting to me.

[https://www.printables.com/model/276011-replacement-air-hockey-table-puck)](https://www.printables.com/model/276011-replacement-air-hockey-table-puck)

<img width="700" height="700" alt="Screenshot 2026-08-28 210918" src="https://github.com/user-attachments/assets/9858ad2d-1fe2-49bc-b5b0-f4f2cdec204b" />

I chose this model for two main reasons. First, I am an avid hockey fan, so I thought it would be more interesting to print something related to one of my interests. Second, the flatter geometry required less material and resulted in a shorter print time. This made the hockey puck a more efficient choice and reduced the amount of time our group collectively needed to spend printing. I only considered two designs because we had limited time and needed the print to finish within the 40-minute constraint.

## Preprocessor

Since a hockey puck has a flat top and bottom, I decided to keep the puck flat against the build plate. This orientation made the most sense because it provided a stable base for the print and did not require the model to be rotated into a more complicated orientation.

I also scaled the puck down to around half of its original size. I did this because our prints had to fit within a 40-minute time constraint. Making the puck smaller reduced the amount of material needed and significantly reduced the print time. This also allowed enough space and time for Lexie's and Morgan's prints to be included in the same printing process.

The main tradeoff with scaling the puck down was that reducing its size also reduced the amount of space available for its smaller features. At the time, I prioritized meeting the printing time requirement, but the final print showed that scaling it down too much affected the definition of some of the details. This became something I would consider differently in a future print.

<img width="1206" height="758" alt="Screenshot 2026-08-31 191637 (1)" src="https://github.com/user-attachments/assets/7eddf1e4-7b15-4895-b51e-2578712e0a1a" />

The bottom row in the screenshot above shows the scaling changes I made to the model. I adjusted the dimensions until the puck was small enough to meet the time requirement while still being large enough to function as a table hockey puck.

<img width="472" height="282" alt="Screenshot 2026-08-31 211105" src="https://github.com/user-attachments/assets/faebc246-17f3-41f2-921f-72228a66664a" />

This is the Sliced Info for my puck:

After slicing the puck in PrusaSlicer, the estimated printing time was 9 minutes in normal mode and 10 minutes in stealth mode. The print used approximately 1.34 g of PETG filament, or .44 m of filament, with an estimated material cost of $0.04.

And the estimated time for each section: 

<img width="1917" height="913" alt="Screenshot 2026-08-31 212605" src="https://github.com/user-attachments/assets/51082b51-8550-428a-89fc-ad66754ad9c5" />

Given that my design was flat and had no significant overhangs, supports were not needed. Therefore, I chose not to use supports for the print. This also helped reduce the amount of material used and kept the print time lower.

At the beginning of the process, I got confused about how to select the correct printer and material in PrusaSlicer. I had to spend some time figuring out which settings to use before continuing with the print. After figuring it out, I was able to continue with the rest of the process without any major issues. This taught me that selecting the correct printer and material is an important first step before preparing a model for printing.

Another mistake we made as a group was scaling our prints down too much, which made the designs less precise. In my print's case, this also made the final product not look as good as it could have if it had been given more surface area. I think this was partly due to the 0.4 mm nozzle size. Because the nozzle deposits material in relatively large lines compared to some of the small features on the model, it cannot reproduce extremely small and precise details as well. The air hockey puck had a small divot that separated the flat portion on the bottom from the raised portion of the puck. When we scaled the model down, this feature became very small compared to the nozzle size, causing the transition between the two sections to lose some of its definition. If we had printed the puck at a larger scale, the nozzle would have had more space to reproduce this feature, resulting in a cleaner and more precise final print.

## My Role in the Printing Process
I was not put in charge of operating the 3D printer. However, throughout the printing process, I completed the part that I was responsible for. I found my model and adjusted it to a reasonable size so that all three prints could be completed within the 40-minute time limit. I also prepared my model in PrusaSlicer and made the necessary adjustments before it was printed.

## Print 

My group used Printer PL-05, which uses PETG filament.

My group consisted of Morgan Gregory and Lexie Cox. We printed our parts together to make the most efficient use of the printer and stay within the available printing time.

Video of our prints being created:

https://github.com/user-attachments/assets/2685956a-0aca-4a02-a47d-ffd0628e7aca

<img width="3024" height="4032" alt="IMG_1390" src="https://github.com/user-attachments/assets/f7079f10-2689-41ed-a74b-f40c776b5ccb" />

My print did not come out quite as well as I originally expected. I believe this was partly because the model was essentially a disk with only a slight change in height, and I had scaled it down to a very small size. This made the small changes in height and geometry more difficult for the printer to reproduce clearly.

<img width="3024" height="4032" alt="IMG_1392" src="https://github.com/user-attachments/assets/4fb53ac7-8f77-4550-9391-62f4a3381c77" />

## What did I learn? 
I already had a basic understanding of how 3D printers worked before this lab, but I still learned some important things from the printing process. One of the biggest things I learned was that I need to be careful when designing small parts with small dips or changes in height. I also learned the importance of keeping the scale of a model reasonable so that the 0.4 mm nozzle can accurately reproduce its smaller features. By scaling the puck down too much, the small dips and changes in height became difficult for the printer to reproduce clearly. Keeping the model at a larger scale would have given these features more room to be printed accurately, which would have resulted in a cleaner-looking puck.


I also learned how to download an STL file and import it into PrusaSlicer. This gave me more experience with the process of taking a model from an online source and preparing it for 3D printing.

Finally, I learned the importance of choosing the correct build orientation. Keeping the puck flat against the build plate provided a stable base and allowed the model to be printed without supports. This showed me that choosing the right orientation can make a print simpler while also reducing the amount of material and time required.
I learned the difference between having a print completed quickly and having a print completed well. While it is important to finish a print in a reasonable amount of time, making it too small or rushing the process can negatively affect the quality of the final product. I learned that the goal is to find a balance between print time and print quality so that the part is completed in a timely manner without sacrificing important details or features.



Actual Time: The total time from downloading the model to completing the print was approximately 30–35 minutes. Morgan Gregory and Lexie Cox were my partners throughout this process. We worked together to prepare and print our models while making sure all three prints could be completed within the 40-minute time constraint.

## Resources

(https://www.printables.com/) - Used to find and download the 3D model for the print.

(https://www.addmangroup.com/wp-content/uploads/2024/08/ADDMAN_DfAM-Guide2024.pdf) - Used as a reference for the Pre-Lab questions.
