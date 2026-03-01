name: inverse
layout: true
class: center, middle, inverse
---

<!-- https://conferences.eg.org/eg2021/for-submitters/video-submission/ 

Fast Forward: 20-26s
STARs: 70-75 min



-->


### State Of The Art Report

# A Survey of Control Mechanisms for Creative Pattern Generation


Lena Gieseke - Film University Babelsberg Konrad Wolf  
Paul Asente - Adobe Research  
Radomír Měch - Adobe Research  
Bedrich Benes - Purdue University  
Martin Fuchs - Hochschule der Medien  
  
#   

.center[<img src="../img/logos.png" alt="logos" style="width:100%;">]

???
.task[COMMENT:]  

* For giving you some insights on what motivated us for this work, lets first have a look at control mechanisms and creative pattern generation separately.
* So, we have "A survey of control mechanisms"

---
template:inverse

## Control Mechanisms

???
.task[COMMENT:]  

* In computer graphics we are striving to support artists with meaningful digital tools for content generation.
* Many of these techniques are described as...

---
layout: false

.header[A Survey of Control Mechanisms for Creative Pattern Generation]

## Control Mechanisms

--

> ...artist-usable!  
> ...creatively controllable!

--

We strive for a realistic discussion and towards defining such terms more objectively.

???
.task[COMMENT:]  

* Little attention, however, has been paid to overall creative workflows, which need to strike a balance, giving users needed power without burdening them with unwanted details. Often, techniques that are claimed to be artist-controllable turn out not to be so.

* Why are we doing what we are doing?

--

Rooted in the field of computer graphics, 

* we review relevant characteristics of underlying algorithms,

--

* motivated by an artist’s perspective.



???
.task[COMMENT:]  

* We include interface design aspects but they are not the focus of this survey

---
template:inverse

## Creative Pattern Generation


???
.task[COMMENT:]  


* So what makes pattern generation to creative pattern generations?

---
.header[A Survey of Control Mechanisms for Creative Pattern Generation]


## Creative Pattern Generation

.center[<img src="../img/examples_01.png" alt="examples_01" style="width:100%;">]

.small[
Left to right:  

* Manuscripts and Archives Division, The New York Public Library. 1450--1475. Historiated initial and another coat of arms.
* Owen Jones. 1867. Examples of Chinese ornament selected from objects in the South Kensington museum and other collections. London: S. & T. Gilbert. 
* The Miriam and Ira D. Wallach Division of Art, Prints and Photographs, The New York Public Library. 1882. Valentine cards utilizing decorative design, depicting flowers, hearts, butterflies and a tree. 
* Spencer Collection, The New York Public Library. 1910. Front doubleur. 
]


???
.task[COMMENT:]  

* France, China, USA, UK, Poland,

---
.header[A Survey of Control Mechanisms for Creative Pattern Generation]

## Creative Pattern Generation

.center[<img src="../img/examples_02.png" alt="examples_02" style="width:100%;">]

.small[
Left to right:  

* The Miriam and Ira D. Wallach Division of Art, Prints and Photographs, The New York Public Library. 1877. Arabesques : mosquée cathédrale de Qous : typan et écoinçons en faïence (XVIe. siècle). 
* William Morris. 1876. African Marigold Printed Textile. Planet Art CD of royalty-free PD images William Morris: Selected Works.
]

???
.task[COMMENT:]  

* Egypt, UK

---
.header[A Survey of Control Mechanisms for Creative Pattern Generation]

## Creative Pattern Generation

.center[<img src="../img/examples_03.png" alt="examples_03" style="width:100%;">]

.small[
Left to right:  
* Colourbox. 2011. Frame with roses. 
* Colourbox. 2013. Illustration of frame in Ukrainian folk style. 
* Izabela Rejke. 2011. Traditional Polish Folk Design. 
* Colourbox. 2013. Ornamental khokhloma oral postcard with seamless stripe.
]

---
.header[A Survey of Control Mechanisms for Creative Pattern Generation]

## A Complex Design Problem

.left-even[<img src="../img/examples.png" alt="examples" style="width:100%;">]

--

.right-even[
    
* Repetitive and balanced distribution of elements
* Hierarchical structures
* Space-specific designs
* Visual accents
]

---
.header[A Survey of Control Mechanisms for Creative Pattern Generation]

## A Representative Scenario 

--

.left-quarter[<img src="../img/spectrum.png" alt="spectrum" style="width:100%;">]

--

.right-quarter[

Balancing

* the efficiency and accuracy of computation, and
* the control and quality of manual creation.

]



???
.task[COMMENT:]  

* The repetitive nature of patterns is well-suited to algorithmic creation and automation, an artist needs more flexible control mechanisms for adaptable and inventive designs.

---

## A Survey of Control Mechanisms for Creative Pattern Generation

--

> What are the recent advances in 2D pattern generation?
  
--
  
* Focus on procedural models
  
--

> How can we describe a creation process from an artist's perspective?

--
  
* How can we classify control mechanisms?
  
--

> How can we discuss whether a technique is creatively controllable?




???
.task[COMMENT:]  


* Why should you listen?
* What will you gain from listing?

---

## A Survey of Control Mechanisms for Creative Pattern Generation

--

**1.** Theoretical Groundings

* Taxonomy 
    * Control Characteristics  
    * Control Mechanisms
* Means For Enabling Creativity

--
  
**2.** Analysis of the State of the Art

--

**3.** Discussion and Outlook


---
template:inverse

