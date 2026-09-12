# A4: Benchmark a Parameter - Hole Diameter. 

# Design process first attempt: 

## CAD Design #1

<img width="392" height="668" alt="image" src="https://github.com/user-attachments/assets/02dba8bd-5a75-4b2c-ac58-006b105f599e" />

The picture below shows my first attempt at designing the benchmark artifact. My idea was to make a domino-shaped test piece with progressively smaller holes. A domino is a simple rectangular shape that already uses circular holes in different patterns, so I thought it would be a good way to keep the design simple while still making the benchmark more interesting than just a basic test block.

The hole diameters would get smaller as they moved across the domino. This would allow me to test the minimum hole diameter that the Prusa Core One could reliably print. I chose this design because it gave me a simple and recognizable shape while also giving me a practical way to test the printer's limits. I wanted the artifact to be something that looked intentional while still giving me useful measurements from the print.

The first attempt did not work the way I expected. The hole locations and circular features were present in the CAD model, but the smaller holes did not stay open once the part was printed. This showed me that just having the correct geometry in CAD does not necessarily mean the printer will be able to reproduce that geometry physically. The failed print gave me a starting point for figuring out what needed to be changed for my second attempt.

The first printed artifact shows that the printer recognized where the smaller holes were supposed to be, but it could not keep them open during the print. The circular features are still visible on the surface, which shows that the printer was following the general geometry of the CAD model. However, because the holes were so small, the openings became partially or completely closed.

This was interesting because the FDM Design Rules provided for the class listed 2 mm as the minimum hole diameter. My largest test hole was approximately 2.8 mm, which is larger than the documented minimum. Based on this information, I expected the 2.8 mm hole to print as an open hole. Since it did not, I realized that the actual result could be affected by more than just the hole diameter. Factors such as layer height, extrusion width, print settings, and the geometry of the part could also affect whether a small hole remains open.

Although the first attempt failed to produce the result I wanted, it was still useful for the project. The purpose of this benchmark was to find the practical limit of the Prusa Core One, and the first print showed me that the printer's actual capabilities did not necessarily match the minimum value listed in the design rules. I used what I learned from this attempt to make changes to the design before creating my second version.

<img width="624" height="824" alt="Image_260912_113432" src="https://github.com/user-attachments/assets/b36e63c6-7291-47bc-a315-09c8818d5774" />

## Slicer build parameters:

### Build Orientation
I chose to print the artifact flat on its back because the design is already flat. This orientation allowed the printer to build the part directly on the build plate without requiring supports. I also chose this orientation because it kept all of the test holes in the same orientation, allowing me to focus on hole diameter rather than introducing another variable from printing the holes at an angle. This helped keep the test consistent while also reducing unnecessary support material and print time.

This photo shows Morgan's design and my design before they were sliced in PrusaSlicer. The models are shown in their final build orientation before the printing parameters were applied. This allowed us to check the placement and orientation of each design before moving on to the slicing process.

<img width="982" height="706" alt="Screenshot 2026-09-10 131319" src="https://github.com/user-attachments/assets/e0aaf7ef-ff31-466b-8d96-bfea0fe85d51" />

### Infill

We started by choosing this infill pattern because it provided additional strength and support through the middle of both designs, making the parts stronger and more sturdy during printing and testing. This was especially useful for Morgan's benchmark because he needed to measure the shrinkage of his bars after printing. The infill helped support the bars while still allowing them to be measured after printing. The infill did not have the same effect on my benchmark because I was testing hole diameter rather than the dimensions of the internal structure. We kept the same infill for both designs so that the printing conditions remained consistent.

<img width="612" height="252" alt="Screenshot 2026-09-10 130641 (1)" src="https://github.com/user-attachments/assets/018e160a-db5a-46f3-9928-570470fa4d7d" />

After discussing the infill settings further, we decided to increase the infill by 5%. We made this change to give both parts slightly more internal structure and detail while still keeping the same infill pattern. This allowed us to make the parts more sturdy without making a major change to the overall design.

<img width="632" height="246" alt="Screenshot 2026-09-10 132308" src="https://github.com/user-attachments/assets/a03e8e3c-3d74-48b9-85bf-68d844d5a41c" />

### Supports

I chose not to use supports because the benchmark was designed to print flat on the build plate and did not have any overhangs that required support material. This kept the print simpler and prevented support material from affecting the holes I was testing. Since the goal of the benchmark was to determine the smallest hole diameter the printer could produce, I wanted to avoid adding another factor that could affect the results.

### Scale

We decided not to scale either design down because both designs were already sized to fit on the build plate and were expected to be completed within the required print time. Scaling the designs down would have changed the dimensions of our benchmarks, which could have affected the results. Since both designs already fit within the available space and were expected to take approximately 1 hour and 45 minutes to print, we kept both models at their original 100% scale.

### 1st Slicing
Here are the three slicing photos we documented during our first print: and then the slicing of my second design: 

10% infill:

<img width="917" height="455" alt="Screenshot 2026-09-10 130924" src="https://github.com/user-attachments/assets/653dfbc6-84f1-41a1-be5d-0b89f5a26d5a" />

15% infill:

<img width="917" height="455" alt="Screenshot 2026-09-10 130956" src="https://github.com/user-attachments/assets/cf49bd70-6321-4a76-a5bc-866155f64e7f" />

