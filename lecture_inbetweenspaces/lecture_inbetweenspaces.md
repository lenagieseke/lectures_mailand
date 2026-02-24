name: inverse
layout: true
class: center, middle, inverse
---


### From Gesture to Code to Space:
# Translational Media

<br />
### Prof. Dr. Lena Gieseke | l.gieseke@filmuniversitaet.de  

#### Film University Babelsberg KONRAD WOLF


???
* This talk examines computational pipelines that translate physical behaviour into algorithmic systems: for example, gesture into fields, architectural layouts into navigable graph structures, and performance movements into agent-based simulation logic. It explores how such translations shape aesthetics, interaction, and our understanding of space as both computational construct and experiential domain.

---

## Teaser Image "Gesture to Space"

---
## Teaser Image "Datamorphism"

---
layout:false
## Agenda

--
* Introduction

--
* Translations


???
2. Framing — What Do We Mean by Translation?

--
* Case *Gesture into Fields*


???
3. Example — Gesture into Fields
    * What is a Gesture?
    * The Capture Problem
    * Example, e.g., Body Paint (2009), Memo Akten
    * What the Field Has That the Gesture Doesn't
    * The Thinking Ocean (2024), Memo Akten & Katie Hofstadter
    * Transition Question

--
* Example *Architecture into Navigation*


???
4. Case 2 — Architectural Layout into Navigation Graphs
    * What is Architectural Space?
    * Space Syntax: The Translation Framework
    * What the Graph Has That the Building Doesn't
    * Million Dollar Blocks (2006), Laura Kurgan
    * The Façade-Tilted Bird's-Eye View


--
* Example *Data into TODO:Space*


???
5. Case 3 — Ecological Data into Navigable Space
    * A Different Kind of Source Domain
    * Julie Freeman, The Lake (2005)
    * What the Space Has That the Lake Doesn't
    * Marshmallow Laser Feast, In the Eyes of the Animal (2015)
    * Transition to Synthesis

--
* The Third Space


???
6. Synthesis —  The Properties of the Third Space (on the example of Datamorphism)
    * What Do These Three Cases Share?
    * Introducing Datamorphism
    * Three Properties of the Third Space
    * The Audience Is Already Inside
    * From Translation to World-Building


--
* World-Building, Not World-Copying



---
layout:false

## MA Creative Technologies



---
template:inverse

# Translation


???
* Going from where to where?
* This talk examines computational pipelines that translate the physical world into algorithmic systems
* I propose the perspective that we are not simply moving something across, but rather — in most cases — producing a third space that belongs fully to neither domain.

---
## From World to Algorithmic Space

* Source domain
    * TODO: Examples
* Translational Operation (incl. Hardware)
* Resulting domain
    -> Is what?

---
## What Do We Mean by Translation?


---

