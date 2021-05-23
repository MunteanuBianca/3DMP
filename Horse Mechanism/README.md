# Final Project - Horse Automata

## This is a readme.md for the final project of the 3D Modeling and Printing course
I chose the Horse Automata project because it looks elegant and appropriate for my skills in 3D modelling. 
I can learn a great deal about mechanisms and linkages from recreating this model.
The mechanism is design using Autodesk Fusion 360.

## Repository contents
I added in the repository the f3d file of the final version of the Horse Mechanism, the stl files for each component, even though some ar identical, all the canvases used in the design and the renders of the mechanism.

## Resources
The initial design was created by Greg Zumwalt and can be found 
on his [youtube accont](https://www.youtube.com/watch?v=dtO8aX2QzzY).
Furthermore, he uploaded stl files with all the components and instructions for the assembly, which have been usefull in understanding and recreating the mechanism. the files and instructions can be found on various sites such as [Instructables](https://www.youtube.com/redirect?event=video_description&redir_token=QUFFLUhqblBlS0NLc04tVERLbnpKdlB5X2xOSXBVZDROZ3xBQ3Jtc0trcXRiVG5DR1c4ai1WeDJ4M2g1QVpHY1dfUzZzdnJ6dFpTTHl3elRUellzeXNLV0RwSVlKcm5KdFRKR3lVNkE0a01OR19oTlNHX2VWZUthQ2NkZ1BXYjBGcVRZYjc2d2Qtd0tXektYeHQ0bHhsa1BXNA&q=https%3A%2F%2Fwww.instructables.com%2Fid%2FHorse-Prototype%2F)and [YouMagazine](https://www.youtube.com/redirect?event=video_description&redir_token=QUFFLUhqbDZYWENka0hKSHJlbzdmbllOd3RaWlJ3MGx3QXxBQ3Jtc0tuY1o3cWtXbmk4aWU1Q1I0S0p4YzMzNlBCbkpid1BzUUpRNDZlczA5RGVLZ2hTT2hwRC1OSXNDckNLT0I3WU45b0ZjQUJBUGw0QWVjdmpXR3RJRWxPRmFZRzRNYVVpRk1vUHJMYkdNNll1eGNtejRWVQ&q=https%3A%2F%2Fwww.youmagine.com%2Fgzumwalt%2Fdesigns)

## Horse Automata Components
The main components in this project are the Body, Head, Tail, Legs and Holder.
With the exception of the Head and Tail, every component has multiple subcomponents inside it. 

### 1.Holder

This is the first component that i started with. Inside it there are the base, housing motor, gear, motor and phono plug. 
The base is the horizontal part that is grounded and sustians the whole construction. 
It has a hole in the middle where the housing motor will be placed. The inside of the body is empty to reduce the usage of plastic.
The housing motor is the vertical part of the holder in wich the motor and gear will be placed.
The body will be fixed on the upper part of the housing motor using screws and the other components will fixed on the body. 
The gear is linked to the motor wich makes it rotate and eventually, creates the entire motion of the horse.
The motor is a design imported from grabcad and can be found on [gearbox](https://grabcad.com/library/nema-34-86mm-with-planetary-gearbox-1).
The phono plug is also imported from grabcad and can be found on [plug](https://grabcad.com/library/3501fr)
Inside this components there is also a subcomponent called screws in witch I put the 4 screws that conect the holder with the body.

### 2.Body
This component is the most complex one (so far). I followed the instructions for the assembly to know in wich order to creat every component.
For the shape of the body I used a canvas created by downloading the stl file of the [Body Right](https://content.instructables.com/ORIG/F3P/SE05/JG42UTH6/F3PSE05JG42UTH6.stl) and cropping the exact immage that I needed using the snipping tool. 
First I created the Right Body. I scketched the shape from the canvas and then extruded it.
Then I created The body spacers which could have also been imported from the McMaster-Car Catalog but I realised that only after I created them.
They are ment to be supports for objects that need to be fixed to the body but also rotate (tail, head and 2 gears)
The body spaceres are fixed to both the front and back body with screws.
For the Idler gears I went back and foth with the dimensions and at the same time changing the dimensions of the holder gear in ored to make them fit together.
The next step was adding the cams. There are 2 on the right side and have different dimension and they are mirrored on the left side,
but rotated at 180 degres. They will link the legs motion with the motion from the body gears (that is linked with the rotation of the holder gear).
At this point, I started adding the joints and motion links to make sure that everything is working fine.
I created the tail and the head around their body spaceres and then I added the back body and fixed it with screws.

### 3.Legs
I created the legs on the right side and then mirrored them on the left using copy-paste new for every component. I used canvases in order to see the right dimensions and position of each part. All four legs are created by first positioning the canvases, creating the sketchs and extruding. The rigid groups and joints are added between components and screws, not between two components. The screw conencts two components, but one component is fixed on the screw, while the other rotates around it, due to its shape (I used shoulder screws). When assambled correctly, the legs move without problem without the need of joint limits.

### 4.Tail
For the tail I sketched around the canvas and extruded. It rotates around a body spacer that is fixed on the right and left body with 2 screws.

### 5.Head
I created a sketch using a canvas and extruded. The motion and link to the body is identical to the tail motion.

## Horse Automata Motion

The motion of this design is a fascinating one because looking at the finished result we see all 4 legs moving but in different ways and 
also a small movment in the head and tail.
All the motion is generated by one single rotation of the holder gear that is powered by a motor.
the holder gear rotates the idler gears. the idler gears then rotate the gears.
The cams are linked with the gears so when the gears move, the cams move.
The cams produce the legs' movement and then the legs push the head, respectively the tail.
To see this movement in Fusion I only need to make a motion study for the holder gear rotation.
I added the tail rotation and head rotation in the motion study to avoid using contact sets.


