# CNC Router
## Intro
In August of 2020, I watched [this](https://www.youtube.com/watch?v=_atw3e0nIrg&pp=sAQA) video. It looked like a very cool project and I was interested in the basics of CNC control and machining. The router is fundamentally and trim router mounted to 3 computer-controlled axes. I bought the plans to go into the building.   


## The Build
The router is made from aluminum tube and 3d printed parts. The aluminum was bought from a local welding supply and the parts were printed on my 3-D printer. The first part of the build consisted of printing all of the parts, I had one printer, an ender 3, and some of the parts took up to 3 days to print so it took a few weeks to get everything printed. 

![Pic](https://media.discordapp.net/attachments/871958447074197535/871958457245401148/unknown.png?width=800&height=674)

After everything was printed I used a miter saw to cut the Aluminum to length and used threaded rod to make a frame. 

![Pic](https://media.discordapp.net/attachments/871958447074197535/871959102115442728/unknown.png?width=800&height=674)

After the frame was constructed I drilled and tapped holes to attach the linear rails. These rails allow for very precise linear movements in one axis. 

![Pic](https://cdn.discordapp.com/attachments/871958447074197535/871959922441601054/b608572dd6d410a7f79df003b02318b5_2_1.png?width=800&height=674)

With the rails in place, I used moved onto the last part, electronics. The machine is driven by 4 stepper motors, these are similar to servo motors but they don't know where they are in space, they just move blindly. The rotational motion is converted to linear motion by a belt system for the X & Y axis and a leadscrew for the Z. These are controlled by an Arduino with a CNC shield running Pololu stepper drivers. The Arduino is sent Gcode (CNC language) from a PC running Universal G-Code Sender. The Arduino turns these high-level instructions into a signal for the motors and moves the router. On the computer side, this code is generated in Fusion 360 in a process called CAM. CAM turns a 3-D model into a series of toolpaths and eventually G-Code. The process for making a part is CAD(Make part on computer) -> CAM (Toolpath) -> GCode -> Machine -> Finished Part.

![Pic](https://media.discordapp.net/attachments/871958447074197535/871962533945294898/IMG_0244.jpg?width=800&height=674)

## Conclusion
This project was a behemoth. I got a part-time job in order to pay for it and it took half a year. That being said it was a fantastic experience. I learned so much about the CNC machining process and electronics as a whole. I got my first introduction into precision and how to make things line up the right the first time. I grew my skills with 3-D printing as well. I would like to take a moment to thank a number of people. For reference, this project was built soon after the drift trike, an insanely difficult project largely because I was on my own. Ivan (the designer of the machine) set up a discord server for fellow builders to help each other, this was invaluable. They answered everything from which version to build to what tap size do I need. Having completed the build I am now a regular contributor in order to give back. This project gave me invaluable insight into both engineering concepts as well as making me a more competent engineer while building my confidence. I made a [video](https://www.youtube.com/watch?v=HGkvg9hrSM4&pp=sAQA) discussing the project in more detail along with videos of cutting and results if you'd like to check it out! Thanks for reading.

![Pic](https://cdn.discordapp.com/attachments/871958447074197535/871962225433260032/unknown.png?width=800&height=674)
