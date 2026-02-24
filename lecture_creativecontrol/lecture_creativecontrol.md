name: inverse
layout: true
class: center, middle, inverse
---


### How, What, Where, When, Who
## Mechanisms for Creative Control

<br />
### Prof. Dr. Lena Gieseke | l.gieseke@filmuniversitaet.de  

#### Film University Babelsberg KONRAD WOLF


???

**Storyline:** CS publications routinely claim their systems are "artist-friendly" or "creatively usable" and validate those claims with small user studies. User studies, when executed properly, are a legitimate form of validation — but they are not the only one, and on their own they leave the underlying question underspecified: what does creative usability actually consist of? The field has made previous attempts to answer this. We examine those attempts, identify what they leave open, and propose that creative control is a configuration space of five interacting dimensions: How, What, Where, When, and Who. The aesthetic qualities that emerge from any creative system — algorithmic or analog — are shaped by how those dimensions are configured and how they interact. These dimensions also give researchers and practitioners a shared vocabulary for asking more precise questions about what a system actually affords.

**Take-home:** "Creative control" is not a diffuse property but something that can be precisely described, designed for, and evaluated.


1. Opening — Five Questions
2. The Problem of Defining Creative Usability
3. Existing Frameworks — And What They Leave Open
4. HOW — The Modality of Input
5. WHAT — The Content and Level of Abstraction
6. WHERE — The Spatial Scope of Control
7. WHEN — The Temporal Position of Control
8. WHO — Agency, Authorship, and the Co-Agency Spectrum
9. Five Dimensions, One Design Space
10. Closing — Authorship is a Configuration




---
layout:false

