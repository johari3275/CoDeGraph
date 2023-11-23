# MC CoDe-Graph Improvement Ideas

Suggestion for improvement:
- Scaffolding as an element (e.g., moderator, prompt…)
- Badge element for finishing the course.
- Connecting arrows forward and backward (if student can move back as well; e.g, rewatching an instructional video)
- Locked and unlocked affordances symbols
- Assessment and feedback elements should be kept separately and connected with a line.
- Sequencing should be obvious to the viewer of a design.

### Design 1: MC CoDe-Graph traditional design (based on current model)
![image](https://github.com/johari3275/CoDeGraph/assets/111693027/4bd5df64-be87-4a86-8370-19481b4a8ae1)


Description:
- Badge element included
- Connecting arrows forward and backward included for learning materials (M1 – M3)
- Locked and unlocked affordances symbols visualized by outer layer of building block (e.g., M2-pretest or M3-post-test)
- Assessment and Feedback connected via line
- Sequencing obvious based on flow from left to right

Mermaid Syntaxt for Design 1:
```
flowchart LR

classDef orange fill:#ffa500
classDef yellow fill:#ffff00
classDef pink fill:#FFC0CB
classDef green fill: #00ff00
classDef turquoise fill: #4FF2E7
classDef purple fill: #ba55d3

A[[Final Test <br>Essay]]:::green --- Z>Course Completion <br> Badge]:::purple

B[[M3: Pre-Test]]:::orange --- BA((Feedback)):::pink -.Learner fails pre-test <br> moves to learning video.-> C([M3: Learning Video]):::yellow <--> CA([Scaffolding: <br> ChatBot Intervention]):::turquoise <--> D([M3: Steps Process]):::yellow <--> E([M3: Lifehacks]):::yellow <--> F[[M3:Post-Test]]:::orange

G[[M2: Pre-Test]]:::orange --- BG((Feedback)):::pink -.Learner fails pre-test <br> moves to learning video.-> H([M2: Learning Video]):::yellow <--> HA([Scaffolding: <br> Prompt with Tips]):::turquoise <--> I([M2: Flashcards]):::yellow <--> J([M2: Scenario]):::yellow <--> K[[M2:Post-Test]]:::orange

L(M1: Pre-Test):::orange --- BL((Feedback)):::pink -.Learner fails pre-test <br> moves to learning video.-> M([M1: Learning Video]):::yellow  <--> MA([Scaffolding: <br> Q&A with Moderator]):::turquoise <--> N([M1: Multitab]):::yellow <--> O([M1: Lifehacks]):::yellow <--> P[[M1: Post-Test]]:::orange

BL -.Learner succeeds in pre-test <br> moves to next pre-test.-> G
BG -.Learner succeeds in pre-test <br> moves to next pre-test.-> B
BA -.Learner succeeds in pre-test <br> moves to  final test.-> A
P -.Learner succeeds in post-test <br> moves to next pre-test <br> Learner fails in post-test <br> studies learning materials again <br> attempts post-test again until success.-> G
K -.Learner succeeds in post-test <br> moves to next pre-test <br> Learner fails in post-test <br> studies learning materials again <br> attempts post-test again until success.-> B
F -.Learner succeeds in post-test <br> moves to next pre-test <br> Learner fails in post-test <br> studies learning materials again <br> attempts post-test again until success.-> A

```

### Design 2: MC CoDe-Graph traditional design + Scaffolding block + ELO block
![image](https://github.com/johari3275/CoDeGraph/assets/111693027/8ab46821-da89-4b7a-9058-c0e605c7a1d0)


Description:
- Study Coordination course as a template
- Scaffolding blocks included with example text
- ELO block included (Essay replaced the final test)

Mermaid Syntaxt for Design 1:
```
classDef orange fill:#ffa500
classDef yellow fill:#ffff00
classDef pink fill:#FFC0CB
classDef green fill: #00ff00
classDef turquoise fill: #4FF2E7
classDef purple fill: #ba55d3,stroke:#333, stroke-width: 5px

A(Final Test <br>Essay):::green --- Z((Course Completion <br> Badge)):::purple

B(M3: Pre-Test):::orange --- BA{Feedback}:::pink -.Learner fails pre-test <br> moves to learning video.-> C[M3: Learning Video]:::yellow <--> CA(Scaffolding: <br> ChatBot Intervention):::turquoise <--> D(M3: Steps Process):::yellow <--> E(M3: Lifehacks):::yellow <--> F(M3:Post-Test):::orange

G[[M2: Pre-Test]]:::orange --- BG{Feedback}:::pink -.Learner fails pre-test <br> moves to learning video.-> H[M2: Learning Video]:::yellow <--> HA(Scaffolding: <br> Prompt with Tips):::turquoise <--> I(M2: Flashcards):::yellow <--> J(M2: Scenario):::yellow <--> K(M2:Post-Test):::orange

L(((M1: Pre-Test))):::orange --- BL{Feedback}:::pink -.Learner fails pre-test <br> moves to learning video.-> M(M1: Learning Video):::yellow  <--> MA(Scaffolding: <br> Q&A with Moderator):::turquoise <--> N(M1: Multitab):::yellow <--> O(M1: Lifehacks):::yellow <--> P(M1: Post-Test):::orange

BL -.Learner succeeds in pre-test <br> moves to next pre-test.-> G
BG -.Learner succeeds in pre-test <br> moves to next pre-test.-> B
BA -.Learner succeeds in pre-test <br> moves to  final test.-> A
P -.Learner succeeds in post-test <br> moves to next pre-test <br> Learner fails in post-test <br> studies learning materials again <br> attempts post-test again until success.-> G
K -.Learner succeeds in post-test <br> moves to next pre-test <br> Learner fails in post-test <br> studies learning materials again <br> attempts post-test again until success.-> B
F -.Learner succeeds in post-test <br> moves to next pre-test <br> Learner fails in post-test <br> studies learning materials again <br> attempts post-test again until success.-> A

```
### Design 3: MC CoDe-Graph BPMN 2.0 oriented
![image](https://github.com/johari3275/CoDeGraph/assets/111693027/9bb0b627-278f-4aaf-9e39-12b382e0b0c1)


- Shapes of objects oriented at BPMN 2.0
- Therefore, shape of elements based on the positioning and purpose in the flowchart instead of base shape (e.g., CoDe-Graph building blocks are always the same shape)
- Shape of objects identical besides:
  - Starting point: circle with a thin outer layer
  - Gateway (Branching): rhombus-shaped object (for feedback in this case)
  - End point: circle with thick outer layer


### Viewing the mermaid syntax

Option 1:
- Copy the above syntax
- Go to https://mermaid.live
- Paste in the code section and the diagram will be automatically generated (if there is no syntax error)

![image](https://github.com/johari3275/CoDeGraph/assets/111693027/a8d3fedc-d265-4108-9575-b06a9f5ecd09)

Option 2:
- Copy the above syntax
- Go to https://draw.io
- Go to Arrange option -> Insert -> Advanced -> mermaid

![image](https://github.com/johari3275/CoDeGraph/assets/111693027/c327e275-ddfe-4ad6-9234-2263e671bdc0)

