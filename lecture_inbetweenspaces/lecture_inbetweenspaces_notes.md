name: inverse
layout: true
class: center, middle, inverse
---


# In-Between Spaces

### Prof. Dr. Lena Gieseke | l.gieseke@filmuniversitaet.de  

#### Film University Babelsberg KONRAD WOLF



---
layout:false

## Translational Media: From Gesture to Code to Space

This talk examines computational pipelines that translate physical behaviour into algorithmic systems: for example, gesture into fields, architectural layouts into navigable graph structures, and performance movements into agent-based simulation logic. It explores how such translations shape aesthetics, interaction, and our understanding of space as both computational construct and experiential domain.

Storyline:
- Thinking about bringing spaces together is meaningful, TODO:why
- going from analog to virtual space is not just an artistic problem, see random number generation
- TODO: example that go from Gesture to Code to Space
- Data morphism example
- In-between spaces, what happens in the "in-between"

The Space That Wasn't There Before

Storyline: When we translate physical behavior into algorithmic systems, I propose the perspective that we are not simply moving something across, but rather — in most cases — producing a third space that belongs fully to neither domain.

Take-home Message: From this, I propose thinking about computational translation less as world-copying and more as world-building.

Opens with the random number generation problem (computers cannot produce true randomness, they simulate it, and the simulation is structurally different from the thing it mimics). This becomes the master metaphor: when you translate physical behavior into algorithmic systems, you don't just move something across — you produce a third space that belongs to neither domain. Gesture fields, navigation graphs, agent simulations are not representations of reality; they are new ontological objects with their own properties. Take-home: Computational translation is world-building, not world-copying.


----

1. The Randomness Problem
(cite / reference Alex)
Consider what happens when we try to bring something from the real world into computation. Take randomness as a first example. Random numbers play a key role in computational processes ranging from the generation of secure cryptographic keys to the random initialization of weights during AI network training. Yet computers cannot produce true randomness. They simulate it using deterministic algorithms — PRNGs — and that simulation is structurally different from the thing it mimics. It has period lengths, statistical biases, seeds. In other words, the move from real-world phenomenon to computational representation is not a neutral transfer. Something changes in the crossing.

One response to this problem is to extract seeds from highly complex physical processes. True random number generators (TRNGs) draw on the latent entropy in chaotic physical phenomena: atmospheric noise, radioactive decay, or — perhaps most evocatively — lava lamps. In the San Francisco offices of the internet security firm Cloudflare, a wall of lava lamps is filmed around the clock, providing cryptographic keys for roughly 20% of the world's internet traffic. Known as Lavarand, the system translates frames from the live feed into numeric seeds for a PRNG. The lamps' chaotic fluid motion, combined with atmospheric and lighting conditions, makes the seeds practically impossible to predict algorithmically. Objects designed purely for human visual pleasure become, in this context, operational instruments for computation.

And here is where it gets interesting: what emerges on the other side is not a failed copy. The simulation is a new kind of object — one that behaves like randomness under certain conditions, but operates according to its own internal logic. It is neither the original phenomenon nor a mere approximation of it. It is something third.

This is the master metaphor for everything that follows.


2. What Do We Mean by Translation?
Computational translation is typically framed as transfer (moving something from one domain into another), but this framing obscures what is actually happening. Introduce the alternative frame: translation as production of a third space. Lead over to examples


3. Example 1 — Gesture into Fields

Slide 1 — What is a Gesture?
Anchoring the source domain
A brief phenomenological provocation: gesture is embodied, continuous, intentional, and unrepeatable. It carries weight, hesitation, momentum — properties that belong to a body in time. One striking visual: a dancer or performer mid-motion, deliberately blurred. Key question planted for the audience: what would it even mean to "capture" this?

Slide 2 — The Capture Problem
Introducing the translation moment
How gesture enters computation: infrared cameras, skeletal tracking, coordinate streams. Show the same gesture as a blurred photograph versus a raw data stream of positional values. The point is already made here: warmth, weight, and intention are gone. What remains is a sequence of numbers. Something changed in the crossing — but we have not yet arrived at the interesting part.