# Taxonomy

???

.task[COMMENT:]  

* The following taxonomy lays groundwork for our later evaluation of control mechanisms of the state of the art.
* It is difficult to derive the discussion of means for enabling creativity directly from the related work, as its authors have followed different motivations and have emphasized various aspects when describing their work and results.


---
template:inverse

Taxonomy

## How can we describe a creation process?

---

.header[Taxonomy]

## Control Characteristics


???
.task[COMMENT:]  

*  To classify the work in an objective and unified manner and to make it comparable, we analyze general characteristics of control with digital creation tools and then relate the actual presented control mechanisms to them

--

A creation process can be described by answering the questions of 

--

* *How*
* *What*
* *Where*
* *When*
* *Who*

---

.header[Taxonomy | Control Characteristics]

### How - User Interaction

> How is a control executed or an input given by an artist?

![how](img/how.png)

* File
* Separate UI
* On-Canvas

---

.header[Taxonomy | Control Characteristics]

### What - Content

> What does an artist give as input?

![what](img/what.png)

* Code
* Value
* Intermediate
* Element


---

.header[Taxonomy | Control Characteristics]

### Where - Canvas

> Where does the input have an effect and what is the area of influence?

![where](img/where.png)

---

.header[Taxonomy | Control Characteristics]

### When - Timeline

> When is the input given and at what time in the creation process is the control executed?

![when](img/when.png)


---

.header[Taxonomy | Control Characteristics]

### Who - User

> Who has the skill set needed to provide the input?

![who](img/who.png)


???
.task[COMMENT:]  

* This category can be in part derived from the above characteristics of how and what. 
*  The discussion of needed competencies, skills and mindsets, including the accompanying psychological and artistic aspects, is out of the scope of this survey

---

.header[Taxonomy]

## Control Characteristics

.center[<img src="../img/table3_01.png" alt="table3_01" style="width:100%;">]


---
template:inverse

Taxonomy

## How can we classify control mechanisms?

---

.header[Taxonomy]

## Control Mechanisms

* Descriptions of low-level mechanisms as given by the state of the art.  
* Define what an artist can or must work with.

---

.header[Taxonomy | Control Mechanisms]

.center[<img src="img/table3_01.png" alt="table3_01" style="width:55%;">]

---

.header[Taxonomy | Control Mechanisms]

.center[<img src="img/table3_02.png" alt="table3_02" style="width:55%;">]

---

.header[Taxonomy | Control Mechanisms]

.center[<img src="img/table3_03.png" alt="table3_03" style="width:55%;">]

---

.header[Taxonomy | Control Mechanisms]

.center[<img src="img/table3_04.png" alt="table3_04" style="width:55%;">]

---

.header[Taxonomy | Control Mechanisms]

.center[<img src="img/table3_05.png" alt="table3_05" style="width:55%;">]

---

.header[Taxonomy | Control Mechanisms]

.center[<img src="img/table3_06.png" alt="table3_06" style="width:55%;">]

---

.header[Taxonomy | Control Mechanisms]

.center[<img src="img/table3_07.png" alt="table3_07" style="width:55%;">]

---

.header[Taxonomy | Control Mechanisms]

.center[<img src="img/table3_08.png" alt="table3_08" style="width:55%;">]


---

.header[Taxonomy | Control Mechanisms]

.center[<img src="img/table3.png" alt="table3" style="width:55%;">]



---

.header[Taxonomy]

## Control Mechanisms

.center[<img src="img/table1_preview_01.png" alt="table1_preview_01" style="width:100%;">]

---

.header[Taxonomy]

## Control Mechanisms

<img src="img/table3_complete.png" alt="table3_complete" style="width:35%;">
<img src="img/table1.png" alt="table1" style="width:40%;">
<img src="img/table2.png" alt="table2" style="width:22%;">


---
template:inverse

## How can we discuss whether a technique is creatively controllable?

---

## Means For Enabling Creativity


Creativity is

* ill-defined, and
* involves insights from various disciplines,
 
making is notoriously difficult topic to address.

<!-- ---
.header[Means For Enabling Creativity]

## HCI

--

.caps[Shneiderman, Ben]. **Creativity Support Tools: Accelerating Discovery and Innovation**. *Communications of the ACM* 50.12 (2007), 20–32

--

* .caps[Frich, Jonas, Mose Biskjaer, Michael, and Dalsgaard, Peter]. **Twenty Years of Creativity Research in Human- Computer Interaction: Current State and Future Directions**. Proceedings of the 2018 Designing Interactive Systems Conference. ACM, 2018, 1235–1257
* .caps[Frich, Jonas, Macdonald Vermeulen, Lindsay, Remy, Christian, et al.] **Mapping the Landscape of Creativity Support Tools in HCI**. Proceedings of the 2019 CHI Conference on Human Factors in Computing Systems. ACM, 2019, 1–1
* .caps[Remy, Christian, Macdonald Vermeulen, Lindsay, Frich, Jonas, et al.] **Evaluating Creativity Support Tools in HCI Research**. Proceedings of the 2020 ACM Designing Interactive Systems Conference. ACM, 2020, 457–47

--

>  ...asking for more rigorous evaluation in regard to claimed creativity support.  
> ...clearer definitions of creativity. -->


---
.header[Means For Enabling Creativity]

## Creativity Support Index (CSI)

.caps[Cherry, Erin and Latulipe, Celine]. **Quantifying the Creativity Support of Digital Tools Through the Creativity Support Index**. *ACM Transactions on Computer-Human Interaction* 21.4 (2014), 21:1– 21:25 

