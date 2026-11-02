---
title: "Hepheastus v1"
author: "Sethu Manigandan Ramu"
description: "A laser engraver that will be simple to build for all."
created_at: "2026-10-26"
---
# October 26: The birth of Hepheastus

Today I decided to start my laser engraver project. I was down because I couldn't get my halflife project done in time for week 3, so decided to do this instead. I first brainstormed for a bit. After some time, I decided to choose between a laser engraver and a tool changing 3D printer. To create a fair comparison, I briefly decided to research both of the options. To begin with, I started with the tool changing 3D printer. After some time, I found the Stealth Changer, a Voron system for tool changes.

<img width="877" height="332" alt="image" src="https://github.com/user-attachments/assets/1a804d15-cdcc-48d8-a377-5249e878db1c" />

I really liked this and was planning to make a printer iinspired on this.

Then, I saw some laser engravers that could be used as reference. Many people have made laser engravers, but there isn't a universal "voron". After some brief research, I realized that blue diode lasers, the ones that'd fit in my budget, can't cut metal, as the light would reflect off of the metal

An example engraver

<img width="1024" height="683" alt="image" src="https://github.com/user-attachments/assets/96f0d450-51b1-4fc9-9c71-9e95b7f63692" />

Overall, I decided to go with a laser engraver due to its simiplicity.

**Total time spent: 0.5 hours**

# October 27: Research
  Today I decided to start the Hepheastus project. I started by researching. Laser GRBL, will be the firmware I'll be using. while on their sight, I saw many laser engravers and build guides for them. However, I wanted to make my own, and these will just be ideas. I found two main systems for laser engravers. A gantry system, in which the laser module physically moves around, as well as a Galvo system, where the laser is stagnant, and a mirror reflects the laser to different areas. I'm not trying to get a Ph.D in light and reflection, so I'll be building a gantry system.

Example of Gantry
<img width="241" height="241" alt="image" src="https://github.com/user-attachments/assets/2f0cc622-4996-4528-bc74-e7545c5eadea" />
Example of Galvo
<img width="651" height="471" alt="image" src="https://github.com/user-attachments/assets/39156e09-617e-49f9-9f15-beec9a3e76b8" />

Galvo systems do look interesting, so I might build one in the future for a different program... I'll be building a belt driven gantry as that's most popular.

  I also decided to research a laser module. I plan to use the laser tree 20w, 4 w optical power laser module. It's relatively cheap, and I found a bunch of cad models of it to use. This is one of the most used laser modules. It costs ~ $51

<img width="447" height="447" alt="image" src="https://github.com/user-attachments/assets/ecbd2db8-d1c2-41dd-a18b-87b407fb847b" />

  Now it's time to research motors. I realized that stepper motors are praised for this as they're able to stop in precise places with simple commands. I did a bit of research and the most popular motor is a NEMA 17. NEMA 17 is the name of the frame of the motor. It's 17x17 in width and height, but the lengths do vary from manufacture to manufacture. I'll be using a 48 mm long one (You can use any really, just with enough torque).

**Total time spent: 1 hour**

# October 28: The start of the frame

I've taken IED (Introduction to Engineering and Design) at my school, and we used Fusion 360. I kinda don't like Onshape, and find Fusion better, so I'll be using Fusion. I first had to download Fusion. My old computer only had 8 gb ram, so I couldn't use it. But now I can! Fusion install went smoothly. Now, it's time for cadding. This was an absolute PAIN to start. I first had to find models for 2020 extrusions, which I'll be using. Fusion allows you to immport any part
 from McMaster-Carr right in the application. However, the button was faded out. With a bit of research, I found out that you can only use McMaster-Carr parts in an assembly. So, I switched my mode to assembly. However, all McMaster-Carr CAD files only come with one lenth, which I didn't want. I planned to have my frame be 16 inches by 16 inches, but the cad only came in 12 inches. No problem; I'll just extrude the model. For some reason, extruding didn't work. With a bit of research, I switched to hybrid mode, with features of parts design and assembly. After extruding all my material, I realized this project wouldn't be as easy as I thought.

Photo of extruding not showing up on the modify tab:
<img width="1501" height="1048" alt="Screenshot 2026-10-27 165032" src="https://github.com/user-attachments/assets/db5ab883-4094-4246-895a-ba33582fb119" />

Photo of all of my extrusions.
<img width="1912" height="1048" alt="Screenshot 2026-10-27 173345" src="https://github.com/user-attachments/assets/c94978f6-4072-49f8-a0fa-7110d50be709" />

**Total time spent: 1 hour**

# October 30: The frame is complete!

I took a break for an incredibly hard calc test (got a 5!) and because I felt kinda down after realiziing something. To use open gussets for the corners, two pieces need to be 40 mm taller (so the other two will fit)).

<img width="938" height="705" alt="image" src="https://github.com/user-attachments/assets/16fdb1d2-b8b9-4058-b83a-daf316fa4599" />

Notice how to make a square, two of the pieces need to be shorter than the other, specifically by twice the width of the rectangles. Overall, this shouldn't matter at all and could be fixed with two quick extrusions, but that would give really weird lengths as the lengths are in inches and adding mm to it would give weird measurements. To fix this, I had to start over, make everything in round mm measurements. My laser frame is now 400mm x 400mm. I also imported in my open gussets for binding the extrusions to each other. Now I'm ready to start joints. For those who don't know, joints are how you connect things to each other in assemblies and hybrids in Fusion. There were a lot of issues, and it took like 8 tries to get the joints right. Sometiimes joints wouldn't connect. I realized that this was because some bodies weren't components. I simply had to make them components, and it fiinally worked. I was extremely relieved.

Example of a joint:
<img width="655" height="447" alt="Screenshot 2026-10-28 163142" src="https://github.com/user-attachments/assets/8849376b-ef38-4c49-a0ca-3fb42dd32274" />

Now unfortunately, I don't know what went wrong, but here was the side view of the frame:
<img width="720" height="311" alt="Screenshot 2026-10-28 173321" src="https://github.com/user-attachments/assets/bd5ba90f-0d3e-452c-b906-f66f51ca0a12" />

I got tired and called it a day.

**Total time spent: 1.75 hours**

# October 31: Fix Frame + Motor Frames

I decided to redo the joints due to the slanted extrusion. After redoing it, I decided to research a bit more on my gantry system. For now, I have chosen a 4 motor system for just one axis, and then two for the other. I derived this from this demo video thumbnail, which only uses two motors, but I added another two for speed.

<img width="515" height="388" alt="image" src="https://github.com/user-attachments/assets/8480151c-dba0-41b9-952f-3de2cf9c0d88" />

My version, in which I cadded my own motor mounting frames. This was difficult getting measurements right, but after a while, I realized sketches could be made on the motor and I just traced around the parts.

<img width="1917" height="1078" alt="Screenshot 2026-10-28 215849" src="https://github.com/user-attachments/assets/980ed243-e183-4c5a-a115-26de3813f639" />

**Total time spent: 2 hours**













  






