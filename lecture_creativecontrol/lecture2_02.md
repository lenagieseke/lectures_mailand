# Lecture 2: How, What, Where, When, Who — Mechanisms for Creative Control

**Duration:** ~60–65 min

**Storyline:** CS publications routinely claim their systems are "artist-friendly" or "creatively usable" and validate those claims with small user studies. User studies, when executed properly, are a legitimate form of validation — but they are not the only one, and on their own they leave the underlying question underspecified: what does creative usability actually consist of? The field has made previous attempts to answer this. We examine those attempts, identify what they leave open, and propose that creative control is a configuration space of five interacting dimensions: How, What, Where, When, and Who. The aesthetic qualities that emerge from any creative system — algorithmic or analog — are shaped by how those dimensions are configured and how they interact. These dimensions also give researchers and practitioners a shared vocabulary for asking more precise questions about what a system actually affords.

**Take-home:** "Creative control" is not a diffuse property but something that can be precisely described, designed for, and evaluated.

---

## Talk Outline

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

## Section 1 — Opening Provocation: One Act, Five Questions
**5 min, 2 slides**

### Slide 1 — The Watercolor Test
A single image: a hand applying watercolor to paper. Five questions posed alongside it, simply: How is input given? What does the artist provide? Where does it act? When in the process? And who is in control? No answers yet — only the questions. The argument planted for the audience: these are not questions about medium. They are questions about the structure of any creative act.

### Slide 2 — The Same Questions, Different System
Same five questions, now posed over a screenshot of a node-based generative system — e.g., a TouchDesigner patch producing an evolving visual field. The point: the questions map perfectly. What changes is not the structure of creative control but its implementation. This talk investigates what happens to each dimension when the medium becomes computational — and what that means for authorship and expression.

---

## Section 2 — The Problem of Defining Creative Usability
**6 min, 3 slides**

### Slide 1 — Why "Artist-Friendly" Isn't Good Enough
CS and HCI publications routinely claim their systems are "artist-friendly" or "creatively usable" — and validate those claims with user studies. When executed properly, user studies are a legitimate form of validation. But they leave the underlying question underspecified: what does creative usability actually consist of? What are we measuring when we say a system supports creativity?

The problem is not a lack of seriousness. It is a definitional one. Creativity is:
- Ill-defined as a construct, and
- A topic that draws insights from psychology, cognitive science, philosophy, and HCI simultaneously — making it notoriously difficult to operationalize.

Source: Frich et al. (2018, 2019), Remy et al. (2020) — a sequence of meta-studies calling for more rigorous evaluation and clearer definitions of creativity in HCI research.

### Slide 2 — Creativity Support Tools: The HCI Tradition
The field of Creativity Support Tools (CSTs) has been central to HCI since Shneiderman's foundational 2007 paper. The ambition: design tools that accelerate discovery and lower the threshold for creative production. The challenge: CST research has historically conflated two distinct questions — whether a tool enables creative outcomes, and whether the tool itself is the source of creative agency.

Source: Shneiderman (2007). Visual: timeline of CST research from 2000–2020 showing volume of publications and the growing methodological critique.

### Slide 3 — The Call for Rigor
Frich et al. (2018) surveyed twenty years of creativity research in HCI and identified a persistent gap: most studies assess whether users feel creative, not whether the system's architecture enables or constrains creative control. Remy et al. (2020) sharpen this: evaluation methods for CSTs remain inconsistent, and user-perceived creativity does not reliably track with the structural affordances of the system being studied.

The implication: we need evaluation on an algorithmic level — a vocabulary that describes what a system structurally affords, as a subset of (not a replacement for) user-study-based assessment.

---

## Section 3 — Existing Frameworks — And What They Leave Open
**8 min, 3 slides**

### Slide 1 — The Creativity Support Index
The most widely used instrument for evaluating creativity support is the Creativity Support Index (CSI), developed by Cherry and Latulipe (2014). CSI is a psychometric survey instrument that measures how well a tool enables creativity across six dimensions: exploration, expressiveness, immersion, enjoyment, results worth effort, and collaboration.

CSI is rigorous within its own register — it provides quantifiable, comparable scores across tools. But it operates entirely at the user-experience level. It tells us how users feel about the system. It does not describe the system's internal architecture or explain why those feelings arise. As a diagnostic tool for system design, it is post-hoc: it can tell you that your system scored low on exploration, but not where in the architecture the problem lives.