--

* Measures how well a tool enables creativity based on a psychometric survey
* *Exploration*, *expressiveness*, *immersion*, *enjoyment*, *results worth effort*, *collaboration*
  
  
--
  
We are looking for

* an evaluation on an algorithmic level,
* as a subset of a more general and user-study-based classification.


---
.header[Means For Enabling Creativity]

## Discussion Basis

.caps[Weisberg, Robert]. **Creativity: Understanding Innovation in Problem Solving, Science, Invention, and the Arts**. *Wiley*, 2006  

.caps[Boden, Margaret A.]. **Creativity and Art: Three Roads to Surprise**. Oxford University Press, 2010  

--

A creative process

> ...intentionally produces a novel product.  

--

Novelty 

> ...as a surprising product, one that the creator did not directly anticipate.

<!-- ---
.header[Means For Enabling Creativity]

## Discussion Basis

 * The general controllability necessary for navigating a design space

> There are many different roads in the landscape.
 
* Transparency of that navigation and the understanding of cause and effect when using the tool

> I have the map to the landscape and know how to get from one point to another. 

* Navigation
* Transparency
* Variation
* Stimulation 

-->


---
.header[Means For Enabling Creativity]

## Navigation

Navigation describes both whether a creation processes is efficiently manageable and the extent of the controllability.

* Interactive
* Number of Controls
* Navigation History

---
.header[Means For Enabling Creativity]

## Transparency

Transparency describes how clear the understanding of cause and effect within the system is.

* Control Domain
* Control Communication

---
.header[Means For Enabling Creativity]

## Variation

Variation indicates how visually different the results can be.

* Size of the Design Space
* Openness of the Design Space

---
.header[Means For Enabling Creativity]

## Stimulation

The means of stimulation indicate how well an artist can enter a pleasurable and stimulating workflow.

* Immersion
* Stimuli

---
.header[Means For Enabling Creativity]

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

<!-- /////////////////////////////////////////////////////////////////////////////////////////// ANALYSIS -->
<!-- /////////////////////////////////////////////////////////////////////////////////////////// ANALYSIS -->
<!-- /////////////////////////////////////////////////////////////////////////////////////////// ANALYSIS -->

---
template:inverse

# Analysis of the State of the Art

---

## Analysis of the State of the Art


* From the perspective of an artist
    * What they can create
    * Required configuration input
    * Performance times
  

* Taken from the authors’ descriptions

---
.header[Analysis of the State of the Art]

## Categorization by Design Features


???

.task[COMMENT:]  

* What they can create

--

* Distribution and repetition

<img src="img/design_features_01.png" alt="design_features_01" style="width:20%;">

.small[
* Loi, Hugo, Hurtut, Thomas, Vergne, Romain, and Thollot, Joelle. **Programmable 2D Arrangements for Element Texture Design**. *ACM Transactions on Graphics* 36.3 (2017), 27:1–27:17]

???

.task[COMMENT:]  

* Distribution and Repetition refers to an overall distribution of elements and usually results in a homogeneous pattern with a texture-like quality. 
* A careful composition of the repeating elements can be used to create a perception of balance and order.
* Compositions are not limited to the repetition of the same element, but different visual qualities such as size or saturation can create various relationships.

---
.header[Analysis of the State of the Art]

## Categorization by Design Features

* Distribution and repetition
* Frames and hierarchies

<img src="img/design_features_02.png" alt="design_features_02" style="width:30%;">

.small[
* Loi, Hugo, Hurtut, Thomas, Vergne, Romain, and Thollot, Joelle. **Programmable 2D Arrangements for Element Texture Design**. *ACM Transactions on Graphics* 36.3 (2017), 27:1–27:17
* Santoni, Christian And Pellacini, Fabio. **gTangle: A Grammar for the Procedural Generation of Tangle Patterns**. *ACM Transactions on Graphics* 35.6 (2016), 182:1–182:11
]

???

.task[COMMENT:]  

* Frames and Hierarchies form compositions that further structure a design by creating contrasts, e.g., foreground vs. background, and accentuating spatial relationships, e.g., framing.

---
.header[Analysis of the State of the Art]

## Categorization by Design Features

* Distribution and repetition
* Frames and hierarchies
* Curves and brushing

<img src="img/design_features_03.png" alt="design_features_03" style="width:55%;">

.small[
* Loi, Hugo, Hurtut, Thomas, Vergne, Romain, and Thollot, Joelle. **Programmable 2D Arrangements for Element Texture Design**. *ACM Transactions on Graphics* 36.3 (2017), 27:1–27:17
* Santoni, Christian And Pellacini, Fabio. **gTangle: A Grammar for the Procedural Generation of Tangle Patterns**. *ACM Transactions on Graphics* 35.6 (2016), 182:1–182:11
* Jacobs, Jennifer, Brandt, Joel R., Měch, Radomír, And Resnick, Mitchel. **Dynamic Brushes: Extending Manual Drawing Practices with Artist-Centric Programming Tools**. *Extended Abstracts of the CHI Conference on Human Factors in Computing Systems*. ACM, 2018, D316:1–D316:4
]

???

.task[COMMENT:]  

* Curves, Lines and Brushing refer to artist-defined curved elements, which are an essential design feature for many creative pattern designs. They can be used, for example, as a base element or frame or as a distinct visual element. Brushing usually gives an individual, hand-made quality to a pattern.

