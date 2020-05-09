# Head Mounted Displays (HMD)

It is my belief the traditional computer desktop (monitor, keyboard, mouse) has long overstayed its welcome. 

You have been mostly unkind to us humans, but you have served a meaningful purpose and we thank you for your invention - 
it is time to move on.

If you're looking for validation to these interfaces being unkind:
- Posture while using a traditional desktop environments is unkind.
- Sitting is unnatural, and sitting for long periods of time hurts the body/cardio system.
- Arthritis, tendon strain/cramp, carpel tunnel syndrome and many other problems with hands-on-keyboard and mouse.
- Static movement, you become immobile by relying on the traditional desktop environment.

I have heard many arguments about ensuring proper ergonomics. personally, I use a standing desk and a cushion under my feet to relax my knees and joints, and
i stand most of the day (until video game time i admit) - my response is basically always the same, you are saying there is a "configuration knob" on your 
desktop environment, and that's cool, I'm saying let's redesign it with the 3 principles I mention in mind first, design it FOR humanity first, instead of
as an afterthought. I don't think it is much of a slight to complain to the inventors of our current computer technology and demand it should have been invented
this way, it was just not in our timeline. So we must observe what exists, ask why and explore ways to design for the 3 principles: to help humanity feel: safe,
connected and empowered.  

It is my belief that our physical world is meant to be explored, and humans are meant to explore it. The reason we don't is the basis of my (3) principles,
humans sometimes don't feel: safe, connected or empowered to do so and it is my belief that real engineers build with these principles at the core of every
solution, no matter the business objective or purpose - building for humanity first is non-negotiable. be a better human.

Currently I'm not sure there is an ideal solution. HMD, which currently I will confess in my mind mostly refer to eyewear, are progressive, in that they are 
the next step for us to move passed the keyboard/mouse but in no way do they satisfy all requirements for an ideal technology. There are concessions that we
as humans must realize and accept. When we compare the usage of a modern computer monitor to a pair of eyeglasses, I prefer the latter. When we compare the use
of a keyboard/mouse to "natural interfaces" - the movement of the human body, the voice of a human, etc. these are natural ways we already communicate as humans,
I prefer natural interfaces. 

The naive approach here is to move the Graphical Window Manager you're familiar with (X11/Wayland on Linux, or whatever the f*ck Win/Mac call theirs) to the
optical waveguide designs that HMD's like magic leap's ml1 or microsoft's hololens use. And that is certainly an excellent first step, but the real ideas here
are founded in truly understanding how humans leverage technology and access information, post information-age. 

currently in 2020 i prefer the idea of the augmented (left) part of the immersivity spectrum, along with the ideas of spatial
computing, anchoring technology to our physical world. humans must feel safe/connected/empowered to explore our physical world, and augmenting reality allows 
this to happen. while the virtual (right) part of the immersivity spectrum is a form of escapism. 

---

## hardware

designing HMD/wearable platforms for the open source community. 

currently the hardware platform is based on a pair of glasses called "proto" that was available on thingiverse that i am modifying to house **omnivision ovm7690 cameracube's** and 3D print on my prusa mk3s in PLA. the idea is to modify the proto glasses model in fusion360 to make room for (5) cameracube's to start. then design FPC (flex printed circuit) to connect the cameracube's to a midplane that can either route to a jetson nano or over usb-c into a Snapdragon 840+ SoC smart phone.

starting with cameras allows those interested to build their own platform, modifying the mount hardware (glasses) and building ontop of a common framework together.

## my naive timeline to building an HMD platform is:
- mount (5) ovm7690 cameracube's onto proto glasses frames
- route cameras via custom FPC + hirose connector into a midplane
- translate signals into whatever dev platform requires
- process signals into images
- add 3D time of flight sensor to test depth mapping
- add IR emitter/photodiode to test surface detection/depth
- test optics engine
- LCOS microdisplay into a polarized beamsplitter (3 channels to start? 1 focal plane?)
- add rgb led light source
- add optics routing into entrance diffractions of optical waveguides (3 layers, RGB 1 planar of focus to start?)