Source: Cherry and Latulipe (2014).

### Slide 2 — A Closer Attempt: Navigation, Transparency, Variation, Stimulation
Gieseke et al. (2021), in their survey of control mechanisms for creative pattern generation, propose four dimensions that operate closer to the algorithmic level:

**Navigation** — whether a creative process is efficiently manageable and controllable. Sub-dimensions: interactivity, number of controls, navigation history.

**Transparency** — clarity of cause-and-effect within the system. Sub-dimensions: control domain (what does a control affect?), control communication (how legibly is that effect conveyed?).

**Variation** — how visually different the achievable results can be. Sub-dimensions: size of the design space, openness of the design space.

**Stimulation** — how well a system supports pleasurable, immersive creative workflow. Sub-dimensions: immersion, stimuli.

This framework is significantly more structural than CSI. It gives researchers and practitioners a vocabulary for system-level analysis rather than user-feeling assessment.

Source: Gieseke et al. (2021). Visual: a 2x2 grid or taxonomy diagram of the four dimensions and their sub-components.

### Slide 3 — What the Survey Cannot Answer
Gieseke et al.'s four dimensions are a substantial advance. But the survey — by design — addresses the what, where, how, and when of control mechanisms. It systematically maps input modes, spatial scope, and temporal structure.

What it does not address is the fifth question: who is in control?

This is not an oversight — it is a boundary. The question of agency and authorship belongs to a different register of analysis: not algorithm design but the theory of creative intentionality. Without the WHO dimension, a system can score well on Navigation, Transparency, Variation, and Stimulation, and still leave the fundamental question of creative authorship unresolved.

Closing provocation for the section: if a system produces behavior the artist did not anticipate — who made that? Navigation and Transparency cannot answer this question. We need a fifth dimension.

---

## Section 4 — HOW: The Modality of Input
**10 min, 5 slides**

### Slide 1 — What "How" Means
How asks: by what physical or computational act does the artist exert control? In traditional media the answer is direct and embodied — a brushstroke, a chisel strike, a placement. In computational systems, the same question opens into a design problem: the artist must decide how to make control available, not just how to use it. Source: Gieseke et al. (2021): the distinction between on-canvas and separate UI as the two primary modalities, and their different levels of indirection between artist action and output effect.

### Slide 2 — On-Canvas vs. Separate UI
On-canvas control: the artist acts directly on the output surface — drawing, placing, guiding. Separate UI: the artist works through detached controls (sliders, parameters, menus) that require translation between input and effect. Key insight from Gieseke et al.: separate UIs introduce indirection; an artist must actively translate their action into an imagined result. On-canvas controls reduce this cognitive gap — but impose their own constraints on what is expressible. Visual: a parameter panel on the left, a direct sketch-on-canvas interface on the right.

### Slide 3 — Direct vs. Indirect Input
Another axis orthogonal to on-canvas/separate UI: how directly does the artist's action map to the output? A drawn stroke that becomes a visual element is more direct than a numerical seed that propagates through multiple algorithmic layers. Thesis link: the distinction between text-based environments (high abstraction, indirect path from code to canvas) and node-based environments (spatialized, more transparent data flow, intermediate states visible) as two architectures of HOW. Neither is superior — they enable different creative relationships with the system.

### Slide 4 — Sketch-Based Input as a Special Case
Sketch-based input occupies a privileged position: it is on-canvas, direct, and low-threshold, yet feeds into algorithmic processes. Show an example of sketch-based control in pattern generation — a vector field drawn by hand that governs the growth direction of a procedurally generated ornament (Gieseke et al. 2017 system referenced in the survey). This collapses the gap between the artist's embodied act and the system's behavior. The hand doesn't just mark — it governs.

### Slide 5 — How Shapes Aesthetic Quality
The modality of input is not neutral with respect to aesthetics. A system controllable only through sliders produces a different kind of authorial fingerprint than one responsive to drawing, gesture, or external sensor data. Thesis link: remapping controls — the strategy of translating raw computational parameters into spatially or visually meaningful controls — is precisely an intervention at the level of HOW. By changing how input is given, the artist changes what creative acts become possible and thus what expressions are reachable. Note the connection back to Gieseke et al.'s Transparency dimension: HOW determines whether cause and effect are legible.