Final Completed slice: 

<img width="917" height="455" alt="Screenshot 2026-09-10 132109" src="https://github.com/user-attachments/assets/fd047514-679e-434a-af72-be05f7f04d96" />

# CAD Design #2 
After the first attempt, I realized that I needed to make a few changes to the way I approached the benchmark. The first change was revising the starting hole diameter. Since the first design started with holes that were already very close to the expected limit, I wanted to create a wider range of hole sizes so I could better see where the printer started to struggle.

I also changed the units of the overall design from inches to millimeters. Using millimeters allowed me to work with more precise, whole-number dimensions instead of repeatedly converting between inches and millimeters. This made it easier to control the hole sizes and compare my results directly to the 2 mm minimum hole diameter listed in the class FDM Design Rules.

For the second attempt, I started with a 10 mm hole and decreased the diameter by 1 mm for each test hole, continuing down to 2 mm. This gave me a range of hole diameters from 10 mm to 2 mm and allowed me to gradually approach the documented minimum instead of immediately starting near the limit.

The results of the second print showed that the printer was able to produce the larger holes consistently, but its performance became increasingly inconsistent as the diameter decreased. Once the holes reached approximately 5 mm and below, the printer began having difficulty reproducing them accurately. The 4 mm hole was visible and open, but only barely, while the 3 mm hole did not print properly. Based on these results, Based on these results, the practical minimum for my particular print setup appears to be approximately 4 mm, rather than the 2 mm value listed in the design rules.

This was different from my original prediction. I initially expected the printer to successfully produce a 2 mm hole because the class design rules listed it as the minimum. The second attempt showed that the documented value should be treated as a guideline rather than a guarantee. My results suggest that the actual printable limit depends on the specific printer settings, geometry, and printing conditions used for the benchmark.

## Final CAD Design

The following image shows the updated CAD model. Compared with the first design, the holes are much more distinct and easier to identify. Changing the dimensions to millimeters also made it easier to control the hole diameters and create the 1 mm increments used for the test.

<img width="928" height="792" alt="Final CAD design" src="https://github.com/user-attachments/assets/2f609968-defe-406d-8c6a-bafadbf5598c" />

## Final Printed Artifact

The image below shows the final printed artifact. This print allowed me to see exactly where the Prusa Core One began to have difficulty reproducing the hole geometry. The larger holes remained open and recognizable, while the smaller holes became increasingly difficult for the printer to reproduce. The 4 mm hole was only barely successful, while the 3 mm hole did not form correctly.

## final thoughts on the design: 

Based on this benchmark, 4 mm represents the approximate lower limit for a reliably open hole under my selected printing conditions, while 3 mm was below the reliable printing threshold.

<img width="3024" height="4032" alt="Final printed artifact" src="https://github.com/user-attachments/assets/931744ff-6499-4db1-b914-b86dd89efa36" />

## 2nd Slicing 

When I created my second design, I used the same infill pattern and kept the infill at 15%. I chose to keep the infill the same because it had worked for the first print, and I wanted to focus on changing the hole diameters rather than changing multiple printing settings at once. This allowed me to make a more direct comparison between my first and second designs. 

<img width="996" height="438" alt="image" src="https://github.com/user-attachments/assets/8b858e30-cdf4-4d31-b889-360c0a038b0b" />

<img width="2556" height="1426" alt="image" src="https://github.com/user-attachments/assets/f7811253-dace-41ba-a72f-d9a306f7a7dc" />

## 2nd attempt Scale:

For my second design, I scaled the model down by 35% because the original design was a little larger than necessary. Scaling the design down allowed me to reduce the print time and get the benchmark completed more quickly. The estimated print time went from approximately 30 minutes to 13 minutes after reducing the scale by 35%. I kept the design at the same scaled size throughout the second print so the hole sizes could still be compared consistently within the model.

## Which Parameter did I use? (Preprocessor) 

For this project, I chose hole diameter as the parameter to characterize on the Prusa Core One. The objective was to determine the smallest hole diameter that the printer could reliably produce as an open, recognizable feature. Rather than testing a typical or recommended dimension, I designed the benchmark to approach the practical limit of the printer's capabilities. By using progressively smaller hole diameters, I could identify the point at which the printer could no longer accurately reproduce the geometry from the CAD model.

Based on the FDM Design Rules chart provided for the project, I predicted that the smallest hole diameter I could reliably print would be approximately 0.11 in, which is equivalent to approximately 2.794 mm. The chart listed 2 mm as the minimum recommended hole diameter, so I used this value as a reference when determining the dimensions for my benchmark. Since 0.11 in (2.794 mm) is larger than the 2 mm guideline, I expected the 0.11 in hole to remain open after printing.

I chose to test around this value because my goal was not simply to produce a hole that was comfortably within the recommended range. Instead, I wanted to approach the practical printing limit of the Prusa Core One and determine how closely the printer could reproduce small internal features. My expectation was that the larger holes would remain open while progressively smaller holes would eventually become closed or poorly defined. This would allow me to identify the approximate point at which decreasing the hole diameter caused the printer to lose the intended geometry. 



## Objective


## Analyze


## Decide


## Communicate

