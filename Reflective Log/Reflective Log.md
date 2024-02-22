Science of Programming
Human Computer Interaction (HCI)
Biocomputing
Data Science
Game Engineering

Quality 30%
Analysis 30%
Interconnections 20%
Self-criticism 20%

Description - What did you learn?
Interpretation - What is most important/interesting/useful/relevant about the topic or concepts?
Interconnection - How is it similar to and different from others?
Outcome - What have you learned from this? What does this mean for your future?


Science of Programming
======================

Description
-----------

- How do we know a computer program is correct; correctness of a program
- Scientific paradigms, methodology, ontology, epistemology
- Forms of knowledge; a priori (from programme script), a posteriori (from programme process)
- Different paradigms see computer science as a branch of engineering, mathematics or empirical science? (link to biocomputing)
- Lots of talk on assertions; obtain a priori about a programme script
- Assertion = boolean statement that returns an error if false
- Assertions act as guards, or a pre-condition, start point
- Also act as a formal assumption, or a post-condition, end point
- Can have them as their own functions, def pre_(): return bool, then assert pre_()
- Data invariant, a condition that must always be met, can also be functions see above
- Abstraction, planning, importance of preparation - lecture was confusing but interesting
- "Abstraction is all we've got"

HCI
===

Description
-----------

- Designing usable interfaces to digital technology
- 'a discipline concerned with the design, evaluation and implementation of interactive computing systems for human use and with the study of the major phenomena surrounding them'
- multiple different definitions, this is just an example
- Multidisciplinary field; Social Sciences, Technical Systems, Applied areas (e.g. health sciences), Creative disciplines (e.g. graphic design)
- Frustrating nature of poor 'interaction design'
- Design of any digital product, service or application involves some computational and interactive elements and needs  to support a quality user experience (UX)
- Knowing what a user wants, how to design new interactive experiences, knowing the design is right
- Examples of UI designs and their evolution
- Human-Centered design lifecycle
- Identifying needs and establishing requirements for the user experience; who are the users, what do they want
- Produce alternative design solutions that meet those requirements; sketches and storyboards
- Build interactive versions of those designs; paper prototypes
- Iteratively testing and evaluating the designs and the user experience that they offer; expert testing, user testing
- Gathering data to do this; questionnaires, surveys, interviews, focus groups
- Shadowing - walking around, observing what they do, can be powerful but hard to do for large samples and tricky to record data

Biocomputing
============

Description
-----------

- No access to slides come back to this

Data Science
============

Description
-----------

- Data Scientist vs Data Engineer; science - machine learning, analytics, visualisation for easier human interpretation, often applied statistics, engineer - efficient data management at scale, both - big data analytics
- Spend most of their time cleaning and organising data; also deemed to be the least enjoyable part of data science
- Second most is collecting data sets, also the second least enjoyable part of data science according to the given graph
- High quality data is required for data science, needed for good AI, emphasises importance of data engineering
- Big data
- Machine Learning and associated algorithms; improved performance due to improved experience -> machine learning
- Classification, regression, denoising, very mathematical
- Two types of machine learning: supervised - map data to labels, classification and regression, unsupervised - data without labels, feature extraction, dimensionality reduction, clustering
- Overfitting and underfitting; aim to make training error small, make gap between train error and test error small; underfitting - model not able to obtain a low error value on training data set; overfitting - gap between training error and test error is too large
- Different shaped graphs can have the same summary data; make both calculations and graphs, never trust summary data alone

Game Engineering
================

Description
-----------

- Code that makes the game work = game engineer
- Lots of other roles required to successfully make a game, e.g. writers for storyline, textures and meshes by artists, etc.
- Engineers need to understand the wider context of the code they're writing
- Rendering engineer, Physics engineer, AI engineer
- PhD topic examples: GPU assisted machine learning for material deformation, load balancing for streamed gaming applications, machine learned synthesis of soft body physics, machine learned generation of character movements, serious gaming for mental health, gamification of school lessons
- Gameplay programming - taking game engine's features and turning them into a working game, scripting languages
- Engine programming - high-performance code, systems programming, providing services to the gameplay programming aspect, interacting with the GPU
- e.g. game engine doesn't have "pick this up for 100 points", but it has collision detection; the rest you have to do yourself
- Games are a real-time problem, code needs to run fast at high frame rates (60 minimum is ideal)
- But people want newer games to look better, meaning more shader effects, more AI and physics updates, more memory usage for assets, which all makes this a lot harder
- Multithreaded programming is tricky
- C#, Lua, JavaScript, custom language, C++ is THE language of the gaming industry
- Portfolio, completed project, interest are all requirements to get into the industry
- History of games, birth of AAA in 1990s, evolution of video games across time
- Game design process, no more graphics for games module