---

## Section 5 — WHAT: Content and Level of Abstraction
**10 min, 5 slides**

### Slide 1 — What "What" Means
What asks: what does the artist actually provide as creative input? This is a question of content and abstraction. At one extreme: a single numeric value (opacity = 0.7). At the other: a full exemplar image, a semantic description, or a drawn motif. The level of abstraction is not a technical detail — it determines the granularity of creative intent that can be expressed and the degree to which the system completes, extends, or overrides that intent.

### Slide 2 — The Abstraction Spectrum
Gieseke et al. (2021) identify a set of input content types for pattern generation: exemplar-based (providing a reference pattern the system learns from), parameterized (numerical or slider-based control over separately addressable characteristics), image-based (pixel data used as indirect control), sketch/shape-based (visual structures given as scaffolding), and placing/guiding (explicit positional information). Visual: a diagram placing these on a spectrum from low abstraction (raw values) to high abstraction (reference image or semantic intent).

### Slide 3 — Parameterization: The Double-Edged Strategy
Parameterization — the process of identifying and exposing controllable variables of a system — is the most prevalent strategy for managing WHAT in generative practice. From the thesis: parameters "represent certain visual characteristics and their prominence" and a few can control many details. But the challenge is equally clear: parameters are often non-intuitive, representing abstract system internals rather than perceptual qualities. The gap between parameter space and design space is a persistent creative friction. The artist must develop fluency in a language that is not visual.

### Slide 4 — Remapping: Translating WHAT into Something Navigable
The response to non-intuitive parameters is remapping: translating abstract system variables into content that corresponds more closely to a visual or spatial intuition. From the thesis: control textures, procedurally generated fields, and hierarchically grouped parameter bundles all serve this function. From Gieseke et al.: image-based control maps pixel data (brightness, hue, gradient) to system behaviors, providing "transparent control for filling a space." WHAT the artist gives is redesigned to fit the artist's actual mode of thinking. This is not just UX work — it is aesthetic work. Note the connection to Gieseke et al.'s Navigation dimension: the size and legibility of the navigable space is partly a function of how WHAT is structured.

### Slide 5 — WHAT Determines What Is Sayable
The content level at which an artist interacts with a system determines the expressive vocabulary available. If WHAT is only numeric parameters, the artist can say precise but abstract things. If WHAT includes sketches, images, and spatial structures, the artist can say embodied and relational things. The thesis frames this as the challenge of "meaningful interface metaphors": finding a representational language for input that carries creative intent without too much loss in translation. What the artist provides is the vocabulary. The system is the grammar. But vocabularies can be impoverished or rich.

---

## Section 6 — WHERE: The Spatial Scope of Control
**8 min, 4 slides**

### Slide 1 — What "Where" Means
Where asks: does a control act globally on the entire output, or locally on a specific region? In traditional media, the answer is almost always local and direct — a brushstroke affects exactly where it lands. In computational generative systems, the default is often the opposite: a single parameter value governs the entire canvas. WHERE is thus a design dimension that must be explicitly addressed. Gieseke et al. (2021) organize this as a spectrum from automatic/global to manual/local, with varying levels of spatial targeting available.

### Slide 2 — Global vs. Local Control
Global control: one decision shapes everything — scale, density, color shift applied uniformly. Local control: the artist can target specific regions, elements, or layers with different behaviors. Gieseke et al. identify several mechanisms for spatial targeting: curves and paths drawn on the canvas, masks (regions defined by shapes or images), and flow fields (directional controls that vary spatially). Visual: the same generative pattern with global parameter change on the left, region-specific mask-based control on the right — dramatically different expressive results.

### Slide 3 — The Global-to-Local Refinement Strategy
Thesis link: artists working with generative systems routinely adopt a global-to-local workflow. First establish the overall visual character through broad parameters; then progressively refine local details through more targeted controls. This is not a limitation but a strategy — it mirrors the way any skilled visual artist works, building structure before detail. What changes computationally is that this workflow must be architecturally planned in advance: local control must be built into the system before it can be used. WHERE is thus something that must be designed, not assumed. Connection to Gieseke et al.'s Variation dimension: the openness of the design space is partly determined by how spatially differentiated control can be.