Slide 3 — Body Paint (2009), Memo Akten
The translation in action
Akten's infrared camera does not record the body — it records movement. Speed, acceleration, curvature, and size of motion are extracted and fed into a fluid simulation, producing strokes, drips, spirals, and splashes on a projected canvas. Show the installation image alongside the output field. Crucially: the system does not see people at all, only movement. Anything moving — living or not — triggers the same response. The body has already been abstracted away.

Slide 4 — What the Field Has That the Gesture Doesn't
The third space emerges
The fluid field produced by Body Paint has viscosity, diffusion rates, attractor behavior, gradient flows — properties that are physically well-defined but were never properties of the original gesture. A side-by-side: gesture (embodied, singular, temporal) versus field (spatial, persistent, iterable, generative). Akten's own framing supports the argument directly: what matters is not the painting at the end, but the sensation of playing. The output has escaped the input. It is a new kind of object.

Slide 5 — The Thinking Ocean (2024), Memo Akten & Katie Hofstadter
The field becomes a world
Choreographer Alexander Whitley's motion capture data drives a fluid dynamics simulation governed by Navier-Stokes equations at the Whitney Museum. The ocean produced is not a metaphor for the body — it is caused by the body, yet operates entirely according to fluid physics: drifting particulate matter, bubble dynamics, pressure gradients. The simulation starts producing behavior the original performer never executed. Akten's framing here is the sharpest version of the third-space argument: the piece proposes that oceans and computers are expressions of the same underlying principles. The third space is not a copy of either domain — it is a system with its own rules.

Slide 6 — Transition Question
Bridge to Case 2
Content: Minimal text. One closing provocation: the field is no longer about the gesture — it is a space with its own rules. Then pivot: what happens when the source domain is not a body but a building?

Case 2 — Architectural Layout into Navigation Graphs: Revised Slide Breakdown
10 min, 6 slides

Slide 1 — What is Architectural Space?
Anchoring the source domain
Architecture is experienced as a continuous, embodied phenomenon: enclosure, threshold, depth, the pull of a corridor, the release of an atrium. Space is not a collection of nodes and edges — it carries weight, light, atmosphere, material resistance, social meaning. Key question planted: what would it mean to "capture" this?

Slide 2 — Space Syntax: The Translation Framework
Introducing the graph
Bill Hillier and Julienne Hanson's Space Syntax (UCL, 1980s) offers the canonical example. Rooms or street segments become nodes, connections become edges, traversal difficulty becomes weights. Show a floor plan on the left, its justified graph on the right — they look nothing alike. The graph has integration values, choice measures, topological depth: properties that are mathematically well-defined but were never properties of walls or corridors. A real-world instance worth one sentence: Space Syntax's pedestrian model for the Trafalgar Square redesign with Foster and Partners predicted movement flows from graph topology alone, with no reference to how the space actually looks or feels.

Slide 3 — What the Graph Has That the Building Doesn't
The third space emerges
The graph reveals properties invisible to the inhabitant: betweenness centrality, integration scores, dead ends defined by connectivity rather than by walls. A corridor that feels open may be a topological dead end; a cramped passageway may be the most integrated node in the building. The graph is not a lesser representation of spatial experience — it is a different kind of object operating by its own logic. And it starts making predictions about how people actually move, which the building itself cannot make.

Slide 4 — Million Dollar Blocks (2006), Laura Kurgan / Spatial Information Design Lab, Columbia
The creative-critical instance
Kurgan's project translates the urban geometry of five American cities into a graph of incarceration flows — mapping where prisoners come from and how public money circulates between city blocks and the prison system. The city is not represented as a visual environment but as a connectivity and expenditure graph. The resulting maps, now in MoMA's permanent collection, reveal a spatial logic that is completely invisible at street level: entire neighborhoods functioning as topological dead ends in the graph of civic life. The map does not show the city as it looks — it shows the city as it operates. This is the third space argument made visible and politically urgent. The graph produces knowledge that the physical city cannot.

