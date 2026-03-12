name: inverse
layout: true
class: center, middle, inverse
---

# Code as Material
### From Instruction to Expression

<br /><br />
### Prof. Dr. Lena Gieseke | l.gieseke@filmuniversitaet.de  

#### Film University Babelsberg KONRAD WOLF


???
Code as Material: 

Lecture and workshop invite students to consider computation not as a tool to master, but as a material to think and create with. What processes, aesthetics, and forms of authorship does code offer as a medium, and how does it shape contemporary artistic and design practice? In turn, how does artistic thinking shape code, and how can programming be positioned as a space for exploration, experimentation, and expression?




---
layout:false

## TODO: Teaser 1

???
  
Not the arts need technology but technology needs the arts.
  
  
Also: Just another step in human art making.

---

## TODO: Teaser 2

---

## TODO: Teaser 3

---
## Agenda

* Instructions - *Art as score*
* Algorithms - *Art as process*
* Computational Systems - *Art as interaction*
* Misuse - *Art as technological critique*


???
* The computer was invented to eliminate ambiguity and error. 
* Artists immediately turned it into a machine for producing ambiguity and aesthetic accidents.
* That tension between precision and misbehavior is what makes most interesting computational art.


---
template:inverse

# Instructions
## *Art as score*

???
* What is code at the most basic level?
* Describing an action

Many artworks are not objects.


```C++
#include <iostream>
using namespace std;

int main() {
    
    cout << "Hello World";
    return 0;
}
```

---
## Instructions

> Many artistic practices rely on **instructions that produce actions and outcomes**.

---
.header[Instructions]