### Slide 4 — Spatial Control as Authorial Instrument
The degree of spatial targeting available in a system shapes what kinds of compositions are possible. Systems with only global control can produce internally consistent but spatially homogeneous outputs. Systems with rich spatial targeting can produce differentiated, hierarchically organized, and locally responsive work. Gieseke et al. identify this as one of the key limitations of many current procedural systems: the "trade-off between global automation and local manual manufacturing" is rarely solved elegantly. WHERE you can act determines the compositional range of what you can make.

---

## Section 7 — WHEN: The Temporal Position of Control
**8 min, 4 slides**

### Slide 1 — What "When" Means
When asks: at what point in the creation process can the artist intervene? Before the system runs (initialization)? During execution (real-time interaction)? After the fact (curation, post-processing)? In traditional media, "when" is mostly synonymous with "now" — the artist acts in the immediate present. In computational generative systems, WHEN is a design variable: it can be structured, sequenced, or closed off entirely. Gieseke et al. (2021) explicitly include temporal stage as a classification axis for control mechanisms. Connection to Gieseke et al.'s Stimulation dimension: the density of feedback — how often the loop closes — directly shapes whether a workflow feels immersive or speculative.

### Slide 2 — The Iterative Creative Loop as a WHEN Architecture
From the thesis: the core creative process in generative practice is an iterative loop of conception, implementation, execution, perception/curation, and re-conceptualization. Every cycle through this loop is a WHEN — a moment at which control is available. The "liveness" of a system (Tanimoto) determines how tight this loop is: high-frequency feedback enables a conversational pace; low-frequency feedback forces speculative, non-dialogic authorship. WHEN is thus partly a question of system architecture and partly a question of tool design.

### Slide 3 — Statefulness, Feedback Loops, and Temporal Evolution
From the thesis Ch. 4: systems that maintain state across the draw-loop — accumulating, remembering, responding to prior states — introduce a form of temporal agency that is not reducible to any single moment of control. The artist sets initial conditions; the system evolves. Parameters may be animated, accumulated, or driven by external data. This creates a situation where WHEN is distributed across time: the artist acts at multiple points, and the system's own temporal behavior mediates between those interventions. History-keeping as a strategy: the ability to return to, compare, and branch from prior states is a temporal control mechanism that most Creative Coding tools underserve.

### Slide 4 — WHEN Shapes Authorial Presence
The temporal structure of control determines whether the artist is present as a continuous force or as an initiating architect who then withdraws. Systems with rich real-time WHEN afford ongoing dialogue; systems with locked initialization afford front-loaded intention-setting followed by observation. Neither is superior — they produce different aesthetic relationships between artist and work. But they must be chosen deliberately. The thesis frames this as the dialogic nature of the creative process: the artist is "in conversation" with the system, and WHEN defines the rhythm and density of that conversation.

---

## Section 8 — WHO: Agency, Authorship, and the Co-Agency Spectrum
**10 min, 5 slides**

### Slide 1 — The Question the Survey Cannot Answer
Gieseke et al. (2021) systematically map HOW, WHAT, WHERE, and WHEN — corresponding, at the system level, to Navigation, Transparency, Variation, and Stimulation as evaluative dimensions. But neither the taxonomy nor the CSI addresses the fifth question: who is in control? This is not an oversight — it is a boundary. WHO belongs to a different register of analysis: not algorithm design but agency theory. The thesis (Ch. 2) provides the framework. Opening provocation: if the system produces behavior the artist did not anticipate — who made that?

### Slide 2 — The Co-Agency Spectrum
From the thesis: creative work with generative systems is not a binary between the artist controlling the system and the system controlling itself. It is a spectrum — from fully artist-led (the system as obedient tool) to fully system-led (the artist as observer of autonomous behavior). At each position, distinct artist-system relationships emerge: Tool-Protagonist (direct execution), Delegate-Manager (conductor/project manager role), Collaborator (equal creative partner), Curator (responds to what the system produces). Visual: the co-agency spectrum diagram from the thesis. The key insight: working with generative systems is not about ceding control — it is about distributing it.

### Slide 3 — How Architectural Choices Position the WHO
The WHO question is not answered by intent alone — it is determined by architectural choices. From the thesis Ch. 4: introducing randomness shifts creative agency toward the system; rule-based systems with emergent behavior shift it further; agent-based systems can produce behavior that genuinely exceeds the artist's predictive capacity. The same system architecture that produces surprise also redistributes authorship. The thesis is explicit: "autonomy" describes operational independence; "agency" describes impact on the creative outcome. A system can be operationally autonomous but have low aesthetic agency — or vice versa.

