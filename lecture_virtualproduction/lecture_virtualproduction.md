name: inverse
layout: true
class: center, middle, inverse
---


## Introduction to Virtual Production Techniques

<br />
### Prof. Dr. Lena Gieseke | l.gieseke@filmuniversitaet.de  

#### Film University Babelsberg KONRAD WOLF


???

This talk offers an introduction to virtual production and its toolset. It outlines how real-time engines, LED volumes, performance capture and in-camera visual effects reshape the relationship between physical sets and digital environments. Through practical examples, the talk considers the creative and organisational implications of virtual production, showing how these techniques influence aesthetic and narrative decisions in contemporary filmmaking.

---
layout:false

.center[<img src="./img/vp_shot_01.png" alt="vp_shot_01" style="width:100%;">].imgref[[Image: Der Turm - Filmuniversität]]

---

.center[<img src="./img/vp_shot_02.jpg" alt="vp_shot_02" style="width:100%;">].imgref[[Image: Interconnections - Filmuniversität]]

---

.center[
 <video width="1024" controls>
  <source src="./img/mandalorian_cutout_01.mp4" type="video/webm">
</video>  
]

.footnote[[[YouTube - The Virtual Production of The Mandalorian Season One](https://www.youtube.com/watch?v=gUnxzVOs3rk), Industrial Light & Magic]]

---

.center[<img src="./img/mandalorian_01.png" alt="mandalorian_01" style="width:100%;">]

.footnote[[[YouTube - The Virtual Production of The Mandalorian Season One](https://www.youtube.com/watch?v=gUnxzVOs3rk), Industrial Light & Magic]]


---

.center[<img src="./img/halostage_01.jpg" alt="halostage_01" style="width:100%;">].imgref[[Image: Adrian Weber & Halostage]]

---

.center[<img src="./img/mandalorian_02.png" alt="mandalorian_02" style="width:100%;">]

.footnote[[[YouTube - The Virtual Production of The Mandalorian Season One](https://www.youtube.com/watch?v=gUnxzVOs3rk), Industrial Light & Magic]]



---
## Who am I?

* Master in Fine Art (MFA Dramatic Media)
* 6 years in the industry (VFX, R&D, Software Development)
* Phd in Computer Science (Dr. rer. nat. Computer Graphic)

--

<br />

* Film University Babelsberg KONRAD WOLF, Potsdam, Germany
* Professor for Image-based Media Technologies
* MA Creative Technologies

> Computer Science meets Creativity, Art & Film...


---
.header[MA Creative Technologies]

.center[<img src="./img/qr_filmunictech.png" alt="qr_filmunictech" style="width:45%;">]

---
.header[MA Creative Technologies]

.center[<img src="./img/qr_filmuniinsta.png" alt="qr_filmuniinsta" style="width:45%;">]


---
## Film University Babelsberg KONRAD WOLF

--

* Largest film school in Germany (established 1954), now public university

--

* About 100 in-house film productions yearly

--

* State-of-the-art equipment and environments (2 studios, 150 and 300 sqm)

???
* e.g., Sony F55, ARRI Alexa, Panasonic VariCam, Harrison MPC4D console with Dolby Atmos
* ceiling lighting rigs

---
## Film University Babelsberg KONRAD WOLF

.left-quarter[
Neighbor: Babelsberg Film Studio, oldest large-scale film studio in the world, producing films since 1912.
]
.right-quarter[<img src="./img/studio_01.jpg" alt="studio_01" style="width:78%;"> .imgref[[Image: [Studio Babelsberg](https://www.metropolitanbacklot.com/galerie/)]]]


???
* Hundreds of films, including Fritz Lang's Metropolis and Josef von Sternberg's The Blue Angel were filmed there. More recent productions include V for Vendetta, Captain America: Civil War, Æon Flux, The Bourne Ultimatum, Valkyrie, Inglourious Basterds, Cloud Atlas, The Grand Budapest Hotel, The Hunger Games, Isle of Dogs and The Matrix Resurrections. 

---
template:inverse

# Introduction to Virtual Production Techniques


---
## Agenda

--

* Basics
    * Film Production Steps
    * Visual Effects

--

* Virtual Production
    * Real-time Engines
    * LED Walls

--
* Implications

???

The tools of virtual production: Realtime Engines, LED Walls, Hybrid Green Screens


---
template:inverse

# Basics

???
Let's assume we are talking about movie making that includes computer generated imagery (CGI)

---

.center[<img src="./img/vfx_01.jpg" alt="vfx_01" style="width:100%;">].imgref[[Image: *Avatar: The Way of Water*, Disney via [Backstage](https://www.backstage.com/magazine/article/create-digital-effects-film-project-13748/)]]

---

.center[<img src="./img/vfx_02.jpg" alt="vfx_02" style="width:100%;">].imgref[[Image: *House of the Dragon* Credit: Ollie Upton/HBO via [Backstage](https://www.backstage.com/magazine/article/create-digital-effects-film-project-13748/)]]

---

.center[<img src="./img/vfx_03.png" alt="vfx_03" style="width:100%;">].imgref[[Image: *1899 Virtual Production*, [Framestore](https://www.framestore.com/work/1899-virtual-production)]]


---
.header[Basics]

## Visual Effects

--

.left-even[
* VFX

]


.right-even[<img src="./img/vfx_04.jpg" alt="vfx_04" style="width:100%;"> .imgref[[Image: studiobinder](https://www.studiobinder.com/blog/what-is-vfx/)]]

---
.header[Basics]

## Visual Effects


.left-even[
* VFX
* Computer-generated imagery (CGI) or manipulated images integrated into live-action footage

]


.right-even[<img src="./img/vfx_04.jpg" alt="vfx_04" style="width:100%;"> .imgref[[Image: studiobinder](https://www.studiobinder.com/blog/what-is-vfx/)]]

---
.header[Basics]

## Visual Effects

.left-even[
* VFX
* Computer-generated imagery (CGI) or manipulated images integrated into live-action footage
* **Post-Production** step
]


.right-even[<img src="./img/vfx_04.jpg" alt="vfx_04" style="width:100%;"> .imgref[[Image: studiobinder](https://www.studiobinder.com/blog/what-is-vfx/)]]





---
.header[Basics]

## Visual Effects

.center[<img src="./img/cgi_03a.png" alt="cgi_03a" style="width:80%;">].imgref[[Image: Adrian Weber & Halostage]]

???

Live action plus CG elements.
* Gravity  
* The Mandalorian


Full CG productions.
Mocap with live preview.
* The Lion King  
* The Jungle Book  
* Ready Player One

Live action and CG characters.
Live preview of characters.
* Real Steel  
* Hulk (MCU)



---
.header[Basics | Visual Effects]

## 2D Compositing

.center[<img src="./img/layers_01.jpg" alt="cgi_03a" style="width:55%;">].imgref[[Image: [freepik](https://www.freepik.com/free-vector/parallax-background-2d-landscape-with-fantasy-tree_21133686.htm#fromView=keyword&page=1&position=0&uuid=ded0997d-7f07-48a2-aca5-d62e5071c9b6&query=Cgi+animation+portfolio)]]



---
.header[Basics | Visual Effects]

## On Set Green Screen Shooting

.center[<img src="./img/vfx_05.png" alt="vfx_05" style="width:36%;">  <img src="./img/vfx_06.png" alt="vfx_06" style="width:36%;">.imgref[[Images: [digitalsynopsis](https://digitalsynopsis.com/design/movies-before-after-green-screen-cgi/)]]]





---
.header[Basics | Visual Effects]

## VFX Film Production Pipeline

.center[<img src="./img/pipeline_01.png" alt="pipeline_01" style="width:100%;">].imgref[[Image: [Unreal Engine - Virtual Production](https://www.unrealengine.com/en-US/explainers/virtual-production/what-is-virtual-production)]]







---

## The VP “Toolset”

Preproduction  
Previs / Stuntvis / Techvis / …

Production  
Mocap / Facial Capture / Volucap / Greenscreen Preview / …

Postproduction  
Postvis / VFX-Vis / …

![](Picture11.jpg)
![](Picture13.jpg)
![](ContentPlaceholder9.jpg)
![](Grafik6.jpg)
![](Grafik7.jpg)

???
These three production types of virtual production use various technologies and methods for different project stages.

The goal is reliable visualization and fast interaction with CG content throughout all stages of production.

Stage 1: Previs, Stuntvis, Techvis  
Stage 2: Mocap, Facial Capture, Volumetric Capture  
Stage 3: Postvis, VFX-Vis  

---

## ICVFX (LED Virtual Production)

![](Picture5.jpg)

???
In-Camera VFX production test.
Reference: Unreal Engine documentation.

---

## Greenscreen Virtual Production

![](Picture5.jpg)

???
Example: The Adam Project behind-the-scenes blooper reel.

---

## Terminology: LED, Realtime Engines, ICVFX

???
Short overview of the studio and LED technology.

---

![](Inhaltsplatzhalter5.jpg)
![](Grafik7.jpg)

???
The volume is built from cabinets.
Cabinets consist of modules.
Modules contain LEDs.

LED properties:
Pixel pitch  
Brightness  
Refresh rate  
Multiplexing  

---

![](Grafik7.jpg)
![](Grafik1.jpg)
![](Grafik4.jpg)
![](Grafik5.jpg)
![](Grafik6.jpg)

???
Realtime engines in 3D:
Unreal Engine, Unity.

Realtime engines in 2D:
Pixera, Vertex.

What works well for what?
FX, nature, and more.

---

![](Picture5.jpg)

???
Brainbar setup:
Unreal Engine, Pixera, controller.

Head of department: Technical Director.

Signal path:
Control via master system.
Rendering on offsite render nodes.
Transfer via LED processor over fiber.
Through extender to the wall.

Tracking:
Processed on tracking PC.
Sent to all Unreal engines.
Then output to the wall.

---

![](Inhaltsplatzhalter6.jpg)

???
Overview of Unreal Engine signaling.

---

## 2D vs. 3D vs. 2.5D

???
Short coverage of the possibilities and roles on set and during preparation.
Differences depend on studio, country, and budget.

---

![](Grafik5.jpg)

# 3D

???
Full 3D environments rendered in realtime.

---

![](Grafik5.jpg)
![](Inhaltsplatzhalter5.jpg)

# 2D

???
Flat backgrounds.
Limited parallax.
Often performance efficient.

---

![](Inhaltsplatzhalter5.jpg)

# 2.5D

???
Combination of layered 2D and selective 3D elements.

---

## Short Break

???
Coffee time and snacks.

---

## General Advantages and Possibilities

---

![](Grafik4.jpg)

???
In-Camera VFX production test.
Reference: Unreal documentation.

Result on set:
Immediate in-camera results.

Gigantic sets:
Large environments without physical restrictions.

Impossible sets:
Floating elements, flight, extreme architecture.

Any set:
Almost everything can be digitally recreated.

---

![](Grafik4.jpg)

???
Time stop:
Shoot any location at any time of day.

Flexibility:
Change time of day during the shoot.
Modify objects live.

Plannability:
Costs are fixed in advance.
No weather days.
No night shooting required.

Comfort:
Studio shooting is often more comfortable than location shoots.

Budget:
Often cheaper than on-location production.

---

![](Grafik4.jpg)

???
Driving shots:
Instant reset.

Flight shots:
Any camera movement possible.

Game logic:
Movements can be transferred.

---

![](Grafik4.jpg)

???
Multi-camera:
Possible to a certain degree.
More natural setups.

On location feeling:
Shoot directly in the digital location.

CO2 reduction:
Disney estimated about 30 tons CO2 saved per avoided flight.
Netflix reported 1.1 million tons CO2 in 2021.
About half came from physical production.

Shifting 10 to 20 locations into LED studio
could save 300 to 600 tons CO2 per title.
Reduction up to 30 percent.

---

## Drawbacks and Limitations

---

![](Grafik4.jpg)

???
Unwanted effects:
Scanlines, color shifts, banding, moiré.

Limitations:
SFX like fire, smoke, water, dust only limited.

Latency:
Sudden movements on set are challenging.

---

![](Grafik4.jpg)

???
Less freedom:
Large setups must be optimized for performance.
Sometimes only 2D possible.

Fixed framerate:
24 FPS.
No switching mid-day.

High-speed:
Difficult due to sync standards and performance constraints.

If it is down, it is down:
If a wall fails, production stops.
Hard to quickly switch alternatives.

---

![](Grafik4.jpg)

???
The new process:
Everything is more interconnected.
Requires more planning and more preparation time.

New roles:
Many new job profiles.
They must first be established.

New set conditions:
New aspects must be considered on set.
Often not enough time allocated.

Set your expectations:
The clearer decisions are made before the shoot,
the more targeted and cost-efficient the production becomes.

---

## Questions and Answers

---

## THANK YOU – SEE YOU LATER!

![](Grafik3.jpg)

Adrian Weber  
adrian.weber@halostage.studio  

www.halostage.studio  
www.ict.de  

Copyright by ICT AG / HALOSTAGE