.center[<img src="./img/watercolor_01.jpg" alt="watercolor_01" style="width:84%;">].imgref[[Image: [pexels, Fahad Puthawala](https://www.pexels.com/photo/close-up-of-hand-painting-a-watercolor-landscape-29559075/)]]


???
ASK: 
* How is input given? 
* What does the artist provide? 
* Where does it act? 
* When in the process? 
* And who is in control? 

No answers yet — only the questions. These are not questions about medium. They are questions about the structure of any creative act.

---

.center[<img src="./img/touchdesigner_01.gif" alt="touchdesigner_01" style="width:100%;">].imgref[[Image: [interactiveimmersive.io: Scaling Interactive Notch Content in TouchDesigner](https://interactiveimmersive.io/blog/touchdesigner-resources/scaling-interactive-notch-content-in-touchdesigner/)]]


???
ASK: 
* How is input given? 
* What does the artist provide? 
* Where does it act? 
* When in the process? 
* And who is in control? 

No answers yet — only the questions. These are not questions about medium. They are questions about the structure of any creative act.



---

.center[<img src="./img/keyboard_01.jpg" alt="keyboard_01" style="width:74%;">].imgref[[Image: [Filmuniversität](https://www.filmuniversitaet.de/studium/studienangebot/masterstudiengaenge/creative-technologies/projekte/making-waves)]]


???
ASK: 
* How is input given? 
* What does the artist provide? 
* Where does it act? 
* When in the process? 
* And who is in control? 


The point: the questions still map. What changes is not the structure of creative control but its implementation. This talk investigates what happens to each dimension when the medium becomes computational — and what that means for authorship and expression.

---
## Agenda

* The Problem of Defining Creative Usability
* Existing Frameworks
    * How
    * What
    * Where
    * When
    * Who
* Five Dimensions, One Design Space
* Authorship as Configuration



---
template:inverse

# Defining Creative Control

---
## Defining Creative Control

--

> ...artist-usable!  
> ...creatively controllable!


---
.header[Defining Creative Control]

## "Artist-Friendly" Isn't Good Enough


We should strive for a realistic discussion and towards defining such terms more systematically.

???
  

* Little attention, however, has been paid to overall creative workflows, which need to strike a balance, giving users needed power without burdening them with unwanted details. Often, techniques that are claimed to be artist-controllable turn out not to be so.

* Why are we doing what we are doing?

--

One approach: 

* review relevant characteristics of underlying algorithms,

--

* motivated by an artist’s perspective.



???

* We include interface design aspects but they are not the focus of this survey


CS and HCI publications routinely claim their systems are "artist-friendly" or "creatively usable" — and validate those claims with user studies. When executed properly, user studies are a legitimate form of validation. But they leave the underlying question underspecified: what does creative usability actually consist of? What are we measuring when we say a system supports creativity?

The problem is not a lack of seriousness. It is a definitional one. Creativity is:
- Ill-defined as a construct, and
- A topic that draws insights from psychology, cognitive science, philosophy, and HCI simultaneously — making it notoriously difficult to operationalize.

Source: Frich et al. (2018, 2019), Remy et al. (2020) — a sequence of meta-studies calling for more rigorous evaluation and clearer definitions of creativity in HCI research.

---
template:inverse

# Defining Creative Control


---
.header[Defining Creative Control]

## Creativity


Creativity is

* ill-defined, and
* involves insights from various disciplines,
 
making is notoriously difficult topic to address.

<br />

> How can creative control be defined?

---
.header[Defining Creative Control]

## HCI

--

.caps[Shneiderman, Ben]. **Creativity Support Tools: Accelerating Discovery and Innovation**. *Communications of the ACM* 50.12 (2007), 20–32

--

* .caps[Frich, Jonas, Mose Biskjaer, Michael, and Dalsgaard, Peter]. **Twenty Years of Creativity Research in Human- Computer Interaction: Current State and Future Directions**. Proceedings of the 2018 Designing Interactive Systems Conference. ACM, 2018, 1235–1257
* .caps[Frich, Jonas, Macdonald Vermeulen, Lindsay, Remy, Christian, et al.] **Mapping the Landscape of Creativity Support Tools in HCI**. Proceedings of the 2019 CHI Conference on Human Factors in Computing Systems. ACM, 2019, 1–1
* .caps[Remy, Christian, Macdonald Vermeulen, Lindsay, Frich, Jonas, et al.] **Evaluating Creativity Support Tools in HCI Research**. Proceedings of the 2020 ACM Designing Interactive Systems Conference. ACM, 2020, 457–47

--

>  ...asking for more rigorous evaluation in regard to claimed creativity support.  
> ...clearer definitions of creativity.



???
The field of Creativity Support Tools (CSTs) has been central to HCI since Shneiderman's foundational 2007 paper. The ambition: design tools that accelerate discovery and lower the threshold for creative production. The challenge: CST research has historically conflated two distinct questions — whether a tool enables creative outcomes, and whether the tool itself is the source of creative agency.

Source: Shneiderman (2007). Visual: timeline of CST research from 2000–2020 showing volume of publications and the growing methodological critique.

Frich et al. (2018) surveyed twenty years of creativity research in HCI and identified a persistent gap: most studies assess whether users feel creative, not whether the system's architecture enables or constrains creative control. Remy et al. (2020) sharpen this: evaluation methods for CSTs remain inconsistent, and user-perceived creativity does not reliably track with the structural affordances of the system being studied.

The implication: we need evaluation on an algorithmic level — a vocabulary that describes what a system structurally affords, as a subset of (not a replacement for) user-study-based assessment.



---
.header[Defining Creative Control]

## Creativity Support Index (CSI)

.caps[Cherry, Erin and Latulipe, Celine]. **Quantifying the Creativity Support of Digital Tools Through the Creativity Support Index**. *ACM Transactions on Computer-Human Interaction* 21.4 (2014), 21:1– 21:25 

--

* Measures how well a tool enables creativity based on a psychometric survey
* *Exploration*, *expressiveness*, *immersion*, *enjoyment*, *results worth effort*, *collaboration*
  
  
--
  
We are looking for

* an evaluation on an algorithmic level,
* as a subset of a more general and user-study-based classification.


???
The most widely used instrument for evaluating creativity support is the Creativity Support Index (CSI), developed by Cherry and Latulipe (2014). CSI is a psychometric survey instrument that measures how well a tool enables creativity across six dimensions: exploration, expressiveness, immersion, enjoyment, results worth effort, and collaboration.

CSI is rigorous within its own register — it provides quantifiable, comparable scores across tools. But it operates entirely at the user-experience level. It tells us how users feel about the system. It does not describe the system's internal architecture or explain why those feelings arise. As a diagnostic tool for system design, it is post-hoc: it can tell you that your system scored low on exploration, but not where in the architecture the problem lives.

Source: Cherry and Latulipe (2014).



---
.header[Defining Creative Control]

## Discussion Basis

.caps[Weisberg, Robert]. **Creativity: Understanding Innovation in Problem Solving, Science, Invention, and the Arts**. *Wiley*, 2006  

.caps[Boden, Margaret A.]. **Creativity and Art: Three Roads to Surprise**. Oxford University Press, 2010  

--

A creative process

> ...intentionally produces a novel product.  

--

Novelty 

> ...as a surprising product, one that the creator did not directly anticipate.



---
.header[Defining Creative Control]

## Discussion Basis

Gieseke et al. (2021).

<!-- * The general controllability necessary for navigating a design space

> There are many different roads in the landscape.
 
* Transparency of that navigation and the understanding of cause and effect when using the tool

> I have the map to the landscape and know how to get from one point to another. -->

* Navigation
* Transparency
* Variation
* Stimulation


???
This framework is significantly more structural than CSI. It gives researchers and practitioners a vocabulary for system-level analysis rather than user-feeling assessment.

Source: Gieseke et al. (2021). Visual: a 2x2 grid or taxonomy diagram of the four dimensions and their sub-components.


---
.header[Defining Creative Control]

## Navigation

Navigation describes both whether a creation processes is efficiently manageable and the extent of the controllability.

* Interactive
* Number of Controls
* Navigation History


???
Navigation describes both whether a creation processes is efficiently manageable and the extent of the controllability.

* Interactive: Refers to the lack of noticeable delays when executing controls and computing results. Lengthy, non-creative configuration requirements are potentially distracting. Hence, a thorough analysis should consider the whole process an artist has to go through to produce a result.
* Number of Controls: Indicates how flexible and controllable a technique is by counting the number of different controls that can be adjusted for one output. Ideally, this category would refer to the ratio in the possible output of visual features that are relevant to humans to controllable features. This would ensure that the controls cover all necessary features and that they complement each other. However, the identification of generally describable, perceptually relevant visual features is out of the scope of this survey and left to future work.
* Navigation History: Describes the ability to go back and forth in one’s own creation process, such as using an eraser.


---
.header[Defining Creative Control]

## Transparency

Transparency describes how clear the understanding of cause and effect within the system is.

* Control Domain
* Control Communication
* Control Consistency

???
* **Transparency** — clarity of cause-and-effect within the system. Sub-dimensions: control domain (what does a control affect?), control communication (how legibly is that effect conveyed?).

* Control Domain: Refers to how well controls are mapped to visual features and how well they cover the possible design range of each feature. A high-quality control should not have any overlapping effects with other controls.
* Control Communication: Describes how well controls (e.g., with a visualization and/or little abstraction) represent their effects on the result. For artist-centered tools this could mean that controls should be visual and directly on the canvas.


---
.header[Defining Creative Control]

## Variation

Variation indicates how visually different the results can be.

* Size of the Design Space
* Openness of the Design Space

???
* **Variation** — how visually different the achievable results can be. Sub-dimensions: size of the design space, openness of the design space.

* Size of the Design Space: This is limited if all results look rather similar to each other and are part of a specific design class. A large design space of one technique allows, for example, combining different texture classes such as stochastic and structural creation.
* Openness of the Design Space: Refers to the limitlessness of possible designs and that there is no attachment of the technique to a specific design class. An open design space enables an artist to come up with a distinctive individual style. Different artists can create inherently different and unique results with the same tool if it has a open design space.
  
We do understand that a clear definition of the available different design classes is needed. However, these depend solely on the design task.


---
.header[Defining Creative Control]

## Stimulation

The means of stimulation indicate how well an artist can enter a pleasurable and stimulating workflow.

* Immersion
* Stimuli

???
* **Stimulation** — how well a system supports pleasurable, immersive creative workflow. Sub-dimensions: immersion, stimuli.

* Immersion: How natural and enjoyable the usage of a system feels. An immersive technique needs navigation to be fluent, controls to be intuitive, and the design space large enough to not to hit its boundaries while using the tool.
* Stimuli: The support for finding surprising results—for example, with design suggestions or variations of the input. Options to support stimulation are still underrepresented but on the rise with machine learning techniques. A clear definition of this category is not feasible at this point.


---
.header[Defining Creative Control]

## Discussion Basis

<!-- * The general controllability necessary for navigating a design space

> There are many different roads in the landscape.
 
* Transparency of that navigation and the understanding of cause and effect when using the tool

> I have the map to the landscape and know how to get from one point to another. -->

* Navigation
    * Interactive
    * Number of Controls
    * Navigation History
* Transparency
    * Control Domain
    * Control Communication
* Variation
    * Size of the Design Space
    * Openness of the Design Space
* Stimulation
    * Immersion
    * Stimuli



???
These four dimensions describe what a well-designed system achieves.
  
They do not describe what decisions produce it.
  
Navigation doesn't tell you how to build navigability.  
Transparency doesn't tell you what to make transparent.  
Variation doesn't tell you where variation should be available.  
Stimulation doesn't tell you when the artist should be in the loop.
  
And none of them ask: *who* is in control?

The Gieseke framework scores the map, but the five dimensions describe the territory. Configure HOW, WHAT, WHERE, WHEN, and WHO deliberately — and Navigation, Transparency, Variation, Stimulation follow as consequences. That reframing makes the transition feel earned rather than abrupt.

---
template:inverse

# Configuring Creative Control

---

## Configuring Creative Control


To design for creative control, we need to ask:

* **How** does the artist act?
* **What** do they provide?
* **Where** does it land?
* **When** can they intervene?
* **Who** holds agency?

These are *control characteristics* we need to decide on for our systems on algorithmic level.




---
template:inverse

# *How?*
### The Modality of Input

---

.header[Control Characteristics]

## How - User Interaction

> How is a control executed or an input given by an artist?

<br />
.center[<img src="./img/how.png" alt="how" style="width:80%;">]


???
How asks: by what physical or computational act does the artist exert control? In traditional media the answer is direct and embodied — a brushstroke, a chisel strike, a placement. In computational systems, the same question opens into a design problem: the artist must decide how to make control available, not just how to use it. Source: Gieseke et al. (2021): the distinction between on-canvas and separate UI as the two primary modalities, and their different levels of indirection between artist action and output effect.



---
.header[Control Characteristics | How]

## How - User Interaction


* File
* Separate UI
    * Sliders, parameters, menus
    * Need translation between input and effect
* On-Canvas
    * Drawing, placing, guiding
    * Usually local, limited in their effect


???
File: The control is externally given, such as with code or a configuration file.
Separate UI: A separate UI is given through which an artist gives input and activates states. Separate UIs are often in close proximity to the canvas, carefully designed and easily usable. However, because they detach the work from the actual output, separate UIs have a level of indirection. An artist must actively translate the interaction with the separate UI to the resulting output on the canvas.
* On-Canvas: Controls are executed directly on the output canvas. Most of them require activating or selecting a tool in a separate UI, such as selecting a pen for drawing on a canvas. 
* There are cases where controls cannot clearly be classified as either separate UI or on-canvas. A pen, for example, can have different characteristics that an artist needs to set in the UI. The adjustment of settings should be as seamlessly integrated into an on-canvas tool as possible (e.g., with choices appearing as tool tips).


On-canvas control: the artist acts directly on the output surface — drawing, placing, guiding. Separate UI: the artist works through detached controls (sliders, parameters, menus) that require translation between input and effect. Key insight from Gieseke et al.: separate UIs introduce indirection; an artist must actively translate their action into an imagined result. On-canvas controls reduce this cognitive gap — but impose their own constraints on what is expressible. Visual: a parameter panel on the left, a direct sketch-on-canvas interface on the right.


## Direct vs. Indirect Input
Another axis orthogonal to on-canvas/separate UI: how directly does the artist's action map to the output? A drawn stroke that becomes a visual element is more direct than a numerical seed that propagates through multiple algorithmic layers. Thesis link: the distinction between text-based environments (high abstraction, indirect path from code to canvas) and node-based environments (spatialized, more transparent data flow, intermediate states visible) as two architectures of HOW. Neither is superior — they enable different creative relationships with the system.

---
.header[Control Characteristics | How]

## Sketch-Based Input 

Combination of local, direct control and global effect through computation:

* Areas of operation, outlines, layouting
* Directions, guidance fields
* Autocompletion

> For hierarchical composition!

???
Sketch-based input occupies a privileged position at the intersection of embodied and algorithmic authorship. The Gieseke et al. (2017) ornament system is the canonical example: a vector field drawn by hand governs the growth direction of a procedurally generated ornament. This collapses the gap between the artist's embodied act and the system's behavior — and scores exceptionally well on Transparency, because cause and effect are spatially identical. Worth noting: this is also where HOW directly shapes WHO. When the hand governs, authorship stays firmly with the artist even as the system generates.

---
.header[Control Characteristics | How]

## How

How the input is given

--

* Determines *Transparency* making cause and effect legible when input and effect share the same space

--

* Changes what creative acts are possible

--

> The modality of input is not neutral with respect to aesthetics!



???
The key move here is remapping as an aesthetic decision, not a UX one. It is not about making the interface friendlier — it is about expanding the expressive range of what can be said. A system where the artist draws a density field to control particle distribution affords different expressions than one where they type a float value. Same underlying algorithm; completely different authorial relationship. The Transparency link is worth stressing: on-canvas HOW modalities score high on Transparency almost automatically, because the control domain and the output domain are spatially identical.







---
template:inverse

# *What?*
### Content and Level of Abstraction

---

.header[Control Characteristics]

## What - Content

> What does an artist give as input?

<br />
.center[<img src="./img/what.png" alt="what" style="width:90%;">]


---

.header[Control Characteristics]

## What - Content

What is the level of abstraction of the content that an artist works with?

* Code
* Value
* Intermediate
* Element


???
* Code: Input is a syntactically structured formal language.
* Value: The input is a single value, chosen from a range—for example, with a slider.
* Intermediate: The input is visual but abstract, such as sketching a mask or arrows for directionality Artists still have to interpret how the input affects the result.
* Element: The input is a component of the resulting pattern

What asks: what does the artist actually provide as creative input? This is a question of content and abstraction. At one extreme: a single numeric value (opacity = 0.7). At the other: a full exemplar image, a semantic description, or a drawn motif. The level of abstraction is not a technical detail — it determines the granularity of creative intent that can be expressed and the degree to which the system completes, extends, or overrides that intent.


---
.header[Control Characteristics | What]

## Exemplars

* Image
* Element Arrangement
* Element

???
* Image: An example image that should be matched in its entirety. Examples are usually pixel data.
* Element Arrangement: An example element arrangement that should be matched in its entirety. Elements in the arrangement are usually separate shapes and might carry additional data.
* Element: One specific, individual asset that becomes part of the result. Elements can be shapes or pixel data.


Gieseke et al. (2021) identify a set of input content types for pattern generation: exemplar-based (providing a reference pattern the system learns from), parameterized (numerical or slider-based control over separately addressable characteristics), image-based (pixel data used as indirect control), sketch/shape-based (visual structures given as scaffolding), and placing/guiding (explicit positional information). Visual: a diagram placing these on a spectrum from low abstraction (raw values) to high abstraction (reference image or semantic intent).


---
.header[Control Characteristics | What]

## Parameterization

Parameter usually represent certain visual characteristics and their prominence.

* Often non-intuitive, representing abstract system internals rather than perceptual qualities
    * Parameter space vs. design space
* Too many are tedious, too few limit design space

> Notoriously difficult to develop!

???
* Parameterization — the process of identifying and exposing controllable variables of a system — is the most prevalent strategy for managing WHAT in generative practice. From the thesis: parameters "represent certain visual characteristics and their prominence" and a few can control many details. But the challenge is equally clear: parameters are often non-intuitive, representing abstract system internals rather than perceptual qualities. The gap between parameter space and design space is a persistent creative friction. The artist must develop fluency in a language that is not visual.


Parameterization
* Visual Output: Parameters that can adjust visual features directly in the output.
* System/Generation: Parameters that influence the output indirectly, such as parameters for an optimization algorithm or constraints.


The response to non-intuitive parameters is remapping: translating abstract system variables into content that corresponds more closely to a visual or spatial intuition. From the thesis: control textures, procedurally generated fields, and hierarchically grouped parameter bundles all serve this function. From Gieseke et al.: image-based control maps pixel data (brightness, hue, gradient) to system behaviors, providing "transparent control for filling a space." WHAT the artist gives is redesigned to fit the artist's actual mode of thinking. This is not just UX work — it is aesthetic work. Note the connection to Gieseke et al.'s Navigation dimension: the size and legibility of the navigable space is partly a function of how WHAT is structured.


---
.header[Control Characteristics | What]

## What

The content level of interaction determines the expressive vocabulary available.


???

* Numeric parameters → precise but abstract; the artist must speak in system language
* Sketches, images, spatial structures → embodied and relational; the artist speaks in visual language

--

* We need *meaningful interface metaphors*.


???
* — input that carries creative intent without loss in translation

--

> The artist provides the **vocabulary**. The system provides the **grammar**.



???
* But vocabularies can be impoverished or rich.

The metaphor of vocabulary vs. grammar is the core takeaway. A system that only exposes numeric parameters forces the artist to translate every creative impulse into an abstraction — the expressive range is not limited by the algorithm, but by the language available to address it. Meaningful interface metaphors are the design response: finding representational forms for input that map onto how artists actually think. This connects directly back to Transparency in the Gieseke framework — if the artist cannot read the relationship between what they give and what they get, the vocabulary is effectively impoverished regardless of its theoretical richness.


---
template:inverse

# *Where?*
### The Spatial Scope of Control

---
.header[Control Characteristics]

## Where - Canvas

> Where does the input have an effect and what is the area of influence?

<br />
.center[<img src="./img/where.png" alt="where" style="width:80%;">]



???
* The input can have global influence, regional, e.g., on a drawn curve or local, e.g., on one specific element.
* Does a control act on the **entire output** — or on a **specific region**?

Global control: one decision shapes everything — scale, density, color shift applied uniformly. Local control: the artist can target specific regions, elements, or layers with different behaviors. Gieseke et al. identify several mechanisms for spatial targeting: curves and paths drawn on the canvas, masks (regions defined by shapes or images), and flow fields (directional controls that vary spatially). Visual: the same generative pattern with global parameter change on the left, region-specific mask-based control on the right — dramatically different expressive results.



---
.header[Control Characteristics | Where]

## Where


* In traditional media: almost always local and direct
    * A brushstroke affects exactly where it lands.

--

* In computational systems: the default is often the opposite
    * A single parameter value governs the entire canvas.


--


* It is a spectrum from *automatic / global* to *manual / local*

???

* WHERE is therefore a design dimension that must be **explicitly addressed** — it does not emerge by default
* The inversion is the key provocation here: traditional media is local by default, computational systems are global by default. This means spatial targeting is not a feature that comes for free — it has to be deliberately designed into the system architecture before the artist can use it. The Gieseke spectrum from automatic/global to manual/local is the organizing structure for the next three slides.


---
.header[Control Characteristics | Where]

## Global-to-Local Strategies

Artists routinely work global-to-local: establish overall character first, refine local detail second.

???
* This is not a limitation — it mirrors how any skilled visual artist builds structure before detail

--

> Computationally the global to local spectrum must be **architecturally planned in advance**


???
The critical insight is the asymmetry between traditional and computational practice. A painter can decide mid-process to work locally — they just move the brush. A generative artist cannot decide mid-process to have local control if the system was not designed for it. This makes WHERE a front-loaded architectural decision with downstream aesthetic consequences. The Variation link is worth lingering on: a system with only global control can produce a wide range of global looks, but its compositional range — the ability to produce spatially differentiated, hierarchically organized work — is structurally capped.


---
.header[Control Characteristics | Where]

## Where

The openness of the design space is partly determined by how spatially differentiated control can be and with that the *Variation* of the system.

--

> Trade-off between global automation and local manual manufacturing!
  


???

The degree of spatial targeting available in a system shapes what kinds of compositions are possible. Systems with only global control can produce internally consistent but spatially homogeneous outputs. Systems with rich spatial targeting can produce differentiated, hierarchically organized, and locally responsive work. Gieseke et al. identify this as one of the key limitations of many current procedural systems: the "trade-off between global automation and local manual manufacturing" is rarely solved elegantly. WHERE you can act determines the compositional range of what you can make.

---
template:inverse

# *When?*
### The Temporal Position of Control

---
.header[Control Characteristics]

## When - Timeline

> When is the input given and at what time in the creation process is the control executed?

<br />
.center[<img src="./img/when.png" alt="when" style="width:76%;">]


???
* ASK: How many systems they use actually offer all three intervention points?
* Input can be given before the creation process, during it when parts of the results are already visible, or after, when the result is visible and can be adjusted retrospectively.

---
.header[Control Characteristics | When]

## When

* Initialization: before the system runs
* Execution: real-time interaction during the process
* Post-hoc: curation and post-processing after the fact

--

* In traditional media: *when* is mostly synonymous with *now*
    * The artist acts in the immediate present.

--

* In computational systems: *when* can be freely designed
    * Sequenced, gated, branched, looped, deferred, etc.


???
In traditional media, temporal access to the work is continuous and assumed. In computational systems it is a design decision — and one that is often made implicitly rather than deliberately. A system that only 
allows initialization-stage control forces a speculative, non-dialogic mode of authorship: the artist sets conditions and observes consequences, with no ability to intervene mid-process. The Stimulation link is direct: immersion requires a tight feedback loop, and a tight feedback loop requires that WHEN includes execution-stage access.  


Access patterns:
* Continuous — the artist can intervene at any moment
* Discrete — intervention is possible only at defined checkpoints
* Triggered — intervention is activated by a system event or threshold
* Scheduled — control is time-indexed (e.g., parameter curves, keyframes)

Closure:
* Locked — intervention points are fixed and cannot be added
* Open — the artist can introduce new intervention points at any time



---
.header[Control Characteristics | When]

## Temporal Evolution

--

* Stateless systems — each frame is independent; the past leaves no trace
* Stateful systems — the system accumulates, remembers, responds to prior states

Statefulness is hard, e.g. on the GPU!

???
* E.g., on the GPU: statefulness requires explicit memory management across the render pipeline with buffers, ping-pong textures, persistent render targets.
* The artist sets initial conditions. The system evolves.
* WHEN becomes **distributed across time**: each prior state mediates the next intervention

--

* History-keeping — the ability to return to, compare, and branch from prior 
states is itself a temporal control mechanism

--

* Non-trivial engineering problems! Most creative coding environments underserve this...


???
Statelessness is not a design choice in GPU pipelines — it is the architectural default. Each fragment shader call is independent by design; carrying state forward requires deliberate engineering: ping-pong framebuffers, feedback textures, or hybrid CPU-GPU state management. This means that temporal richness — accumulation, memory, evolution — costs significantly more to implement than a single-frame system. History-keeping compounds this: storing, indexing, and restoring prior states requires persistent memory structures that most real-time environments do not provide out of the box. 

The creative consequence is that many systems that could be temporally rich are stateless by default simply because statefulness is hard — not because it was deliberately chosen.

???
* From the thesis Ch. 4: systems that maintain state across the draw-loop — accumulating, remembering, responding to prior states — introduce a form of temporal agency that is not reducible to any single moment of control. The artist sets initial conditions; the system evolves. Parameters may be animated, accumulated, or driven by external data. This creates a situation where WHEN is distributed across time: the artist acts at multiple points, and the system's own temporal behavior mediates between those interventions. History-keeping as a strategy: the ability to return to, compare, and branch from prior states is a temporal control mechanism that most Creative Coding tools underserve.

---
.header[Control Characteristics | When]

## When

> The artist is "in conversation" with the system, and *when* defines the rhythm and density of that conversation.

???

The temporal structure of control determines whether the artist is present as a continuous force or as an initiating architect who then withdraws. Systems with rich real-time WHEN afford ongoing dialogue; systems with locked initialization afford front-loaded intention-setting followed by observation. Neither is superior — they produce different aesthetic relationships between artist and work. But they must be chosen deliberately. The thesis frames this as the dialogic nature of the creative process: the artist is "in conversation" with the system, and WHEN defines the rhythm and density of that conversation.

---
template:inverse

# *Who?*
### Agency, Authorship, and the Co-Agency Spectrum

---
.header[Control Characteristics]

## Who - User

> Who has the skill set needed to provide the input?

<br />
.center[<img src="./img/who.png" alt="who" style="width:90%;">]

--

> Who is authoring: human or system?


---
.header[Control Characteristics | Who]

## The Question the Survey Cannot Answer
Gieseke et al. (2021) systematically map HOW, WHAT, WHERE, and WHEN — corresponding, at the system level, to Navigation, Transparency, Variation, and Stimulation as evaluative dimensions. But neither the taxonomy nor the CSI addresses the fifth question: who is in control? This is not an oversight — it is a boundary. WHO belongs to a different register of analysis: not algorithm design but agency theory. The thesis (Ch. 2) provides the framework. Opening provocation: if the system produces behavior the artist did not anticipate — who made that?

---
.header[Control Characteristics | Who]

## The Co-Agency Spectrum
From the thesis: creative work with generative systems is not a binary between the artist controlling the system and the system controlling itself. It is a spectrum — from fully artist-led (the system as obedient tool) to fully system-led (the artist as observer of autonomous behavior). At each position, distinct artist-system relationships emerge: Tool-Protagonist (direct execution), Delegate-Manager (conductor/project manager role), Collaborator (equal creative partner), Curator (responds to what the system produces). Visual: the co-agency spectrum diagram from the thesis. The key insight: working with generative systems is not about ceding control — it is about distributing it.

---
.header[Control Characteristics | Who]

## How Architectural Choices Position the WHO
The WHO question is not answered by intent alone — it is determined by architectural choices. From the thesis Ch. 4: introducing randomness shifts creative agency toward the system; rule-based systems with emergent behavior shift it further; agent-based systems can produce behavior that genuinely exceeds the artist's predictive capacity. The same system architecture that produces surprise also redistributes authorship. The thesis is explicit: "autonomy" describes operational independence; "agency" describes impact on the creative outcome. A system can be operationally autonomous but have low aesthetic agency — or vice versa.

---
.header[Control Characteristics | Who]

## Intention, Curation, and the Inalienability of the WHO
From the thesis: no matter how autonomous a generative system becomes, the artist retains what the thesis calls "artistic control" — the combination of intention (the conceptual framework that initializes and continuously shapes the process) and curation (the iterative act of selection and evaluation). These are the dimensions of WHO that cannot be delegated. Curation is convergent thinking — the creative complement to the system's divergent generation. Even when the artist cannot predict the output, they remain the entity that decides whether it matters. This is the irreducibly human component of the WHO.

---
.header[Control Characteristics | Who]

##  WHO Determines Aesthetic Meaning
The distribution of WHO across artist and system is not just a question of authorship — it shapes the kind of meaning the work can carry. A work made by an artist exercising tight intentional control carries a different aesthetic quality than one shaped by emergent system behavior that the artist curates but cannot author. Neither is more valuable, but they are different. The thesis quotes Boden: "The autonomy in the intentional sense of the generative systems does not exist." But something else exists — a form of creative surprise that the artist creates the conditions for, without being able to produce directly. That gap is where generative aesthetics lives.

---
template: inverse

# Five Dimensions, One Design Space

---

## The Five Dimensions Are Coupled
HOW, WHAT, WHERE, WHEN, and WHO are not independent variables. A decision about WHAT — introducing exemplar-based input instead of parametric control — changes HOW interaction works, WHERE it applies, and WHEN it is possible, and it redistributes WHO by reducing the artist's ability to specify and increasing the system's generative latitude. Any change in one dimension propagates. The design space is not flat — it is a high-dimensional configuration space in which every choice has consequences across all axes.

Note the relationship to the Gieseke et al. framework: Navigation, Transparency, Variation, and Stimulation are evaluative outcomes; HOW, WHAT, WHERE, WHEN, and WHO are the generative inputs to those outcomes. Configuring the five dimensions well is what produces a system that scores well on the four evaluative criteria — plus, now, a fifth: meaningful authorship.


---

## The Same Five Questions Apply to Watercolor on Paper
Return to the opening image: watercolor on paper. Walk through all five dimensions. HOW: direct, on-canvas, embodied. WHAT: pigment, water ratio, pressure — low-abstraction, physical parameters. WHERE: wherever the brush lands, with bleed behavior that propagates outward. WHEN: continuous, real-time, non-reversible. WHO: fully artist-led, with the material as an agent of unpredictability (bleed, granulation, drying) that the artist works with but does not control. The point: digital generative systems do not introduce a new problem. They scale the same problem into a design space that must be explicitly and consciously architected.

---

## Emergent Aesthetics as a Configured Outcome
The aesthetic qualities that emerge from a generative system — complexity, surprise, coherence, expression — are not accidental properties of the algorithm. They are functions of how the five dimensions are configured. A system with rich spatial targeting (WHERE), real-time feedback (WHEN), sketch-based input (HOW + WHAT), and a deliberately calibrated co-agency spectrum (WHO) will produce different aesthetic qualities than one with global parameters, deferred feedback, and full autonomy. Aesthetic quality is not a byproduct. It is the outcome of design decisions made across all five dimensions. This is what it means to be the author of a generative system.

---
template: inverse

# Authorship is a Configuration

---
## The Practical Implication
If the five dimensions structure creative control, then designing a generative system means making explicit decisions about each of them. HOW will the artist interact? WHAT will they provide? WHERE will control act? WHEN in the process will it be available? WHO will hold agency at each stage? These are not interface questions or UX questions. They are authorial questions. The thesis frames this as the shift from artist-as-craftsperson to artist-as-system-architect. The system architect makes decisions that are not about individual outputs but about the entire class of outputs the system can produce.

---
## The Open Question
Every generative system instantiates a theory of creative control — whether or not its maker has articulated it. The five dimensions are always configured; the question is whether they are configured deliberately. Closing provocation: when you next design a system, or teach a student to design one, ask not "does it work?" but: How does the artist act? What do they give? Where does it land? When can they intervene? And who, at the end, is responsible for what emerges?