Slide 5 — The Façade-Tilted Bird's-Eye View
Your own research as concrete instance
The façade-tilted bird's-eye view technique for urban pedestrian navigation is a direct instance of the same translation logic. Urban geometry — facades, intersections, open space — is reorganized according to navigational relevance, foregrounding what the graph considers meaningful: orientation, branching, landmark proximity. The resulting representation does not look like the city. Ask the provocation directly: when a pedestrian navigates using this representation, are they moving through the city, or through the graph of the city?


Case 3 — Ecological Data into Navigable Space
10 min, 5 slides

Slide 1 — A Different Kind of Source Domain
The escalation
In Cases 1 and 2, the source domain was something humans can directly inhabit: a body, a building. What happens when the source domain is a phenomenon we can measure but never experience? Ecological and animal data — movement trajectories, sensory ranges, perceptual physiology — describes worlds that are structurally inaccessible to human perception. The translation here is not just a technical problem. It is an epistemological one. The question is not only what do we lose in the crossing but what are we even trying to cross into?

Slide 2 — Julie Freeman, The Lake (2005)
Translation as attentiveness
Sixteen freshwater fish in a lake, electronically tagged. Their location, speed, direction, and proximity to each other are captured continuously and translated into a real-time audiovisual installation in an 80-foot cylindrical tower beside the water. The fish are never represented visually — what the audience encounters is a sound and animation space derived entirely from behavioral data. The fish do not know they are composing music. The resulting space belongs to neither domain: it is not the lake, and it is not an artwork in any traditional sense. Freeman describes her interest as understanding the underwater environment through what the data makes available — not through what the eye can see. The installation is literally built from non-perceptible data made experiential.

Slide 3 — What the Space Has That the Lake Doesn't
The third space emerges
The computational space produced by The Lake has musical structure, harmonic relationships, rhythmic patterns — properties that emerge from the translation logic, not from fish behavior itself. Proximity triggers interaction rules that produce emergent soundscapes no single fish could generate alone. The space is generative: it produces aesthetic events that are caused by the animals but not authored by them. This is the third-space argument in its sharpest form: the space is irreducible to its source, and yet the source is the only reason it exists.

Slide 4 — Marshmallow Laser Feast, In the Eyes of the Animal (2015)
Translation as world-construction
LiDAR scans, CT scans of animal anatomy, drone footage, and bioacoustic recordings from Grizedale Forest are processed into a VR environment in which the viewer navigates the forest through the perceptual apparatus of four woodland species — a midge, a dragonfly, a frog, an owl. A dragonfly experiences time approximately ten times faster than a human and sees in twelve color wavelengths. The midge detects CO₂ clouds at a distance. These perceptual parameters are encoded into the real-time rendering pipeline, reshaping what the viewer can see and when. The resulting space is not the forest. It is not the animal's experience either — the artists acknowledge it is speculative, an artistic interpretation built from scientific data about physiology. It is a third space: a computational world constructed from ecological data, navigable by humans, belonging to neither.

Slide 5 — Transition to Synthesis
Bridge to Section 6
Minimal text. Closing provocation: in each of these three cases — gesture, architecture, ecology — the translation produces a space that could not have existed without its source, yet cannot be reduced to it. What kind of objects are these spaces? And what are our responsibilities toward the worlds we build from data we do not own?


Section 6 — Synthesis: Datamorphism and the Properties of the Third Space

10 min, 5 slides

Slide 1 — What Do These Three Cases Share? Establishing the pattern

A minimal comparative table or three-column visual: gesture → field, architecture → graph, ecology → navigable space. In each case: the source domain is physical and experiential; the translation is computational and selective; the output has properties the source never had. The question the slide poses without yet answering: is there a name for what happens in the middle?

Slide 2 — Introducing Datamorphism The theoretical lens

In related work, we proposed datamorphism to describe how data properties — their size, their mapping logic, and their meta-communication — actively shape both the form of a data-based representation and its reception by an audience. The concept was developed in the context of data art about other-than-human phenomena, but it applies directly here. The key insight: translation is never neutral. The codec is an argument. What you encode, how you map it, and what you make visible to the audience are all decisions that produce the third space — not merely describe it.