---
.header[Analysis of the State of the Art]

## Categorization by Design Features

* Distribution and repetition
* Frames and hierarchies
* Curves and brushing
* Connections, branches and directionality

<img src="img/design_features_04.png" alt="design_features_04" style="width:88%;">

.small[
* Loi, Hugo, Hurtut, Thomas, Vergne, Romain, and Thollot, Joelle. **Programmable 2D Arrangements for Element Texture Design**. *ACM Transactions on Graphics* 36.3 (2017), 27:1–27:17
* Santoni, Christian And Pellacini, Fabio. **gTangle: A Grammar for the Procedural Generation of Tangle Patterns**. *ACM Transactions on Graphics* 35.6 (2016), 182:1–182:11
* Jacobs, Jennifer, Brandt, Joel R., Měch, Radomír, And Resnick, Mitchel. **Dynamic Brushes: Extending Manual Drawing Practices with Artist-Centric Programming Tools**. *Extended Abstracts of the CHI Conference on Human Factors in Computing Systems*. ACM, 2018, D316:1–D316:4
* Guo, Jianwei, Jiang, Haiyong, Benes, Bedrich, et al. **Inverse Procedural Modeling of Branching Structures by Inferring L- Systems**. *ACM Transactions on Graphics* 39.5 (2020)
* Saputra, Reza Adhitya, Kaplan, Craig S., Asente, Paul, and Měch, Radomír. **FLOWPAK: Flow-based Ornamental Element Packing**. Proceedings of the Graphics Interface Conference. Canadian Human-Computer Communications Society, 2017, 8–15
]

???
.task[COMMENT:]  

* Connections, Branches and Directionality between base elements are often used to further emphasize frames and hierarchies. 
* These structures and directionality are also often used to elaborate and accentuate the form of the space they fill, e.g., by aligning to it, building an pattern-space relationship [ABS06].

---
.header[Analysis of the State of the Art]

## Categorization by Design Features

* Distribution and repetition
* Frames and hierarchies
* Curves and brushing
* Connections, branches and directionality
* Single accents

.center[<img src="img/design_features.png" alt="design_features" style="width:100%;">]

.small[
* Loi, Hugo, Hurtut, Thomas, Vergne, Romain, and Thollot, Joelle. **Programmable 2D Arrangements for Element Texture Design**. *ACM Transactions on Graphics* 36.3 (2017), 27:1–27:17
* Santoni, Christian And Pellacini, Fabio. **gTangle: A Grammar for the Procedural Generation of Tangle Patterns**. *ACM Transactions on Graphics* 35.6 (2016), 182:1–182:11
* Jacobs, Jennifer, Brandt, Joel R., Měch, Radomír, And Resnick, Mitchel. **Dynamic Brushes: Extending Manual Drawing Practices with Artist-Centric Programming Tools**. *Extended Abstracts of the CHI Conference on Human Factors in Computing Systems*. ACM, 2018, D316:1–D316:4
* Guo, Jianwei, Jiang, Haiyong, Benes, Bedrich, et al. **Inverse Procedural Modeling of Branching Structures by Inferring L- Systems**. *ACM Transactions on Graphics* 39.5 (2020)
* Saputra, Reza Adhitya, Kaplan, Craig S., Asente, Paul, and Měch, Radomír. **FLOWPAK: Flow-based Ornamental Element Packing**. Proceedings of the Graphics Interface Conference. Canadian Human-Computer Communications Society, 2017, 8–15
* Gieseke, Lena, Asente, Paul, Lu, Jingwan, and Fuchs, Martin. **Organized Order in Ornamentation**. *Proceedings of the Symposium on Computational Aesthetics*. ACM, 2017, 4:1–4:9
]

???
.task[COMMENT:]  

* Single Accents refer to visually dominant elements and structures that might not follow the underlying order of a pattern, breaking an otherwise homogeneous appearance. This design feature is based on the principle of contrasts and accents, which is crucial for the overall visual appeal of a creative pattern design [War96; WZS98; MOT99].

CHECK: Add historic examples and explain, if there is time.

--

* Control mechanisms are clustered for each design feature

---
template:inverse

Analysis of the State of the Art

## Distribution and Repetition

---

.header[Analysis of the State of the Art]

## Distribution and Repetition

* Stochastic Pattern
* Regular to Near-Regular Pattern
* Rule-based and Design-Specific Patterns
* Element Arrangements

---

.header[Analysis of the State of the Art | Distribution and Repetition]

### Stochastic Pattern

--

.center[<img src="img/galerne_2012_gne_noise.png" alt="galerne_2012_gne_noise" style="width:100%;">]

.caps[Galerne, Bruno, Lagae, Ares, Lefebvre, Sylvain, and Drettakis, George]. **Gabor Noise by Example**. *ACM Transactions on Graphics* 31.4 (2012), 73:1–73:9

---

.header[Analysis of the State of the Art | Distribution and Repetition]

### Stochastic Pattern

.center[<img src="img/table1_distribution_stochastic_01.png" alt="table1_distribution_stochastic_01" style="width:100%;">]

Cluster

* Example-Based


???
.task[COMMENT:]  

* GILET et al. [GD10] can create displacement map textures, with the parameter computation taking from one to three hours. With a given rough approximation of the geometry and a representative pattern patch in the input, even volumetric repre- sentations can be created from the exemplar.
* Workflow of our method. Using an example photograph (a), the user gives a coarse approximation of the geometry (b) and chooses a relevant zone for analysis.