### Slide 4 — Intention, Curation, and the Inalienability of the WHO
From the thesis: no matter how autonomous a generative system becomes, the artist retains what the thesis calls "artistic control" — the combination of intention (the conceptual framework that initializes and continuously shapes the process) and curation (the iterative act of selection and evaluation). These are the dimensions of WHO that cannot be delegated. Curation is convergent thinking — the creative complement to the system's divergent generation. Even when the artist cannot predict the output, they remain the entity that decides whether it matters. This is the irreducibly human component of the WHO.

### Slide 5 — WHO Determines Aesthetic Meaning
The distribution of WHO across artist and system is not just a question of authorship — it shapes the kind of meaning the work can carry. A work made by an artist exercising tight intentional control carries a different aesthetic quality than one shaped by emergent system behavior that the artist curates but cannot author. Neither is more valuable, but they are different. The thesis quotes Boden: "The autonomy in the intentional sense of the generative systems does not exist." But something else exists — a form of creative surprise that the artist creates the conditions for, without being able to produce directly. That gap is where generative aesthetics lives.

---

## Section 9 — Synthesis: Five Dimensions, One Design Space
**7 min, 3 slides**

### Slide 1 — The Five Dimensions Are Coupled
HOW, WHAT, WHERE, WHEN, and WHO are not independent variables. A decision about WHAT — introducing exemplar-based input instead of parametric control — changes HOW interaction works, WHERE it applies, and WHEN it is possible, and it redistributes WHO by reducing the artist's ability to specify and increasing the system's generative latitude. Any change in one dimension propagates. The design space is not flat — it is a high-dimensional configuration space in which every choice has consequences across all axes.

Note the relationship to the Gieseke et al. framework: Navigation, Transparency, Variation, and Stimulation are evaluative outcomes; HOW, WHAT, WHERE, WHEN, and WHO are the generative inputs to those outcomes. Configuring the five dimensions well is what produces a system that scores well on the four evaluative criteria — plus, now, a fifth: meaningful authorship.

### Slide 2 — The Same Five Questions Apply to Watercolor on Paper
Return to the opening image: watercolor on paper. Walk through all five dimensions. HOW: direct, on-canvas, embodied. WHAT: pigment, water ratio, pressure — low-abstraction, physical parameters. WHERE: wherever the brush lands, with bleed behavior that propagates outward. WHEN: continuous, real-time, non-reversible. WHO: fully artist-led, with the material as an agent of unpredictability (bleed, granulation, drying) that the artist works with but does not control. The point: digital generative systems do not introduce a new problem. They scale the same problem into a design space that must be explicitly and consciously architected.

### Slide 3 — Emergent Aesthetics as a Configured Outcome
The aesthetic qualities that emerge from a generative system — complexity, surprise, coherence, expression — are not accidental properties of the algorithm. They are functions of how the five dimensions are configured. A system with rich spatial targeting (WHERE), real-time feedback (WHEN), sketch-based input (HOW + WHAT), and a deliberately calibrated co-agency spectrum (WHO) will produce different aesthetic qualities than one with global parameters, deferred feedback, and full autonomy. Aesthetic quality is not a byproduct. It is the outcome of design decisions made across all five dimensions. This is what it means to be the author of a generative system.

---

## Section 10 — Closing: Authorship is a Configuration
**5 min, 2 slides**

### Slide 1 — The Practical Implication
If the five dimensions structure creative control, then designing a generative system means making explicit decisions about each of them. HOW will the artist interact? WHAT will they provide? WHERE will control act? WHEN in the process will it be available? WHO will hold agency at each stage? These are not interface questions or UX questions. They are authorial questions. The thesis frames this as the shift from artist-as-craftsperson to artist-as-system-architect. The system architect makes decisions that are not about individual outputs but about the entire class of outputs the system can produce.

### Slide 2 — The Open Question
Every generative system instantiates a theory of creative control — whether or not its maker has articulated it. The five dimensions are always configured; the question is whether they are configured deliberately. Closing provocation: when you next design a system, or teach a student to design one, ask not "does it work?" but: How does the artist act? What do they give? Where does it land? When can they intervene? And who, at the end, is responsible for what emerges?