One slide, kept lean. Introduce the term, give it one sentence of definition, and make clear it is your own theoretical framework.

Slide 3 — Three Properties of the Third Space 

Emergent structure — the third space has properties that were not present in the source and could not have been predicted from it alone. The fluid field has attractors; the navigation graph has centrality; the lake installation has harmonic emergence.

Generativity beyond the source — the third space produces outputs, events, or behaviors that exceed what the source could generate. The field produces movements no body made; the graph predicts flows the building cannot; the fish installation composes music no fish intended.

Feedback potential — the third space begins to shape behavior in the original domain. The navigation representation changes how pedestrians walk. The datamorphic artwork changes how audiences perceive the phenomenon it represents. The encoded space starts encoding us.

Slide 4 — The Audience Is Already Inside The perceptual and ontological situation

Datamorphism sharpens the argument at the level of reception. When an audience encounters the simulation — the fluid field, the navigation map, the fish soundscape — they are not standing outside the third space looking in. They are already operating within it, whether they know it or not. The meta-communication property of datamorphism is relevant here: awareness of the translation layer changes the experience, but the third space exerts its logic regardless. This is what makes the in-between not a gap but a domain.

One strong visual: a person navigating with the façade-tilted view, or standing in The Lake installation. The caption: are they in the city, or in the graph of the city?

Slide 5 — From Translation to World-Building 

If the third space is real — if it has its own structure, generativity, and feedback effects — then the act of designing the pipeline is not a technical decision. It is an ontological one. The pipeline author decides what exists in the third space. This reframes the entire practice of computational translation: not as a means of representing the world, but as a means of producing new parts of it. One line to close the section and open the final movement: we have been building worlds. The question is whether we have been doing so deliberately.

Section 7 — Closing: World-Building, Not World-Copying


Slide 1 — Returning to the Beginning The PRNG callback

A single image: the Cloudflare lava lamp wall. The opening provocation revisited. The PRNG was never a failed copy of randomness — it was a new kind of object, built deliberately for a purpose, with its own internal logic and its own real-world effects. It secures 20% of the world's internet traffic. The third space it produces is consequential. The same is true, I want to propose, of every computational pipeline that translates physical behavior into algorithmic systems.

Slide 2 — The Take-Home

Computational translation is not world-copying. It is world-building.


Slide 3 — The Open Question Closing without resolution

If we accept that computational pipelines produce third spaces — spaces with emergent structure, generativity, and feedback potential — then every design decision in the pipeline carries authorial and ethical weight. Who decides what gets encoded? What is lost in the translation, and for whom? When the third space starts shaping behavior in the original domain, who is responsible?

If we are building worlds, what does that oblige us to?


## Outline

Talk Outline: "The Space That Wasn't There Before"

1. Opening — The Randomness Problem
2. Framing — What Do We Mean by Translation?
3. Case 1 — Gesture into Fields
    * What is a Gesture?
    * The Capture Problem
    * Example, e.g., Body Paint (2009), Memo Akten
    * What the Field Has That the Gesture Doesn't
    * The Thinking Ocean (2024), Memo Akten & Katie Hofstadter
    * Transition Question
4. Case 2 — Architectural Layout into Navigation Graphs
    * What is Architectural Space?
    * Space Syntax: The Translation Framework
    * What the Graph Has That the Building Doesn't
    * Million Dollar Blocks (2006), Laura Kurgan
    * The Façade-Tilted Bird's-Eye View
5. Case 3 — Ecological Data into Navigable Space
    * A Different Kind of Source Domain
    * Julie Freeman, The Lake (2005)
    * What the Space Has That the Lake Doesn't
    * Marshmallow Laser Feast, In the Eyes of the Animal (2015)
    * Transition to Synthesis
6. Synthesis —  The Properties of the Third Space (on the example of Datamorphism)
    * What Do These Three Cases Share?
    * Introducing Datamorphism
    * Three Properties of the Third Space
    * The Audience Is Already Inside
    * From Translation to World-Building
7. Closing — World-Building, Not World-Copying
    * Returning to the Beginning
    * The Take-Home
    * The Open Question