.center[<img src="./img/score_01.png" alt="score_01" style="width:74%;">  
.imgref[[[Image: Wikipedia - From the opera William Ratcliff, by César Cui](https://simple.wikipedia.org/wiki/Sheet_music#/media/File:CuiVil3_2p204.png)]]]  


???
* Musical scores: instructions for producing sound
* ...does not contain music.  
* It contains **instructions for producing sound**.

---
.header[Instructions]

.center[<img src="./img/choregraphie_01.png" alt="choregraphie_01" style="width:70%;">  
.imgref[[[Image: The Public Domain Review - Dances in Beauchamp-Feuillet Notation (1701)](https://publicdomainreview.org/collection/dances-in-beauchamp-feuillet-notation/)]]]  



???
* Choreography: instructions for producing movement
* A choreography notation does not contain movement.  
* It contains **instructions for producing movement**.


First published in 1701, Choregraphie details an early dance notation system invented in the 1680s at the court of Louis XIV. Four years after the book was published, its author Raoul-Auger Feuillet, maître de danse to the King, found himself subject to a formal complaint by another maître de danse, Pierre Beauchamp, who argued that Feuillet had taken credit for an invention that was in fact his own. Surviving in modified forms into the 1780s, the system is now known as Beauchamp-Feuillet notation. Voltaire ranked the invention as one of the “achievements of his day” and Denis Diderot devoted ten pages to the subject in his Encylopédie. In 1706, the book was translated into English by John Weaver under the title Orchesography, or the Art of Dancing.


???

> Draw a line, pick a new color, move a bit...
  
<iframe src="https://editor.p5js.org/legie/full/-HB6nto44" width="540" height="540" ></iframe> 
<iframe src="https://editor.p5js.org/legie/full/WWsJj-V0D" width="540" height="540" ></iframe>

* https://editor.p5js.org/legie/sketches/WWsJj-V0D
 

---
.header[Instructions]

## Sol LeWitt - Wall Drawing #122, 1972

--

> ...all combinations of two lines crossing, placed at random, using arcs from corners and sides, straight, not straight and broken lines.
  
.footnote[[[Wikipedia - Sol LeWitt]](https://en.wikipedia.org/wiki/Sol_LeWitt)]

???
Wikipedia:  
Solomon "Sol" LeWitt (September 9, 1928 – April 8, 2007) was an American artist linked to various movements, including conceptual art and minimalism.
LeWitt came to fame in the late 1960s with his wall drawings and "structures" (a term he preferred to "sculptures") but was prolific in a wide range of media including drawing, printmaking, photography, painting, installation, and artist's books. He has been the subject of hundreds of solo exhibitions in museums and galleries around the world since 1965. The first biography of the artist, Sol LeWitt: A Life of Ideas, by Lary Bloom, was published by Wesleyan University Press in the spring of 2019.


---
.header[Instructions]

## Sol LeWitt - Wall Drawing #122, 1972

.center[<img src="./img/lewitt_01.jpeg" alt="lewitt_01" style="width:100%;">]


.footnote[[A. Adler. 2017. [*Sol LeWitt: 'Arcs and Lines' At Paula Cooper Gallery, NYC.*](https://www.huffpost.com/entry/sol-lewitt-arcs-and-lines_b_870641). Huffpost.]]


???

* In Wall Drawing #122, first installed in 1972 at the Massachusetts Institute of Technology in Cambridge, the work contains "all combinations of two lines crossing, placed at random, using arcs from corners and sides, straight, not straight and broken lines" resulting in 150 unique pairings that unfold on the gallery walls. LeWitt further expanded on this theme, creating variations such as Wall Drawing #260 at the Museum of Modern Art, New York, which systematically runs through all possible two-part combinations of arcs and lines.[23] Conceived in 1995, Wall Drawing #792: Black rectangles and squares underscores LeWitt's early interest in the intersections between art and architecture. Spanning the two floors of the Barbara Gladstone Gallery, Brussels, this work consists of varying combinations of black rectangles, creating an irregular grid-like pattern.[24]

---
.header[Instructions | Sol LeWitt - Wall Drawing #122, 1972]

.center[<img src="./img/lewitt_02.jpeg" alt="lewitt_02" style="width:30%;">]

.footnote[[A. Adler. 2017. [*Sol LeWitt: 'Arcs and Lines' At Paula Cooper Gallery, NYC.*](https://www.huffpost.com/entry/sol-lewitt-arcs-and-lines_b_870641). Huffpost.]]

---
.header[Instructions | Sol LeWitt - Wall Drawing #122, 1972]

.center[<img src="./img/lewitt_03.jpeg" alt="lewitt_03" style="width:70%;">]

.footnote[[A. Adler. 2017. [*Sol LeWitt: 'Arcs and Lines' At Paula Cooper Gallery, NYC.*](https://www.huffpost.com/entry/sol-lewitt-arcs-and-lines_b_870641). Huffpost.]]

---
.header[Instructions | Sol LeWitt - Wall Drawing #122, 1972]

.center[<img src="./img/lewitt_04.jpeg" alt="lewitt_04" style="width:70%;">]

.footnote[[A. Adler. 2017. [*Sol LeWitt: 'Arcs and Lines' At Paula Cooper Gallery, NYC.*](https://www.huffpost.com/entry/sol-lewitt-arcs-and-lines_b_870641). Huffpost.]]


---
.header[Instructions | *Funeral March for the Obsequies of a Deaf Man*, Alphonse Allais, 1897]

.center[<img src="./img/allais_01.jpeg" alt="allais_01" style="width:77%;"> .imgref[[Image: [Wikipedia -  Allais' Funeral March](https://en.wikipedia.org/wiki/4%E2%80%B233%E2%80%B3#/media/File:Marche_fun%C3%A8bre_compos%C3%A9e_pour_les_fun%C3%A9railles_d'un_grand_homme_sourd_-_Alphonse_Allais.jpeg)]]]

???
* Silent Compositions
* Designed Unpredictability
* Funeral March may have motivated John Cage's famous 4′33″
* https://en.wikipedia.org/wiki/4%E2%80%B233%E2%80%B3
    * 4′33″ is a modernist composition  by American experimental composer John Cage. It was composed in 1952 for any instrument or combination of instruments; the score instructs performers not to play their instruments throughout the three movements. It is divided into three movements,[c] lasting 30 seconds, 2 minutes and 23 seconds, and 1 minute and 40 seconds, respectively,[d] although Cage later stated that the movements' durations can be determined by the musician. As suggested by the title, the composition lasts 4 minutes and 33 seconds. It is marked by silence except for ambient sound, which is intended to contribute to the performance. 



---
.header[Instructions | *Score for December 1952 from Folio and 4 Systems*, Earle Brown, 1952]

.center[<img src="./img/brown_01.png" alt="brown_01" style="width:76%;"> .imgref[[Image: [getty.edu - Score for December 1952](https://www.getty.edu/publications/scores/object-index/301/#fig-301-a)]]]

???
* Indeterminate Music
* Score composed of floating rectangles and lines arranged without fixed order or instrumentation.
* Rather than prescribing exact pitches or rhythms, the score provides a visual field of elements that performers interpret freely, determining sequence, duration, and relationships in real time.
* It shifts composition from fixed notation to structured possibility, making performance an act of spatial and temporal decision-making rather than execution of a predefined script.

Aleatoric music often uses chance procedures in composition, sometimes fixed before performance. Brown’s score, by contrast, leaves key decisions to the performer in real time. The structure is open. The order, duration, and interpretation are not predetermined.

So it is aleatoric in spirit, but specifically a form of performer-driven indeterminacy. The composer defines a system of possibilities. The performer actualizes one path through it.





---
.header[Instructions]

## Yoko Ono - Grapefruit, 1964

.left-even[<img src="./img/ono_01.jpg" alt="ono_01" style="width:80%;">]

--
.right-even[
> ...an early example of conceptual art, containing a series of "event scores" that replace the physical work of art [...] with instructions that an individual may, or may not, wish to enact. 
 
]
.footnote[[Wikipedia. 2023. [*Grapefruit (book)*](https://en.wikipedia.org/wiki/Grapefruit_(book)), Kozy Feeling]]
  
---
.header[Instructions | Yoko Ono - Grapefruit, 1964]

## Painting To Be Constructed In Your Head

> Go on transforming a square canvas in your head until it becomes a circle. Pick out any shape in the process and pin up or place on the canvas an object, a smell, a sound or a colour that came to your mind in association with the shape. 
  
  
— 1962 Spring Sogetsu

  
.footnote[[Wikipedia. 2023. [*Grapefruit (book)*](https://en.wikipedia.org/wiki/Grapefruit_(book)).]]
  
---
.header[Instructions | Yoko Ono - Grapefruit, 1964]

## Cloud Piece

>Imagine the clouds dripping.
> Dig a hole in your garden to
> put them in.

  
— 1963 Spring

  
.footnote[[Wikipedia. 2023. [*Grapefruit (book)*](https://en.wikipedia.org/wiki/Grapefruit_(book)).]]
  
---
.header[Instructions | Yoko Ono - Grapefruit, 1964]

## Snow Piece

>Think that snow is falling. Think that snow is falling everywhere all the time. When you talk with a person, think that snow is falling between you and on the person. Stop conversing when you think the person is covered by snow. 

  
— 1963

  
.footnote[[Wikipedia. 2023. [*Grapefruit (book)*](https://en.wikipedia.org/wiki/Grapefruit_(book)).]]
  
???

## Tuna Sandwich Piece

>Imagine one thousand suns in the sky at the same time. Let them shine for one hour. Then, let them gradually melt into the sky. Make one tunafish sandwich and eat. 

  
— 1964 Spring

.footnote[[Wikipedia. 2023. [*Grapefruit (book)*](https://en.wikipedia.org/wiki/Grapefruit_(book)).]]
  



---
## Instructions

> Code is a way of writing **instructions that produce actions and outcomes**.

???
* At the most basic level, programming is not about machines.
* It is about **describing actions through precise instructions**.
* A line of code does not contain an image or sound.
* It is a **formal description of an action** executed by a machine.

Creative Coding Exercises:
* Circles!
* Happiness
* A single instruction produces a single action.
* But when instructions **repeat and interact**, something new appears.

The medium matters.


--

<br />

Computation as medium (*automation*)

* Repeat processes
* Condition behavior
* Respond to inputs

--

> Scale beyond human execution
--

> and re-distribution of authorship.


---
## Instructions

A single instruction produces a single action.

--

<br />

When computational instructions **repeat according to rules**,  
they become **processes**.

--

<br />

> These rule-based processes are called **algorithms**.


---
template:inverse

# Algorithms

---


* Algorithms (What happens when instructions are combined and repeated?) (Describing a process)
    * Rules + iteration
    * Fractals
    * Generative art (defined by the process rather than the final image)
    * Emergence (complex patterns from simple rules — here code already begins to behave like material)
    * Workshop example

---
template:inverse

# Computational Systems

---

* Computational Systems (What happens if we build pipelines, add hardware, and let things interact — analog and digital?)
    * Feedback
    * Interaction
    * Experience
    * Embodiment

---
template:inverse

# Misuse

---

* Misuse (What happens if we go against the intended use?)
    * Example: Generative AI
    * Misuse and pushing limits
    * Revealing hidden assumptions in technology

---
template:inverse

# Summary

---

* Summary and Outlook
    * Not technology challenging artists
    * Artists challenging technology








---
template:inverse 

.center[
<img src="./img/qr_lecturecodeasmaterial.png" style="width:20%;">
]


# *The End*


### Prof. Dr. Lena Gieseke | l.gieseke@filmuniversitaet.de  

#### Film University Babelsberg KONRAD WOLF

