What Was Done and How

    A description of the work done at a high level, including descriptions of design, implementation, testing strategies as appropriate.
    A rationale for the approach taken and any decisions made, taking account of the wider context of contemporary topics in computing as appropriate.
    References, quotes and examples of existing research and practice relevant to the approach taken and the artefact produced.
    Should use diagrams, tables, images and code snippets with captions to appropriately support text.

Results and Evaluation

    A clear description of the final artefact.
    An evaluation of how well the artefact meets the task description. 

Conclusions

    A summary of the work done.
    Suggestions for future work.
    Personal reflection on how the project went.
    Evaluation and reflections should include positive and negative aspects.

References

    Full references for any quotes, figures, code or other external sources used.
    A standard and consistent format will full bibliographic data.
    Appropriate use of in-text citations.

Appendices (optional)

    Brief appendices may be included that contain additional material such as diagrams and tables.  

What Was Done and How

- Continuing from the practical, using the sample solution
- Adding tests as we go
- Hint decisions
- Cannot guess the same word twice
- Guesses have to be words
- Regex
- Check Comments
- Problems with getting the clues working because mixing up answer and guess

- create screen
- add a letter
- add outline
- implement typing
- implement letters showing across from each other
- implement backspace
- enter, moving to next line
- actual gameplay, enter does something
- implement hard mode button
- fix hard mode
- messages
- Tkinter window
- Doesn't refocus back to PyGame window
- either fix or add as improvement
- changed print_state to return instead of print
- changed a regex to an iteration; regex cares about order for yellow hints which is not wanted
- 'keyboard' for clue visibility
- add box_size argument to Letter class, smaller boxes for keyboard
- problem with assertion in terms of screen space, check for < 0 instead of < SPACE // 2 since the initialiser was adding it>
- swapped grey and dark grey
- hint button, could've made hint part of the game class to not need arguments, next time
- talk about the buttons always being just rectangles when defined, so the same method can be used to display the hint itself
- edited hint method to work, previously wasn't doing yellows correctly
- changed hint colour to yellow
- keyboard colours being overwritten when duplicate is grey, fixed now to check light grey first
- function to recall keyboard for when game restarts
- hint not perfect, based off previous guess and does not use already known yellow; perfect for hard mode

- "You could just stop there—if you know there’s a G in it somewhere, seeing that headline might help you place it without taking an extra guess." https://lifehacker.com/how-to-get-a-wordle-hint-without-spoiling-the-whole-thi-1849610779
- https://www.youtube.com/watch?v=mJ2hPj3kURg
- https://stackoverflow.com/questions/63395415/how-to-change-focus-to-pygame-window