---

.header[Analysis of the State of the Art | Distribution and Repetition]

### Stochastic Pattern

.center[
<video style="padding-top:10px; outline:none; width:80%;" controls>
  <source src="img/galerne_2012_gne_cut.mp4" type="video/mp4">
</video>
]  
  
.caps[Galerne, Bruno, Lagae, Ares, Lefebvre, Sylvain, and Drettakis, George]. **Gabor Noise by Example**. *ACM Transactions on Graphics* 31.4 (2012), 73:1–73:9

???
.task[COMMENT:]  

* GALERNE et al. [GLLD12] add an interactive visual editor for adjusting their Gabor noise to the example fitting, and take about two minutes per texture. Sets of Gaussians represent the power spectrum of the noise, which can be rotated, scaled, translated, and cloned. Due to the abstract visual nature of a power spectrum, its connection to the visual features of the noise is not directly intuitive for artists. Hence, the editor has a strong exploratory nature to it. However, as the editing itself is interactive and visually appealing, it is inviting to do so.


---

.header[Analysis of the State of the Art | Distribution and Repetition]

### Regular to Near-Regular Patterns

--

.center[<img src="img/gieseke_2014_ipp.png" alt="gieseke_2014_ipp" style="width:100%;">]

.caps[Gieseke, L., Koch, S., Hahn, J.-u., and Fuchs, M.] **Interactive Parameter Retrieval for Two-Tone Procedural Textures**. *Computer Graphics Forum* 33.4 (2014), 71–79

---

.header[Analysis of the State of the Art | Distribution and Repetition]

### Regular to Near-Regular Patterns

.center[<img src="img/table1_distribution_regnearreg_01.png" alt="table1_distribution_regnearreg_01" style="width:100%;">]


Cluster

* Example-Based
* Data-Driven

---

.header[Analysis of the State of the Art | Distribution and Repetition]

### Regular to Near-Regular Patterns

<video style="padding-top:10px; outline:none; width:100%;" controls>
  <source src="img/guehl_2020_stu_cut.mp4" type="video/mp4">
</video>

.caps[Guehl, Pascal, Allègre, Remi, Dischler, Jean- Michel, et al.] **Semi-Procedural Textures Using Point Process Texture Basis Functions**. *Computer Graphics Forum* (2020)

---

.header[Analysis of the State of the Art | Distribution and Repetition]

### Rule-Based and Design-Specific Patterns

.center[<img src="img/wong_1998_cgf.png" alt="wong_1998_cgf" style="width:80%;">]

.caps[Wong, Michael T., Zongker, Douglas E., and Salesin, David H.] **Computer-generated Floral Ornament**. *Proceedings of the Conference on Computer Graphics and Interactive Techniques*. ACM, 1998, 423–434

---

.header[Analysis of the State of the Art | Distribution and Repetition]

### Rule-Based and Design-Specific Patterns

.center[<img src="img/table1_distribution_rulebased_01.png" alt="table1_distribution_rulebased_01" style="width:100%;">]


Cluster

* Probabilistic Interference
* Fields
* Example-Based

---

.header[Analysis of the State of the Art | Distribution and Repetition]

### Rule-Based and Design-Specific Patterns

<video style="padding-top:10px; outline:none; width:100%;" controls>
  <source src="img/zehnder_2016_dso_cut.mp4" type="video/mp4">
</video>

.caps[Zehnder, Jonas, Coros, Stelian, and Thomaszewski, Bernhard.] **Designing Structurally-sound Ornamental Curve Networks**. *ACM Transactions on Graphics* 35.4 (2016), 99:1–99:10


---

.header[Analysis of the State of the Art | Distribution and Repetition]

### Element Arrangements

.center[<img src="img/saputra_2018_rde_preview.png" alt="saputra_2018_rde_preview" style="width:100%;">]