---

## Source Notes

**Shneiderman, Ben. (2007).** "Creativity Support Tools: Accelerating Discovery and Innovation." *Communications of the ACM*, 50(12), 20–32.
Core contribution: foundational framing of Creativity Support Tools as a research agenda; emphasis on tool design as an enabler of creative discovery.

**Frich, Jonas, Biskjaer, Michael Mose, and Dalsgaard, Peter. (2018).** "Twenty Years of Creativity Research in Human-Computer Interaction: Current State and Future Directions." *Proceedings of DIS 2018*, ACM, 1235–1257.
Core contribution: meta-survey identifying the lack of definitional rigor and methodological consistency in HCI creativity research.

**Frich, Jonas, Vermeulen, Lindsay Macdonald, Remy, Christian, et al. (2019).** "Mapping the Landscape of Creativity Support Tools in HCI." *Proceedings of CHI 2019*, ACM, 1–1.
Core contribution: landscape survey of CST research; reinforces the call for clearer evaluation frameworks.

**Remy, Christian, Vermeulen, Lindsay Macdonald, Frich, Jonas, et al. (2020).** "Evaluating Creativity Support Tools in HCI Research." *Proceedings of DIS 2020*, ACM, 457–470.
Core contribution: critique of inconsistent evaluation methods for CSTs; establishes the distinction between user-perceived creativity and system-structural affordances.

**Cherry, Erin and Latulipe, Celine. (2014).** "Quantifying the Creativity Support of Digital Tools Through the Creativity Support Index." *ACM Transactions on Computer-Human Interaction*, 21(4), 21:1–21:25.
Core contribution: psychometric instrument for evaluating creativity support (CSI); six dimensions: exploration, expressiveness, immersion, enjoyment, results worth effort, collaboration. Operates at user-experience level, not system-architecture level.

**Weisberg, Robert. (2006).** *Creativity: Understanding Innovation in Problem Solving, Science, Invention, and the Arts.* Wiley.
Core contribution: definition of creative process as intentionally producing a novel product; novelty as surprise — a product the creator did not directly anticipate.

**Boden, Margaret A. (2010).** *Creativity and Art: Three Roads to Surprise.* Oxford University Press.
Core contribution: framework of creative surprise; argument that autonomy in the intentional sense does not exist in generative systems.

**Gieseke, L., Asente, P., Měch, R., Benes, B., Fuchs, M. (2021).** "A Survey of Control Mechanisms for Creative Pattern Generation." *Computer Graphics Forum*, 40(2), 585–609. DOI: 10.1111/cgf.142658.
Core contribution: the HOW/WHAT/WHERE/WHEN taxonomy of control mechanisms; on-canvas vs. separate UI; global-to-local spectrum; input mode categories (exemplars, parameterization, handling, filling, guiding, placing); creativity dimensions (navigation, transparency, variation, stimulation).

**[Author]. (2024).** Master's Thesis: *Balancing Creative Intention and Systemic Autonomy* [Film University Babelsberg Konrad Wolf].
Core contribution: the WHO dimension — co-agency spectrum, artistic control (intention + curation), artist-system relationships (Tool-Protagonist through Curator), autonomy vs. agency distinction; operational strategies (parameterization, remapping, reuse, history-keeping); architectural mechanisms (order/chaos, randomness, statefulness, rule-based and agent-based systems); analytical three-layer framework.

---

## Timing

| Section                                    | Duration    |
| ------------------------------------------ | ----------- |
| 1. Opening                                 | 5 min       |
| 2. The Problem of Defining Creative Usability | 6 min    |
| 3. Existing Frameworks — And What They Leave Open | 8 min |
| 4. HOW                                     | 10 min      |
| 5. WHAT                                    | 10 min      |
| 6. WHERE                                   | 8 min       |
| 7. WHEN                                    | 8 min       |
| 8. WHO                                     | 10 min      |
| 9. Synthesis                               | 7 min       |
| 10. Closing                                | 5 min       |
| **Total**                                  | **~77 min** |

*Note: HOW and WHAT can each be trimmed by 2 min if needed. Sections 2 and 3 can be merged and compressed to ~8 min combined, bringing total to ~65 min.*
