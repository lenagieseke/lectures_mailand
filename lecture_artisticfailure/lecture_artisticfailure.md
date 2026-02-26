name: inverse
layout: true
class: center, middle, inverse
---


### Models of Misbehaviour
## Artistic Uses of Failure

<br />

### Prof. Dr. Lena Gieseke | l.gieseke@filmuniversitaet.de  

#### Film University Babelsberg KONRAD WOLF


???
* Rather than polishing away artefacts, creators often seek them. Drawing on procedural structures, geometric deformations, AI misalignments and temporal distortions, this talk shows how systems and algorithms can benefit from controlled instability. It explores the artistic value of computational “misbehaviour,” demonstrating how elements traditionally treated as flaws, such as glitches or hallucinations, become deliberate materials for expression. Situated at the intersection of art, generative modelling, and generative AI, the talk highlights how these dynamics enable compelling, reflective, and at times stunning audiovisual experiences.



---
layout:false

## Agenda

* The Optimization Trap
* A Genealogy: From Accident to Medium
* Choreographing Collapse
* Misalignment as Medium
* A Poetics of Malfunction

---
template: inverse

## The Optimization Trap

---

## What Computational Systems Are Built to Do

> prevent → pursue → detect → contain


* Sanitization and normalization: keep bad inputs from entering the system

???
* Input validation — anything unexpected is rejected or escaped
* Data cleaning pipelines — outliers removed, formats standardized
* Type systems — prevent "wrong" values from existing at compile time


--

* Optimize for a loss function: actively pursue a target


???
* Optimize for a loss function: lower error, higher accuracy
    * Spam filters minimizing false negatives (at the cost of nuance)
    * Recommendation engines maximizing click-through rate (at the cost of serendipity)
    * Compilers minimizing cycle count or memory footprint
    * Search ranking optimizing engagement signals (dwell time, clicks)
    * TCP congestion control minimizing packet loss

* Converge toward a correct output: iteratively collapse toward the solution

--

* Error correction and redundancy: detect and repair deviation mid-process

???
* Sorting algorithms — the target state is fully defined, deviation is failure
* Consensus protocols (Paxos, Raft) — nodes must converge to a single agreed value
* Gradient descent — iteratively collapses the solution space toward a minimum
* Monte Carlo methods — repeated sampling converges toward the true probability
* DNS propagation — a distributed system resolving toward a single source of truth


--

* Robustness and control systems: contain and neutralize misbehavior at runtime


???
* Try/catch blocks — anomalous behavior is caught and neutralized
* Circuit breakers in microservices — deviant nodes are isolated
* Watchdog timers — if a process misbehaves, it gets killed and restarted

--

> Any deviation from the system's defined envelope of acceptable behavior is failure.


???
* Every layer exists to suppress deviation

---
## Prompt: *Will Smith eating spaghetti*

.center[
 <video width="420" controls>
  <source src="./img/willsmith_02.webm.360p.webm" type="video/webm">
</video>  
  
2023, mixed tools
]


