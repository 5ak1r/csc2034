2. What is the author's central purpose? Why have they written the paper, and what do they wish to communicate? Authors should include this information primarily in the abstract and introduction.

//abstract

- demonstrate ease of code by providing complete implementation
- works for both 2D and 3D, on standard pc hardware
- also talks about historical development of their algorithm, evolution from stable density solvers to fluid velocity simulation
//introduction
- provide immersion; fluid flows are everywhere
- ad-hoc methods already exist; fake effects, hard to animate
- use the physics of fluid flows to make them more accurate
- algorithms are stable unlike physically accurate solvers
- no progress made using these in the past as other things besides video games desparately need physical accuracy, e.g. stresses and drag on an airplane or bridge must be calculated precisely



3. Thinking more specifically about the introduction, what were the stated objectives of the research? 

- see above
- introducing the fluid simulation model, Navier-Stokes equations
- emphasise importance of visual dynamics
- development of algorithms that allow games to simulate fluid flows quickly but effectively

4. What methods were used to accomplish the objectives? This might include systematic recording of observations, analysis and evaluation of published research, assessment of theory, reporting on experience. This will depend on the type of paper and the field in which the research was done.

- Navier-Stokes equations
- Assessment of theory
- Describing how fluids work; intended outcome
- Follow historical development of the Navier-Stokes equations
- Develop algorithm for density moving through a fixed velocity field; realised it could be applied to compute the evolution of the velocity field as well
- Start with simpler solver (density) and then work up to the more difficult ones
- Explanations are all shown in two dimensions; extending to three dimensions is described as straightforward
- Grid structure, assuming each cell has constant velocity and density
- Gauss-Seidel relaxation to interatively invert a matrix
- Densities would be easy to solve if the density were modeled as a set of particles; trace the particles through the velocity field
- Better method: find the particles which over a single time step end up exactly at the grid cell's centers; linearly interpolating the density at their starting location from the four closest neighbours
- Two grids, one for previous time step and one that contains new values, trace the cell's center position backwards through the velocity field, linearly interpolate from the grid of previous density values and assign this value to the current grid cell
- Using this now complete density solver, velocity solver can be made using methods previously created for the density solver, since the two formulae are very similar
- Velocity needs to be mass preserving, project() method defined to do this in the last step
- Velocity field = sum of an incompressible (mass preserving) field and a gradient field - Hodge decomposition
- Computing the height field is equivalent to computing the gradient, rearrange hodge decomposition to obtain mass conserving field
- Computing the height field involves the solution of a Poisson equation, reuse Gauss-Seidel relaxation code to solve i
- Assumption that fluid is contained in a box with solid walls; horizontal component of the velocity should be zero on the vertical walls, while the vertical component of the velocity should be zero on the vertical walls; assume continuity

5. Review the results in light of the stated objectives. What were the results of the study? Does the study reveal what the researcher intended? What, if any, objective evidence was obtained from the author's eﬀorts (observations, measurements etc.)?  

- Successfully created a simple density and velocity solver; fluid dynamics solver using the Navier-Stokes equations
- Imperfect with lots of areas of modification and improvements, e.g. project() routine uses Gauss-Seidel relaxation but could use a conjugate gradient solver instead; better convergence properties (visual improvements are minor so it's deemed unnecessary)
- Current solver suffers from numerical dissipation - fluids dampen faster than they should in reality
- Other fluids done by other researchers but their algorithms tend to be a lot slower and not ideal for games
- Visual proof of effects modeled, animated and rendered within the animation system
- Visually compare to real flows

6. Check the interpretation against the results. How were the results interpreted? How were they related to the original problem (author's view of evidence rather than objective ﬁndings)? Does the interpretation arise logically from the data or is it too far-fetched? Have the faults/ﬂaws/shortcomings of the research been addressed?

- "Do the results they claim actually make sense"


7. Finally, it is important to establish whether the research has been successful – has it led to new questions being asked, new ways of using existing knowledge? How did other researchers view the signiﬁcance of the research reported by your authors? Are other researchers citing this paper? 

- Research cultivated in the MAYA Fluid Effects feature for the modeling and animation software MAYA. That one is more sophisticated and general but the core embodies the ideas presented in the paper



8. Provide a summary of the article, based on your understanding and the answers provided above. You should form an opinion about the strengths and weaknesses of the paper and include these in your summary. Also comment on the content and organisation. Making judgements about someone else's work is often the most diﬃcult part of writing the review, but is an important skill to learn and practice.   

it sucked :)


9. Provide a full reference for your selected paper in the Harvard style. The Referencing section of the Library's guide can help.
The reference would normally go in a list end of your document, and provide information about the source so that a reader can find the information themselves. Each reference would typically have one or more in-text citations, which appear in the main body of the document, indicating which reference was used for a given piece of information.  

- referencing