.caps[Saputra, Rezaadhitya, Kaplan, Craig S.,and Asente, Paul.] **RepulsionPak: Deformation-Driven Element Packing with Re- pulsion Forces**. *Proceedings of the 44th Graphics Interface Conference*. Canadian Human-Computer Communications Society (20180, 10–1

---

.header[Analysis of the State of the Art | Distribution and Repetition]

### Element Arrangements

.center[<img src="img/table1_distribution_elements_01.png" alt="table1_distribution_elements_01" style="width:100%;">]


Cluster

* Example-Based
* Fields
* Data-Driven

---

.header[Analysis of the State of the Art | Distribution and Repetition]

### Element Arrangements

.center[
<video style="padding-top:10px; outline:none; width:80%;" controls>
  <source src="img/ma_2011_det.mp4" type="video/mp4">
</video>
]

.caps[Ma, Chongyang, Wei, Li-yi, and Tong, Xin]. **Discrete Element Textures**. *ACM Transactions on Graphics* 30.4 (2011), 62:1– 62:10

---
template:inverse

Analysis of the State of the Art

## Frames and Hierarchies

---

.header[Analysis of the State of the Art]

## Frames and Hierarchies

.center[<img src="img/benes_2011_gpm_preview.png" alt="benes_2011_gpm_preview" style="width:55%;">]

.caps[Benes,b., Št’ava, O., Měch, R.,and Miller, G.] **Guided Procedural Modeling**. *Computer Graphics Forum* 30.2 (2011), 325– 334

---

.header[Analysis of the State of the Art]

## Frames and Hierarchies

.center[<img src="img/table1_frames_01.png" alt="table1_frames_01" style="width:100%;">]


Cluster

* Curves
* Shapes and Masks
* Curves, Shapes and Masks 

---

.header[Analysis of the State of the Art]

## Frames and Hierarchies

<video style="padding-top:10px; outline:none; width:100%;" controls>
  <source src="img/santoni_2016_ggp_cut.mp4" type="video/mp4">
</video>

.caps[Santoni, Christian And Pellacini, Fabio.] **gTangle: A Grammar for the Procedural Generation of Tangle Patterns**. *ACM Transactions on Graphics* 35.6 (2016), 182:1–182:11


---
template:inverse

Analysis of the State of the Art

## Curves and Brushing

---
.header[Analysis of the State of the Art]

## Curves and Brushing

.center[<img src="img/curves.png" alt="curves" style="width:100%;">]

1. .caps[Lu, Jingwan, Barnes, Connelly, Wan, Connie, et al.] **DecoBrush: Drawing Structured Decorative Patterns by Example**. *ACM Transactions on Graphics* 33.4 (2014), 90:1–90:9
2. .caps[Měch, Radomír and Miller, Gavin.] **The Deco framework for interactive procedural modeling**. *Journal of Computer Graphics Techniques* 1.1 (2012), 43–99.

---
.header[Analysis of the State of the Art]

## Curves and Brushing

.center[<img src="img/table1_curves_01.png" alt="table1_curves_01" style="width:100%;">]

Cluster

* Data-Driven

---
.header[Analysis of the State of the Art]

## Curves and Brushing

<video style="padding-top:10px; outline:none; width:100%;" controls>
  <source src="img/xing_2014_apr_cut.mp4" type="video/mp4">
</video>

.caps[Xing, Jun, Chen, Hsiang-ting, and Wei, Li-Yi.] **Auto- complete Painting Repetitions**. *ACM Transactions on Graphics* 33.6 (2014), 172:1–172:11

---
template:inverse

Analysis of the State of the Art

## Connections, Branches and Directionality

---
.header[Analysis of the State of the Art]

## Connections, Branches and Directionality

.center[<img src="img/guo_2020_ipm.png" alt="guo_2020_ipm" style="width:100%;">]

.caps[Guo, Jianwei, Jiang, Haiyong, Benes, Bedrich, et al.] **Inverse Procedural Modeling of Branching Structures by Inferring L- Systems**. *ACM Transactions on Graphics* 39.5 (2020)


---
.header[Analysis of the State of the Art]

## Connections, Branches and Directionality

.center[<img src="img/table1_connections_01.png" alt="table1_connections_01" style="width:100%;">]

Cluster

* Fields
* Example-based
* Data-Driven


---
.header[Analysis of the State of the Art]

## Connections, Branches and Directionality

.center[
<video style="padding-top:10px; outline:none; width:80%;" controls>
  <source src="img/gieseke_2017_ooo_cut.mp4" type="video/mp4">
</video>
]

.caps[Gieseke, Lena, Asente, Paul, Lu, Jingwan, and Fuchs, Martin.] **Organized Order in Ornamentation**. *Proceedings of the Symposium on Computational Aesthetics*. ACM, 2017, 4:1–4:9 


---
template:inverse

Analysis of the State of the Art

## Single Accents

---
.header[Analysis of the State of the Art]

## Single Accents

.center[<img src="img/gieseke_2017_ooo_preview.png" alt="gieseke_2017_ooo_preview" style="width:60%;">]

.caps[Gieseke, Lena, Asente, Paul, Lu, Jingwan, and Fuchs, Martin.] **Organized Order in Ornamentation**. *Proceedings of the Symposium on Computational Aesthetics*. ACM, 2017, 4:1–4:9 

---
.header[Analysis of the State of the Art]

## Single Accents

.center[<img src="img/table1_accents_01.png" alt="table1_accents_01" style="width:100%;">]

---
.header[Analysis of the State of the Art]

## Single Accents


<video style="padding-top:10px; outline:none; width:100%;" controls>
  <source src="img/guerrero_2016_pep_cut.mp4" type="video/mp4">
</video>

.caps[Guerrero, Paul, Bernstein, Gilbert, Li, Wilmot, and Mitra, Niloy J.] **PATEX: Exploring Pattern Variations**. *ACM Transactions on Graphics* 35.4 (2016), 48:1–48:13 


<!-- /////////////////////////////////////////////////////////////////////////////////////////// Summary -->

---
template:inverse

Analysis of the State of the Art

## Summary & Discussion


???

.task[COMMENT:]  

* We summarize the state of the art in various forms.

---
.header[Analysis of the State of the Art]

### Control Mechanisms in the State of the Art

.left-even[<img src="img/table1.png" alt="table1" style="width:100%;">]
.right-even[
]

???

.task[COMMENT:]  

* First we give an overview of recent techniques, sorted by design areas and visual features.


---
.header[Analysis of the State of the Art]

### Control Mechanisms in the State of the Art

.left-even[<img src="img/table1_path.png" alt="table1_path" style="width:100%;">]
.right-even[
* Uneven distribution
]

???

.task[COMMENT:]  

* It is a fairly uneven distribution, with two major groups...


---
.header[Analysis of the State of the Art]

### Control Mechanisms in the State of the Art

.left-even[<img src="img/table1_path.png" alt="table1_path" style="width:100%;">]
.right-even[
* Uneven distribution
    * Distribution and Repetition
    * Curves and Brushing
]

???

.task[COMMENT:]  

* Distribution and Repetition focuses on repetitive pattern designs and filling a space, usually automatically.
* Curves and Brushing, which lets artist manually create distinct but potentially unstructured designs.
* However, creative pattern designs, such as the historic and commercial patterns in Figure 1, are rarely uniform nor unstructured, so additional control is needed to let artists create structure and work with design rules. 


---
.header[Analysis of the State of the Art]

### Control Mechanisms in the State of the Art

.left-even[<img src="img/table1_path.png" alt="table1_path" style="width:100%;">]
.right-even[
* Uneven distribution
    * Distribution and Repetition
    * Curves and Brushing

<img src="img/examples_subgroup1.png" alt="examples_subgroup1" style="width:100%;">
]

???

.task[COMMENT:]  

* However, creative pattern designs, such as the historic and commercial patterns in Figure 1, are rarely uniform nor unstructured, so additional control is needed to let artists create structure and work with design rules. 

---
.header[Analysis of the State of the Art]

### Control Mechanisms in the State of the Art

.left-even[<img src="img/table1_path_02.png" alt="table1_path_02" style="width:100%;">]
.right-even[

* Uneven distribution
    * Distribution and Repetition
    * Curves and Brushing
* Combinations
    * Balance between automatization and manual creation
    * Understanding of the space being filled
    * Global planning
]

???

.task[COMMENT:]  

* The table categories of Frames and Hierarchies; Connections, Branches, and Directionality; and Single Accents include systems that attempt to address this need. 
* These include algorithms that have a greater understanding of the space being filled and offer global planning to the artist.




---
.header[Analysis of the State of the Art]

### Performance

.left-quarter[<img src="img/table2.png" alt="table2" style="width:88%;">]
.right-quarter[

|               |        |
|---------------|--------|
| Realtime:     | < 1s   |
| Interactive:  | < 10s  |
| Synchronous:  | < 1min |
| Asynchronous: | < 1h   |
| Offline:      | > 1h   |
]

???

.task[COMMENT:]  

* As the works discussed here come from a time frame spanning more than 20 years, older techniques can be expected to significantly outperform their original implementations on current platforms. Accordingly, we categorize them coarsely into realtime, interactive, synchronous, asynchronous, and offline to indicate how one would work with the proposed techniques, and how their original application may have been intended

---
.header[Analysis of the State of the Art]

### Prevalence of Control Mechanisms

.left-even[<img src="img/table3_complete.png" alt="table3_complete" style="width:100%;">]
.right-even[]

???

.task[COMMENT:]  

* In total, 50 publications are included (the discussed state of the art in Section 7). Please note that the total for each step (how, what, where, when) can exceed the total of that category because the cat- egory can be implemented in multiple ways.

---
.header[Analysis of the State of the Art]

### Prevalence of Control Mechanisms

.left-even[<img src="img/table3_complete.png" alt="table3_complete" style="width:100%;">]
.right-even[

* Global control through intermediate representations

]

???

.task[COMMENT:]  

* This shows that global control is most commonly enabled through intermediate representations, such as example images. At the other end of the spectrum, placing elements as part of the actual output is most often local and manual with little automation supporting the artist throughout the creation process


---
.header[Analysis of the State of the Art]

### Prevalence of Control Mechanisms

.left-even[<img src="img/table3_complete.png" alt="table3_complete" style="width:100%;">]
.right-even[

* Global control through intermediate representations
* Parameterization through File and Value

]

???

.task[COMMENT:]  

* The dominant control mechanisms in the Parameterization category, File and Value, both require abstracted input from an artist, such as a text value or the use of a slider.

---
.header[Analysis of the State of the Art]

### Prevalence of Control Mechanisms

.left-even[<img src="img/table3_complete.png" alt="table3_complete" style="width:100%;">]
.right-even[

* Global control through intermediate representations
* Parameterization through File and Value
* Curves and brushing on-canvas but only in a limited region

]

???

.task[COMMENT:]  

* Sketch-based controls move the interaction onto the canvas and can make small-scale adjustments. Spaces to fill, curves to follow, and masking areas are also usually done directly on the canvas, but only influence the output indirectly. Brush- ing creates the output directly on the canvas, but can only do so in a limited region depending on the brush size, unless used to brush intermediate control lines.

---
.header[Analysis of the State of the Art]

### Prevalence of Control Mechanisms

.left-even[<img src="img/table3_complete.png" alt="table3_complete" style="width:100%;">]
.right-even[

* Global control through intermediate representations
* Parameterization through File and Value
* Curves and brushing on-canvas but only in a limited region

Focus on one control type, leading to trade-offs.
]

???

.task[COMMENT:]  

* The classification underlines that a focus on one control type, as is often done in computer graphics research, leads to the common trade-off between global automation and local manual manufacturing.



---
template:inverse

Analysis of the State of the Art | Discussion

## Means for Enabling Creativity


---
.header[Analysis of the State of the Art]

## Means for Enabling Creativity

Discussion is clustered into the most common types of control

* Example-Based Control
* Shapes and Masks
* Fields
* Curves and Brushing
* Element Placement

---
.header[Analysis of the State of the Art | Means for Enabling Creativity]

## Example-Based Control

???


???

.task[COMMENT:]  

* Goal-oriented control
    * Predictable output as efficiently as possible
    * Design task becomes data-driven


--

* Navigation
    * Performance
    * Initialization requirements
* Transparency
    * Matching quality
* Variation
    * Size of the design space
    * Spatial Influence
* Stimuli

--

### Outlook

* Regions
* Layering

---
.header[Analysis of the State of the Art | Means for Enabling Creativity]

## Shapes and Masks

* Navigation
    * Performance
* Transparency
    * Often not predictable
* Variation
    * Global to regional control
* Stimuli
    * Editing of control guides

--

### Outlook

* Elastic curves, drag & drop
* Hierarchies

---
.header[Analysis of the State of the Art | Means for Enabling Creativity]

## Fields

* Navigation
    * Performance
* Transparency
    * Intuitive through a visual representation
    * On-canvas, abstracted
* Variation
    * Global to regional control
    * Directionality and alignments
* Stimuli
    * Balance of control and automatization

--

### Outlook

* Combination of automatic filling with manual control on-canvas
* Structures in combination with alignments

---
.header[Analysis of the State of the Art | Means for Enabling Creativity]

## Curves and Brushing

* Navigation  
    * Options might be separated   
    * Potentially tedious  
* Transparency  
    * Familiar  
    * Direct control over the final result  
    * On-canvas  
* Variation  
    * Anything is possible  
    * Potentially un-structured  
    * Missing distribution techniques 
* Stimuli  
    * Easy and direct usage

--

### Outlook

* Incorporation of procedural creation principles into a data-driven process

---
.header[Analysis of the State of the Art | Means for Enabling Creativity]

## Element Placement

* Navigation
* Transparency
    * Direct control over the final result  
    * On-canvas  
* Variation
    * Maintain underlying global structure
* Stimuli
    * Design variation options

--

### Outlook

* Incorporation of a data-driven process into procedural creation

---
template:inverse

# Outlook

---

.header[Outlook]

## Machine Learning

* Increasing performance
* Inverse procedural modeling
* Design variations and suggestions
* Support of a personal style

.caps[Ritchie, Daniel, Thomas, Anna, Hanrahan, Pat, and Goodman, Noah D.] **Neurally-guided Procedural Models: Amortized Inference for Procedural Graphics Programs Using Neural Networks**. *Proceedings of the International Conference on Neural Information Processing Systems*. Curran Associates Inc., 2016, 622–630  

.caps[Guo, Jianwei, Jiang, Haiyong, Benes, Bedrich, et al.] **Inverse Procedural Modeling of Branching Structures by Inferring L- Systems**. *ACM Transactions on Graphics* 39.5 (2020)  

.caps[Guerrero, Paul, Bernstein, Gilbert, Li, Wilmot, and Mitra, Niloy J.] **PATEX: Exploring Pattern Variations**. *ACM Transactions on Graphics* 35.4 (2016), 48:1–48:13

???

.task[COMMENT:]  

* increasing performance up to 10 times by integrating a neural network and sampling a learned constraint-satisfying ap- proximation. Reported performances are overall below 3 seconds.


---

.header[Outlook]

## Mixed-initiative Interfaces

> [...] put human and computer in a tight interactive loop where each suggests, produces, evaluates, modifies, and selects creative outputs in response to the other.

.caps[Deterding, Sebastian, Hook, Jonathan, Fiebrink, Rebecca, et al.] **Mixed-Initiative Creative Interfaces**. *Proceedings of the CHI Conference Extended Abstracts on Human Factors in Computing Systems* (2017), 628–635  

.caps[Heer, Jeffrey.] **Agency plus automation: Designing artificial intelligence into interactive systems**. *Proceedings of the National Academy of Sciences* 116.6 (2019), 1844–1850


???

.task[COMMENT:]  

*  To achieve this, AI enables computer agency, and novel interfaces enable collaboration between computers and human users. On the topic of agency and automation, HEER [Hee19] discusses three case studies and poses several open questions for further developments.

---

.header[Outlook]

## Collaboration

* Common tools are either fully browser-based, or are in some way connected to cloud-based storage of assets, settings and results
* Navigation is crucial
* Stimulating creativity

.caps[Talton, Jerry O., Gibson, Daniel, Yang, Lingfeng, et al.] **Exploratory Modeling with Collaborative Design Spaces**. *ACM Transactions on Graphics* 28.5 (2009), 1–10

.caps[Salvati, Gabriele, Santoni, Christian, Tibaldo, Valentina, and Pellacini, Fabio.] **MeshHisto: Collaborative Modeling by Sharing and Retargeting Editing Histories**. *ACM Transactions on Graphics* 34.6 (2015), 205:1–205:10

.caps[O’Leary, Jasper, Winnemöller, Holger, Li, Wilmot, et al.] **Charrette: Supporting In-Person Discussions Around Iterations in User Interface Design**. *Proceedings of the CHI Conference on Human Factors in Computing Systems*. ACM, (2018), 535:1–535:11


---
template:inverse

# Conclusion

---

# A Survey of Control Mechanisms for Creative Pattern Generation

> How to support artists in their work with meaningful control mechanism?

* Procedural models for computing repetitions and automatization
* Manual manufacturing for layouts and details

For more complete and meaningful solutions aspects of both data-driven and procedural techniques are needed and must be merged into a unified whole.   

For a creative workflow *navigation*, *transparency*, *variation* and *stimulation* must be considered.


???

.task[COMMENT:]  

* This is the basis for developing innovative tools that further the ability of artists to create and to cre- atively express themselves.


---
template:inverse

# Thanks

## ...to all authors of the state of the art!

#### ...to my co-authors!