.center[<img src="./img/lavarand_01.jpg" alt="lavarand_01" style="width:32%;"> <img src="./img/lavarand_02.png" alt="lavarand_02" style="width:67%;">] .imgref[[Images: [By HaeB - Own work, CC BY-SA 4.0](https://commons.wikimedia.org/w/index.php?curid=116926170), [Martin J. Levy](https://blog.cloudflare.com/randomness-101-lavarand-in-production/)]]

.footnote[[Walmsley, Alexander. 2026. Live Stream.]]


???

* Consider what happens when we try to bring something from the real world into computation. 
* Take randomness as a first example. Random numbers play a key role in computational processes ranging from the generation of secure cryptographic keys to the random initialization of weights during AI network training. Yet computers cannot produce true randomness. They simulate it using deterministic algorithms — PRNGs — and that simulation is structurally different from the thing it mimics. It has period lengths, statistical biases, seeds. In other words, the move from real-world phenomenon to computational representation is not a neutral transfer. Something changes in the crossing.
* One response to this problem is to extract seeds from highly complex physical processes. True random number generators (TRNGs) draw on the latent entropy in chaotic physical phenomena: atmospheric noise, radioactive decay, or — perhaps most evocatively — lava lamps. In the San Francisco offices of the internet security firm Cloudflare, a wall of lava lamps is filmed around the clock, providing cryptographic keys for roughly 20% of the world's internet traffic. Known as Lavarand, the system translates frames from the live feed into numeric seeds for a PRNG. The lamps' chaotic fluid motion, combined with atmospheric and lighting conditions, makes the seeds practically impossible to predict algorithmically. Objects designed purely for human visual pleasure become, in this context, operational instruments for computation.





* https://blog.cloudflare.com/randomness-101-lavarand-in-production/
  
From Alex:  
Random numbers play a key part of computational processes from the generation of secure cryptographic keys to the random initialising of weights during the training of an AI network. While the generation of random numbers with a sufficient level of unpredictability using deterministic pseudo-random number generator (PRNG) is suitable for many purposes, increasingly true random number generators (TRNG), which make use of the latent entropy in chaotic physical processes like atmospheric noise (https://www.random.org/) or radioactive decay (https://www.fourmilab.ch/hotbits/), are used to generate random numbers that are practically impossible to predict using an algorithm. 

This distinction is particularly salient in the area of cryptography, which is involved in the study of securing communication across networks (Rivest, 1990). The security of the world’s internet traffic relies to a large extent on the ability to generate cryptographic keys with a degree of unpredictability high enough to make them difficult if not practically impossible to guess. In such cases, a PRNG is often initialised with a truly random seed in order to quickly and efficiently produce a random key. In the San Francisco offices of the internet security firm CloudFlare there is a wall of lava lamps filmed 24 hours a day in order to provide cryptographic keys for some 20% of the world’s internet traffic (Fig. 1). Known as the Lavarand, the idea is based on an original patent by the US company Silicon Graphics in 1996 (Noll *et al.,* 1996). Whenever a key is required, the CloudFlare systems translate a frame from the live feed into a numeric value that is then fed as a seed into a PRNG, generating the key (Leebow-Fieser, 2017). Due to the highly chaotic movement of the liquid in the lamps, as well as the atmospheric and lighting conditions that eventually become rendered as pixels in the image, the seeds are extremely difficult to predict. The images, despite their use of brightly coloured objects made for human entertainment, are made to be purely operational for the computational process of pseudo-random number generation.


---
## What Do We Mean by Translation?

--
Moving something from one domain into another:
  
--
* Image capture → Pixel value → Seed for Pseudo Random Number Generator (PRNG) → Pseudo Random Number


???
* And here is where it gets interesting: what emerges on the other side is not a failed copy. The simulation is a new kind of object — one that behaves like randomness under certain conditions, but operates according to its own internal logic. It is neither the original phenomenon nor a mere approximation of it. It is something third.

--
<br />
*In which domain are we now?*

--

> Translation as production of a third space.




???

Computational translation is typically framed as transfer (moving something from one domain into another), but this framing obscures what is actually happening. Introduce the alternative frame: translation as production of a third space. Lead over to examples


The integration question is worth thinking through carefully. Here is an honest assessment:
The domain/translation/third space structure for Lavarand

Source domain: chaotic physical phenomenon (fluid, light, heat)
Translation: camera → pixel values → hash function → PRNG seed
"Third space": pseudo-random number sequence

The third space is genuinely novel — it is neither the lava lamps nor true randomness. It has its own internal logic: period lengths, statistical distributions, seed dependency. And it has real-world consequences: it secures 20% of internet traffic. By your own three criteria it actually scores reasonably well: emergent structure (yes), generativity (yes, infinite), feedback potential (yes — it shapes cryptographic infrastructure globally).
But the third space is entirely operational, not experiential or inhabitable. Nobody lives in a PRNG sequence. This is categorically different from Body Paint, Superradiance, or The Lake, where the third space is a space you can be inside.
My recommendation: keep it, but reframe its function explicitly
Lavarand works perfectly as a conceptual on-ramp — it illustrates the translation structure with unusual clarity and surprise, before the artistic examples complicate it. The weakness is actually rhetorical rather than logical: if you present it as a case study on equal footing with the others, the third space claim feels thin. But if you frame it explicitly as the simplest possible example of the structure — translation produces something that belongs to neither domain — it earns its place. And the closing callback to the lava lamp wall lands well precisely because the audience has been carrying it the whole time.
The slide note already says this well: "The PRNG was never a failed copy of randomness — it was a new kind of object." That is the argument. Just make sure the introduction frames Lavarand as illustration, not as full case study.

---
## Lavarand

* Source domain: chaotic physical phenomenon (fluid, light, heat)
* Translation: camera → pixel values → hash function → PRNG seed
* "Third space": pseudo-random number sequence



---
template:inverse

### Example
# Gesture into Fields

---
## What is a Gesture?


???
* Anchoring the source domain
A brief phenomenological provocation: gesture is embodied, continuous, intentional, and unrepeatable. It carries weight, hesitation, momentum — properties that belong to a body in time.

---
## What is a Gesture?

.center[<img src="./img/dance_01.png" alt="dance_01" style="width:37%;"> <img src="./img/dance_02.jpg" alt="dance_02" style="width:21%;"> <img src="./img/hands_01.jpg" alt="hands_01" style="width:39%;">] .imgref[[Images: [Lucas, A. 2014. Breathe Life Into Your Ballet Performance | Dance Advantage. Accessed at illusionsofamisadventurer](https://illusionsofamisadventurer.wordpress.com/2014/04/10/expression-and-communication-through-dance/), [NYC Dance Project. Accessed at Creative Boom](https://www.creativeboom.com/inspiration/the-art-of-movement-breathtaking-photographs-of-incredible-dancers-in-motion/), [freepik](https://www.freepik.com/premium-photo/beautiful-sensitive-hands-concept_29662593.htm#from_element=cross_selling__photo)]]

---
## What is a Gesture?

<img src="./img/dance_01.png" alt="dance_01" style="width:16%;"> <img src="./img/dance_02.jpg" alt="dance_02" style="width:9%;"> <img src="./img/hands_01.jpg" alt="hands_01" style="width:17%;">  


> A movement usually of the body or limbs that expresses or emphasizes an idea, sentiment, or attitude 
[...]

.footnote[[[Merriam-Webster Dictionary: gesture](https://www.merriam-webster.com/dictionary/gesture)]]


???
-> raised his hand overhead in a gesture of triumph
* the use of motions of the limbs or body as a means of expression
* something said or done by way of formality or courtesy, as a symbol or token, or for its effect on the attitudes of others. 
-> a political gesture to draw popular support …— V. L. Parrington

--


*How to capture a gesture?*

.footnote[[[Merriam-Webster Dictionary: gesture](https://www.merriam-webster.com/dictionary/gesture)]]


???
-> raised his hand overhead in a gesture of triumph
* the use of motions of the limbs or body as a means of expression
* something said or done by way of formality or courtesy, as a symbol or token, or for its effect on the attitudes of others. 
-> a political gesture to draw popular support …— V. L. Parrington


---
## Body Capture Technologies



Marker-based
* Optical mocap (Vicon, OptiTrack)
* Inertial mocap (Xsens, Rokoko)


Markerless
* Depth sensors (LiDAR, structured light, e.g. Azure)
* Multi-camera volumetric
* Video-based pose estimation (ML-driven, MediaPipe, OpenPose)



???
Marker-based
* Optical mocap (Vicon, OptiTrack) — retroreflective markers + IR cameras
* Inertial mocap (Xsens, Rokoko) — IMU suits, no optical dependency

Markerless
* Depth sensors (LiDAR, structured light, ToF) — e.g. Azure Kinect
* Multi-camera volumetric capture — photogrammetric reconstruction, e.g. 4D Views
* Video-based pose estimation (MediaPipe, OpenPose) — single or multi-cam, ML-driven

---
## Body Capture Technologies

.center[<img src="./img/mocap_01.png" alt="mocap_01" style="width:86%;"> ] .imgref[[Images: [University of Eastern Finland, HUMEA lab](https://sites.uef.fi/humea/humea-laboratory/human-motion-and-performance-analysis/)]]

---
## Body Capture Technologies

.center[<img src="./img/mocap_02.png" alt="mocap_02" style="width:27%;">] .imgref[[Images: [IEEE Pulse, Decoding Dance](https://www.embs.org/pulse/articles/decoding-dance/)]]


---
## Body Shapes

.center[<img src="./img/mocap_02.png" alt="mocap_02" style="width:27%;"> <img src="./img/mocap_03.png" alt="mocap_03" style="width:28%;"> <img src="./img/mocap_04.png" alt="mocap_04" style="width:43%;">] .imgref[[Images: [IEEE Pulse, Decoding Dance](https://www.embs.org/pulse/articles/decoding-dance/), [Design Collector, Motion Capture Dance Performance for AICP Awards](https://designcollector.net/likes/motion-capture-dance-performance-for-aicp-awards)]]


---


.center[
 <video width="1060" controls>
  <source src="./img/majorlazer_01.mp4" type="video/mp4">
</video> 
]

.footnote[[Major Lazer – Light it Up (feat. Nyla & Fuse ODG)](https://www.youtube.com/watch?v=r2LpOUwca94)]


---
template:inverse
# A *Third* Space

---
## Body Paint

--

<img src="./img/infrared_01.png" alt="infrared_01" style="width:30%;">
???
* The translation in action
Akten's infrared camera does not record the body — it records movement. Speed, acceleration, curvature, and size of motion are extracted and fed into a fluid simulation, producing strokes, drips, spirals, and splashes on a projected canvas. Show the installation image alongside the output field. Crucially: the system does not see people at all, only movement. Anything moving — living or not — triggers the same response. The body has already been abstracted away.
--
 → <img src="./img/field_01.png" alt="field_01" style="width:30%;">
--
 → <img src="./img/bodypaint_02.jpg" alt="bodypaint_02" style="width:30%;">  
.imgref[[Images: [xinfrared](https://www.xinfrared.com/pl/blogs/blog/the-capabilities-and-limitations-of-thermal-camera?srsltid=AfmBOopnv_2JS-e1YbCx1qtqDB4wCziekN6YMK5WAq72denV_wbsOUeO), [numerical-tours](https://www.numerical-tours.com/matlab/graphics_5_fluids/), Memo Atken. 2009. [Body Paint](https://www.memo.tv/works/bodypaint/)]]

--
> What does the field offer (that the gesture doesn't)?


---
.center[<img src="./img/bodypaint_03.png" alt="mocap_02" style="width:90%;">] .imgref[[Image: [Creative Applications: Body Paint – Gestures and dance into evolving compositions](https://www.creativeapplications.net/project/body-paint-openframeworks/)]]




---

.center[
 <video width="1060" controls>
  <source src="./img/bodypaint_01.mp4" type="video/mp4">
</video> 
Memo Atken. 2009. Body Paint. [https://www.memo.tv/](https://www.memo.tv/works/bodypaint/)
]

???

* https://www.creativeapplications.net/project/body-paint-openframeworks/

The fluid field produced by Body Paint has viscosity, diffusion rates, attractor behavior, gradient flows — properties that are physically well-defined but were never properties of the original gesture. A side-by-side: gesture (embodied, singular, temporal) versus field (spatial, persistent, iterable, generative). Akten's own framing supports the argument directly: what matters is not the painting at the end, but the sensation of playing. The output has escaped the input. It is a new kind of object.


---
## The Third Space

<img src="./img/bodypaint_04.jpg" alt="bodypaint_04" style="width:50%;">  

> The joy of the movement, the sensation of play...



.footnote[[[Creative Applications: Body Paint – Gestures and dance into evolving compositions](https://www.creativeapplications.net/project/body-paint-openframeworks/)]]

???
* User-to-user interaction: throw paint, splash each other
* While the installation is suitable for a single user, when multiple users are present a new dynamic emerges between people. A user-to-user interaction is born when the audience start playing with each other through the installation, throwing virtual paint at each other, trying to splash their friends, working collaboratively to create shared artwork, or mischievously trying to vandalize others’ work.

---

## Body Paint

Source domains
* The moving body (infrared camera: speed, acceleration, curvature)
* Fluid dynamics simulation

--

Translation operation
* Motion signal → velocity vectors → fluid field parameters
* The system does not see bodies — only movement


???
* the translation is real-time and reactive, the third space is co-produced live.

--

The third space
* A living painterly space with its own viscosity, diffusion, and memory
* Neither the gesture nor the physics — a new aesthetic domain

???
* The body is already abstracted away at capture: anything moving triggers the same response.
* The field has properties the gesture never had: persistence, diffusion rates, attractor behavior.
* The third space talks back — multi-user dynamics emerge that were never choreographed.


---
## Body Capture Technologies


Neural
* Neural Radiance Fields (NeRF)
* Gaussian Splatting


???
 Neural
* Neural Radiance Fields (NeRF) for dynamic body reconstruction
* Gaussian Splatting for real-time volumetric representation
  
Emerging
* Radar-based (no camera, through walls)
* EEG/EMG — capturing intent before visible movement occurs

---
.center[
 <video width="1000" controls>
  <source src="./img/gaussiansplat_01.mp4" type="video/mp4">
</video> 
Masaki Mizuno. 2026. 3D Gaussian Splatting. [X](https://x.com/MIZNOM/status/2023421414163013995?ref_src=twsrc%5Etfw%7Ctwcamp%5Etweetembed%7Ctwterm%5E2023421414163013995%7Ctwgr%5E6f47b56b09a9834c7d8b448b38bcf38c16c0dcf0%7Ctwcon%5Es1_&ref_url=https%3A%2F%2F80.lv%2Farticles%2Fmagical-animation-with-afterimage-made-from-3d-gaussian-splatting)
]

---
## The Third Space

.center[<img src="./img/thirdspace_01.png" alt="thirdspace_01" style="width:66%;">] .imgref[[Image: Masaki Mizuno. 2026. 3D Gaussian Splatting. [X](https://x.com/MIZNOM/status/2023421414163013995?ref_src=twsrc%5Etfw%7Ctwcamp%5Etweetembed%7Ctwterm%5E2023421414163013995%7Ctwgr%5E6f47b56b09a9834c7d8b448b38bcf38c16c0dcf0%7Ctwcon%5Es1_&ref_url=https%3A%2F%2F80.lv%2Farticles%2Fmagical-animation-with-afterimage-made-from-3d-gaussian-splatting)]]

---

.center[
 <video width="1080" controls>
  <source src="./img/superradiance_01.mp4" type="video/mp4">
</video> 
Memo Akten and Katie Hofstadter, 2025. [Superradiance](https://superradiance.net/)
]


???
* NO AUDIO
* What could be the third space?

---
## Superradiance

Memo Akten and Katie Hofstadter, 2025:

> We know that we are deeply entangled within complex, interdependent networks and assemblages of life, composed of and embedded within expansive scales of intelligence, unfolding across multiple boundaries of self.
  


---
## Superradiance

Memo Akten and Katie Hofstadter, 2025:

> We know that **we are deeply entangled within complex, interdependent networks** and assemblages of life, composed of and embedded within expansive scales of intelligence, unfolding across multiple boundaries of self.
  
--
  
<br />
> It’s one thing to intellectually know this, but how can we feel it, in our bodies?


???
* https://www.roborantreview.com/reviews/superradiance-memo-akten-and-katie-hofstadter-gray-area
* You are only made of non-you elements.
* Memo Akten and Katie Hofstadter have produced something profound and rare: imagery none of us have ever seen before. Katie’s dancing body is the centerpiece of this work, which appropriately, we never see. Instead, her liquid movements materialize nebulae, plankton, trees, worms, and mushrooms that seamlessly blend into video backdrops of earth’s beauty. 
* Literalism can be the bane of good art, but in this case, it’s a literalism that most of us have forgotten and desperately need to restore.

---
## Superradiance

The following images are all from:
  
<br />
  
Memo Akten and Katie Hofstadter. 2025. Superradiance.  
https://superradiance.net/

---
<img src="./img/superradiance_01.jpg" alt="superradiance_01" style="width:100%;">

---
<img src="./img/superradiance_02.jpg" alt="superradiance_02" style="width:100%;">

---
<img src="./img/superradiance_03.jpg" alt="superradiance_03" style="width:100%;">

---
<img src="./img/superradiance_04.jpg" alt="superradiance_04" style="width:100%;">

---
<img src="./img/superradiance_05.jpg" alt="superradiance_05" style="width:100%;">

---
<img src="./img/superradiance_06.jpg" alt="superradiance_06" style="width:100%;">

---
<img src="./img/superradiance_07.jpg" alt="superradiance_07" style="width:100%;">

---
<img src="./img/superradiance_08.jpg" alt="superradiance_08" style="width:100%;">

---
<img src="./img/superradiance_09.jpg" alt="superradiance_09" style="width:100%;">


---
## The Making of Superradiance

* Script
* Choreography
* Simulation
* Generative AI: Chapter 1 - Embodied Simulation
* Generative AI: Chapter 2 - Embodied Earth

.footnote[[Memo Akten and Katie Hofstadter. 2025. Superradiance. https://superradiance.net/]]


---

.center[
 <video width="1080" controls>
  <source src="./img/superradiance_makingof_cutout_01.mp4" type="video/mp4">
</video> 
]

.footnote[[Memo Akten and Katie Hofstadter. 2025. Superradiance. https://superradiance.net/]]

---
## Superradiance

Source domains
* The dancing body
* Natural processes: waves, root growth, wind, tidal movement

--

Translation operation
* Body pose → ControlNet skeleton → diffusion latent space
* Natural imagery → IP-Adapter conditioning


???
* Superradiance it is authored and rendered, the third space is designed in advance. 

--

The third space
* Ecological entanglement made *felt*, not just known
* Neither the dance nor the footage but a new experiential domain

???
* The idea (entanglement) is not in either source domain. 
* It only emerges in the crossing
* The third space is not a copy of either domain (dancing, nature), it is a system with its own rules.

---
## Machine Hallucinations — Nature Dreams

Rafik Anadol, 2021

> A giant data sculpture displaying machine-generated, dynamic pigments of nature.

<br />

> [...] to commemorate the beauty of the earth we share.

---
## Machine Hallucinations — Nature Dreams

* Superradiance → the body steers the latent space
* Anadol → data IS the latent space, rendered as environment


???
* Then Anadol flips the input: instead of a body, the source is pure data — millions of images, climate records, neural signals — fed directly into ML models, and the latent space is rendered as architectural-scale visual space. The gesture disappears; data becomes the gesture.
* utilizes over 300 million publicly available photographs of nature collected between 2018- 2021 at Refik Anadol Studio
* used to train a GAN AI algorithm
* The resulting AI Data Painting incorporates pigments, shapes, and patterns that we associate with nature, but only exist in the mind of a machine as dreams. 

---
## Nature Dreams

* Data collection
    * 300 million publicly available nature photographs of flowers, trees, mushrooms, landscapes, water, clouds, etc

.footnote[Refik Anadol. 2021. [Machine Hallucinations — Nature Dreams.](https://refikanadol.com/works/machine-hallucinations-nature-dreams/)]

---
<img src="./img/naturedreams_01.png" alt="naturedreams_01" style="width:98%;">

.footnote[Refik Anadol. 2021. [Machine Hallucinations — Nature Dreams.](https://refikanadol.com/works/machine-hallucinations-nature-dreams/)]

---
<img src="./img/naturedreams_02.png" alt="naturedreams_02" style="width:98%;">

.footnote[Refik Anadol. 2021. [Machine Hallucinations — Nature Dreams.](https://refikanadol.com/works/machine-hallucinations-nature-dreams/)]

---
<img src="./img/naturedreams_03.png" alt="naturedreams_03" style="width:98%;">

.footnote[Refik Anadol. 2021. [Machine Hallucinations — Nature Dreams.](https://refikanadol.com/works/machine-hallucinations-nature-dreams/)]

---
<img src="./img/naturedreams_04.png" alt="naturedreams_04" style="width:98%;">

.footnote[Refik Anadol. 2021. [Machine Hallucinations — Nature Dreams.](https://refikanadol.com/works/machine-hallucinations-nature-dreams/)]

---
<img src="./img/naturedreams_05.png" alt="naturedreams_05" style="width:98%;">

.footnote[Refik Anadol. 2021. [Machine Hallucinations — Nature Dreams.](https://refikanadol.com/works/machine-hallucinations-nature-dreams/)]

---
## Nature Dreams

* Data collection
    * 300 million publicly available nature photographs of flowers, trees, mushrooms, landscapes, water, clouds, etc

---
## Nature Dreams

* Feature extraction and filtering (ResNeXt)
    * A CNN architecture, producing a high-dimensional feature vector per image
    * Vectors encode semantic content
    * Xie, S., Girshick, R., Dollár, P., Tu, Z., and He, K. 2017. Aggregated Residual Transformations for Deep Neural Networks. In Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition (CVPR), 1492–1500. https://doi.org/10.1109/CVPR.2017.634

---
## Nature Dreams

* Dimensionality reduction and spatial clustering (UMAP)
    * Projection of high-dimensional feature vectors into three-dimensional space using UMAP, preserving local and global structure of the data manifold, where proximity equals semantic similarity. 
    * McInnes, L., Healy, J., and Melville, J. 2018. UMAP: Uniform Manifold Approximation and Projection for Dimension Reduction. arXiv preprint arXiv:1802.03426. https://arxiv.org/abs/1802.03426

---
## Nature Dreams

* Generative synthesis (StyleGAN2-ADA)
    * Thematically clustered subsets train a StyleGAN2-ADA model, producing 1024-dimensional embeddings
    * A custom Latent Space Browser (developed since 2017) enables navigation and interpolation through the learned distribution
    * Sampled GAN outputs — color fields, forms, textures that exist nowhere outside the model — serve as Anadol's "data pigments"
    * These pigments feed a GPU-accelerated fluid dynamics solver (vvvv / Fuse library), where they become color and form attributes driving a particle simulation of up to 100 million elements
    * Karras, T., Aittala, M., Hellsten, J., Laine, S., Lehtinen, J., and Aila, T. 2020. Training Generative Adversarial Networks with Limited Data. In Advances in Neural Information Processing Systems (NeurIPS), Vol. 33, 12104–12114. https://arxiv.org/abs/2006.06676


.footnote[Refik Anadol. 2021. [Machine Hallucinations — Nature Dreams.](https://refikanadol.com/works/machine-hallucinations-nature-dreams/)]


???
The pipeline has four distinct stages:
1. Data collection — 300 million publicly available nature photographs gathered over three years. The scale matters: this is not a curated art dataset but a mass-scraped collective visual memory of how humans have photographed nature.
2. Feature extraction and filtering (ResNeXt) — Each image is passed through ResNeXt, a CNN architecture that extends ResNet via grouped convolutions, producing a high-dimensional feature vector per image. These vectors encode semantic content — not pixels, but learned representations of what the image means to the network. The vectors are then used to qualitatively filter the dataset, removing noise and semantic outliers. (Xie et al., 2017, CVPR)
3. Dimensionality reduction and spatial clustering (UMAP) — The feature vectors, still high-dimensional, are projected into three-dimensional space using UMAP, which preserves both local and global structure of the data manifold. The result is a navigable, real-time 3D "data universe" where proximity equals semantic similarity. This is the step where data becomes space. (McInnes et al., 2018, arXiv:1802.03426)
4. Generative synthesis (StyleGAN2-ADA) — Thematically clustered subsets train a StyleGAN2-ADA model. The ADA variant is specifically designed to prevent discriminator overfitting on smaller training sets — relevant because thematic clusters, despite originating from 300M images, are relatively small after filtering. A latent space browser then allows navigation and interpolation through the learned distribution. (Karras et al., 2020, NeurIPS)
The quantum computing layer mentioned in the project description is not documented with sufficient technical specificity to be cited reliably — best left aside.

This two-stage synthesis is the crucial technical detail for your talk: the GAN is not the final output layer but a material generator feeding a separate spatial simulation system. The translation chain is longer than it appears — and the final aesthetic space is the product of at least two distinct computational domains in dialogue.:

5. Latent space navigation (custom software) — The studio has developed a proprietary Latent Space Browser since 2017. This tool allows navigation and interpolation through the trained GAN's latent space, extracting sequences of generated images — what Anadol calls "data pigments": color fields, forms, and textures that exist only in the model's learned distribution. The output here is not a finished image but a stream of generative material.
6. Fluid particle simulation (vvvv / Fuse) — The data pigments are fed into a GPU-accelerated fluid dynamics solver implemented in vvvv, a visual programming environment developed by the German developer collective, using their Fuse library for GPU computation. The StyleGAN outputs become color and form attributes assigned to particles in a fluid simulation — essentially the GAN paints the fluid. The Fluid Dreams variant at MoMA used approximately 100 million particles with real-time ray-traced lighting. Notably, at that scale the simulation cannot run in real time and must be pre-rendered — even on Anadol's custom-built computing infrastructure.



* Data collection
    * 300 million publicly available nature photographs of flowers, trees, mushrooms, landscapes, water, clouds, etc
* Classification: Complied dataset is fed into an image recognition algorithm, ResNext, for feature vectorization. Those computed features are then to qualitativly filter the dataset.
* Image Cluster: The UML-UMAP algorithm is used in a real time explorable, and three-dimensional data universe with a custom software.
* Style Gan2, with adaptive descriptor augmentation (ADA) with a latent space browser

## Machine Hallucinations — Nature Dreams

Source domain
* 300,000,000 publicly available nature photographs (2018–2021)

--

Translation pipeline
* Feature extraction
* Dimensionality reduction
* Generative synthesis

--

The third space
* Very beautiful moving abstract imagery

> The translation is complete, but the space produced has no grammar of its own.



???
* No new logic, no emergent behavior the audience can inhabit, no feedback loop.
* Nature imagery that has never existed — latent pigments, shapes,  
  patterns distilled from 300M photographs into a navigable dream
* The dataset is not displayed — it is *metabolized*
* Important distinction from Superradiance: no body, no gesture. The data itself is the sole source domain.
* UMAP is the crucial step for your argument: it is where high-dimensional data *becomes space* — literally a spatial translation operation.
* "Data as pigment" — Anadol's own framing — rhymes deliberately with Body Paint.
* Anadol is useful precisely as a limit case: 
  he shows the translation operation with unusual clarity,
  then stops short.
* Body Paint: audience inside the system, co-producing the space
* Superradiance: viewer's body collapsed into the ecological argument
* Anadol: spectacular, but you watch it from the outside
* This sets up the question Datamorphism attempts to answer

## The Third Space

Oftentimes the idea of a thrid space based on data is enoguh.

We call this *Datamorphism*.


---
## Datamorphism

> How data properties and our understanding of data shape the form *and reception* of data artworks.
  

Analogous to anthropomorphism, but instead of projecting *human traits*, datamorphism projects *data values*:  
truth, universality, objectivity.


.footnote[[Huson, M. and Gieseke, L. 2025. Datamorphism: Data Art of the Other-Than-Human. xCoAx 2025.]]


???
* In related work, we proposed datamorphism to describe how data properties — their size, their mapping logic, and their meta-communication — actively shape both the form of a data-based representation and its reception by an audience. The concept was developed in the context of data art about other-than-human phenomena, but it applies directly here. The key insight: translation is never neutral. The codec is an argument. What you encode, how you map it, and what you make visible to the audience are all decisions that produce the third space — not merely describe it.

Four properties that shape datamorphic reception:

* **Dataset size** — scale produces the sublime; comprehension breaks down
* **Meta-communication** — the audience must *know* the work is data-based
* **Machine-generated data** — decoupled from human agency at the moment of capture
* **Data mapping** — the translation from formal data to aesthetic form

* The perceptual shift is the core claim: knowing an artwork is data-based changes how you receive it.
* "Belief at first sight" — Kosminsky et al. 2019 — data lend authority the work may not otherwise possess.
* Key distinction from visualization: datamorphism is about reception and artistic potential, not communicative efficiency.
* The limit case of Anadol now reads clearly: the pipeline is there, the scale is there, but the meta-communication is weak — the audience experiences spectacle, not data.

---
## Datamorphism

Four properties that shape datamorphic reception:

* **Dataset size** — scale produces the sublime; comprehension breaks down
* **Meta-communication** — the audience must *know* the work is data-based
* **Machine-generated data** — decoupled from human agency at the moment of capture
* **Data mapping** — the translation from formal data to aesthetic form

.footnote[[Huson, M. and Gieseke, L. 2025. Datamorphism: Data Art of the Other-Than-Human. xCoAx 2025.]]

---
## Three Properties of the Third Space 

1. Emergent structure
    * the third space has properties that were not present in the source and could not have been predicted from it alone. The fluid field has attractors; the navigation graph has centrality; the lake installation has harmonic emergence.

---
## Three Properties of the Third Space 

2. Generativity beyond the source
    * the third space produces outputs, events, or behaviors that exceed what the source could generate. The field produces movements no body made; the graph predicts flows the building cannot; the fish installation composes music no fish intended.

---
## Three Properties of the Third Space 

3. Feedback potential
    * the third space begins to shape behavior in the original domain. The navigation representation changes how pedestrians walk. The datamorphic artwork changes how audiences perceive the phenomenon it represents. The encoded space starts encoding us.

---
## From Translation to World-Building 

If the third space is real — if it has its own structure, generativity, and feedback effects — then the act of designing the pipeline is not a technical decision. It is an ontological one. The pipeline author decides what exists in the third space. This reframes the entire practice of computational translation: not as a means of representing the world, but as a means of producing new parts of it. One line to close the section and open the final movement: we have been building worlds. The question is whether we have been doing so deliberately.

Closing: World-Building, Not World-Copying

---
## From Translation to World-Building 

A single image: the Cloudflare lava lamp wall. The opening provocation revisited. The PRNG was never a failed copy of randomness — it was a new kind of object, built deliberately for a purpose, with its own internal logic and its own real-world effects. It secures 20% of the world's internet traffic. The third space it produces is consequential. The same is true, I want to propose, of every computational pipeline that translates physical behavior into algorithmic systems.

## The Take-Home

Computational translation is not world-copying. It is world-building.


???

Slide 3 — The Open Question Closing without resolution

If we accept that computational pipelines produce third spaces — spaces with emergent structure, generativity, and feedback potential — then every design decision in the pipeline carries authorial and ethical weight. Who decides what gets encoded? What is lost in the translation, and for whom? When the third space starts shaping behavior in the original domain, who is responsible?

## The Take-Home


If we are building worlds, what does that oblige us to?