.footnote[[[Wikipedia - Will Smith eating spaghetti](https://en.wikipedia.org/wiki/File:Will_Smith_Eating_Spaghetti_Original.webm)]]


---
## Prompt: *Will Smith eating spaghetti*


.center[
 <video width="720" controls>
  <source src="./img/willsmith_01.webm.480p.vp9.webm" type="video/webm">
</video>  
  
May 2025, Google's Veo 3
]


.footnote[[[Wikipedia - Will Smith eating spaghetti](https://en.wikipedia.org/wiki/File:Will_Smith_eating_spaghetti_Google_Veo_3.webm)]]



---
## Generative AI


* Early GAN artifacts → patched
* Limb hallucinations → corrected
* Temporal inconsistency → smoothed out
* Each iteration: less noise, less accident

--

<br />

> The history of generative AI so far is a history of **eliminating the interesting parts**.


???

**Photorealism**
    * Failure = bug
    * Noise = artifact
    * Glitch = version to deprecate

**Neural Glitch**
    * Failure = texture
    * Noise = material
    * Glitch = the whole point


---
## What Do We Mean by "Interesting"?

.center[<img src="./img/normaldistribution_01.png" alt="normaldistribution_01" style="width:80%;">] .imgref[[Image: [scribbr](https://www.scribbr.com/statistics/normal-distribution/)]]



???


* **Statistically:** high-entropy output — the system went somewhere unexpected
* **Perceptually:** violations of learned priors that resist visual resolution
* **Semiotically:** meaning the system produced but was never asked to produce
* **Artistically:** productive ambiguity — output that refuses a single reading
  
In every case: **interesting is what escapes the optimization target**. 

* It lives in the residual — the gap between intended output and actual behavior.
* That gap is what every patch is designed to close.

---
## What Do We Mean by "Interesting"?


.left-even[
 <video width="560" controls>
  <source src="./img/willsmith_01.webm.480p.vp9.webm" type="video/webm">
</video>&nbsp;&nbsp;&nbsp;&nbsp;  
]
  
  
  
.right-even[
 <video width="320" controls>
  <source src="./img/willsmith_02.webm.360p.webm" type="video/webm">
</video>  
]

.footnote[[[Wikipedia - Will Smith eating spaghetti](https://en.wikipedia.org/wiki/Will_Smith_Eating_Spaghetti_test)]]


---

## What Do We Mean by "Interesting"?

???
* Which version are you more likely to remember?

--

> Error can be interesting and memorable.


???
* A perfectly correct output carries no surprise — and no information
* The outputs that circulate, stick, unsettle: they are almost always wrong about something
* "Interesting" and "error" are the same residual, named from opposite sides of the optimization target

Flip the definition: If interesting = what escapes the optimization target, and the optimization target is to eliminate error, then interesting and error are the same thing — just named from different vantage points. The engineer calls it a bug. The artist calls it material.
  
Correctness is forgettable; it's the malfunction that sticks. The Will Smith video didn't circulate because it was accurate.  
  

Invoke information theory directly: A perfectly predicted output carries zero surprise, therefore zero information in the Shannon sense. Error is literally where the information is.

----
Claude Shannon defined information mathematically as a function of probability: the less likely an event, the more information it carries when it occurs. Formally, the information content of an event is −log₂(p), where p is its probability.
If something is perfectly predicted (p = 1), then −log₂(1) = 0. It carries no information because it surprised nobody. A system outputting exactly what it was trained to output is, in this precise technical sense, saying nothing.
Error, by definition, is low-probability output — high surprise, therefore high information content. The glitch literally carries more bits than the correct answer.
Shannon developed this in the context of communication and signal transmission, where the goal was to distinguish signal from noise. The irony for your talk is that noise is informationally rich — it was just inconvenient for the telephone engineers.
----

  
Historical precedent: Noise, distortion, and artifact have been rehabilitated repeatedly — vinyl crackle, film grain, JPEG compression, lo-fi aesthetics. Each was first a defect, then a texture, then a genre. The pattern is consistent enough to suggest something structural.

--

* Statistically: the system went somewhere unexpected (high-entropy output)
* Semiotically: the system produced but was not asked to produce
* Perceptually: violations of the expected and learned priors
* Artistically: productive ambiguity and output that refuses a single reading


???
Semiotics is the study of signs and meaning-making. In a semiotic frame, every output is a sign — it points to something, carries meaning, communicates.
When a generative system hallucinates a sixth finger or produces an impossible shadow, it produces signs that were not encoded in the prompt — meaning that emerged from the system's internals rather than the author's intention. The system became, briefly, an autonomous meaning-maker.
This is interesting because it destabilizes authorship: if the output contains meaning nobody put there, who said it? That question is artistically productive and philosophically uncomfortable — which is precisely why semioticians like Roland Barthes (the death of the author) and Umberto Eco (the open work) are useful references here if you want to go deeper.


--

> The engineer files a bug report. The artist opens a new project.



???
What Artists Actually Want

* Not fidelity — **friction**
* Not convergence — **rupture**
* Not the output — the **behavior** of the system under duress


---
template:inverse

# A Genealogy: From Error to Medium

---

## Making Failure Visible

.center[<img src="./img/kintsugi_01.png" alt="kintsugi_01" style="width:80%;">] .imgref[[Images: [Photo by Riho Kitagawa on Unsplash](https://unsplash.com/photos/round-brown-and-white-ceramic-plate-JuDPjcutors)]]


???

* 15th-century Japanese practice: broken pottery repaired with gold lacquer
* The crack is not hidden — it is **featured**
* Failure becomes the object's most legible history
* Wabi-sabi: impermanence and imperfection as aesthetic category

> The repair is not a return to the original. It is an argument that the broken version is more interesting.

* **Raku firing** — rapid removal from kiln, unpredictable thermal shock determines surface

---

## Conditions for Accident


.center[<img src="./img/pollock_01.jpg" alt="pollock_01" style="width:80%;">] .imgref[[Image: [The Met Collection](https://www.metmuseum.org/art/collection/search/482447)]]



???


* **Pollock** — gravity, viscosity, and velocity replace the brush; the body sets conditions, chance executes
* **Bacon** — threw paint, used rags and friends' photographs; "accident" unlocked what intention blocked

> None of these artists produced the accident. They **engineered the conditions** under which it could occur.

    Title: Untitled
    Artist: Jackson Pollock (American, Cody, Wyoming 1912–1956 East Hampton, New York)
    Date: ca. 1948–49
    Medium: Dripped black ink and red enamel paint on paper
    Dimensions: 22 7/16 × 30 3/16 in. (57 × 76.7 cm)
    Classification: Drawings
    Credit Line: Gift of Lee Krasner Pollock, 1982
    Object Number: 1982.147.27
    Rights and Reproduction: © 2026 Pollock-Krasner Foundation / Artists Rights Society (ARS), New York
    Curatorial Department: Modern and Contemporary Art


---

## Artifacts and Residue

.center[<img src="./img/rodin_01.jpg" alt="rodin_01" style="width:40%;">  <img src="./img/rodin_03.jpg" alt="rodin_03" style="width:31%;">] .imgref[[Image: [The Musée Rodin](https://www.musee-rodin.fr/en/musee/collections/oeuvres/assemblage-mask-camille-claudel-and-left-hand-pierre-de-wissant)]]


???

* **Degas monotypes** — pressing, lifting, reworking a plate that resists repetition; each print is a residue
* **Rodin's seam lines** — left casting artifacts visible; the evidence of process becomes surface

> The work does not depict making. It *is* the making, frozen.

A woman’s face was a source of inspiration for Rodin. Based on an initial portrait made of the sitter’s features, the sculptor never thought twice about composing a new, symbolic work by adding another element, a helmet, for example, or a hand, as here.

The Mask of Camille Claudel, one of the first portraits Rodin executed of his young pupil and mistress, shows the scar-like marks left by the seam lines of the different pieces of the mould. The mask aesthetic, more than that of a head or bust, permits this focus on facial features, without the effects of hair or chest. The wide-open eyes and blank gaze however betray a feeling of distress that the addition of the colossal hand only accentuates.

This hand was borrowed from Pierre de Wissant, one of The Burghers of Calais. Whereas in The Hand of God, Rodin used the right hand, here he employed the more disturbing, threatening, left hand, completely out of proportion with the face.

---

## Designed Unpredictability

* Aleatoric music: some element of the composition is left to chance, 
* John Cage
    * I Ching: an ancient Chinese classic text as composition tool 
    * 4'33": absence of deliberate sound

.footnote[[[Wikipedia - Aleatoric music](https://en.wikipedia.org/wiki/Aleatoric_music), [Wikipedia - John Cage](https://en.wikipedia.org/wiki/John_Cage)]]


???

* The composer defines a **system**, not an output
* Result: every performance is a unique sample from an intended distribution of unpredictability

> The author becomes a systems architect. The accident becomes the product.

<!-- IMAGE: 4'33" score or Cage portrait via Wikimedia: 
     https://commons.wikimedia.org/wiki/File:John_Cage_(1988).jpg -->

---

## Glitches

.center[<img src="./img/glitch_01.png" alt="glitch_01" style="width:50%;"> .imgref[[Image: [Glitch Studies Manifesto](https://beyondresolution.info/Glitch-Studies-Manifesto)]]]

>  The dominant, continuing search for a noiseless channel has been – and will always be – no more than a regrettable, ill-fated dogma.


???

Into the Digital: Menkman's Glitch Studies Manifesto (2010)

* Rosa Menkman: glitch as rupture of the "perfect, clean, and error-free" transmission ideal
* Challenges the **noiseless channel dogma** — Shannon's ideal of lossless communication
* Glitch art does not simulate error — it **instrumentalises** actual system failure
* Compression artifacts, datamoshing, circuit bending: failure modes as vocabulary

> The glitch is not a metaphor for malfunction. It is malfunction, put to work.

---

## Glitches



## Structural Failure as Method: Beckett

> *"Ever tried. Ever failed. No matter.*
> *Try again. Fail again. Fail better."*
> — Worstward Ho, 1983

* Failure is not the obstacle to the work — it **is** the work
* Each attempt degrades deliberately: language contracts, syntax collapses
* The endpoint is not success but a more precise, more honest failure

> Beckett does not iterate toward correctness. He iterates toward a failure that cannot be further reduced.

<!-- IMAGE: portrait via Wikimedia: https://commons.wikimedia.org/wiki/File:Samuel_Beckett,_Pic,_1_.jpg -->


---
class: center, middle

## The Question Is Not Whether to Use Failure

## The Question Is Which Failure Modes to Invite






2. A Genealogy: From Accident to Medium
* Making failure visible: Kintsugi
* Designing conditions for accident: Raku, Pollock, Bacon
* Indexical trace: Degas monotypes, Rodin's seam lines
* Structural failure as method: Beckett's "Fail better"
* Designed unpredictability: Cage, aleatoric composition
* Into digital: Menkman's Glitch Studies Manifesto — the noiseless channel dogma
-> The question is which failure modes to invite


3. Choreographing Collapse
* The parameter at the edge of breakdown: Quayola, Jardins d'Été
* The limitation as expressive device: Memo Akten, Learning to See
-> The artist designs conditions; the system authors its own anomalies


4. Misalignment as Medium
* Corrupting weights deliberately: Klingemann, Neural Glitch
* input-level manipulation
* Speculative biology through misclassification: Crespo, Neural Zoo
* Queering normativity through breakdown: Elwes, Zizi
* Temporal incoherence as emerging aesthetic: Rainisto; the Will Smith video revisited
* Recursive degeneration: model collapse (Shumailov et al., 2024)
-> Failures also reveal what the optimization was hiding



5. Designing Against the Optimization
* The shadow paradigm: anti-ai manifesto meets Antagonistic AI (Cai et al.)
* Negative Prompting
* The Trojan horse: misbehaviour that corrupts models from within
* Random glitch is not art; chosen glitch is
-> Controlled instability requires authorial responsibility: framing, context, intent


6. A Poetics of Malfunction
* The artist as designer of conditions, not producer of outcomes
* The undesigned gap: where training data ends and the system reveals itself
-> Failure is not the absence of craft — it is a craft vocabulary unavailable to those asking the system to reproduce the world


---
template:inverse

## The End

# 💧 🌊 💦
