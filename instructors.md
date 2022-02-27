
## Teaching in class :information_desk_person: :speech_balloon:

## Tips for teaching

Here are some steps and guidelines when you are an **instructor**:

- Start by *introducing a bit about yourself* and perhaps why you're interested
in teaching R and data analysis.
- Keep mindful of the time and try to *stay on time*. The lead organizer will be
also be keeping track of time and wave to you to continue on or slow down.
- Try to assume the participants *know as little as possible*. This is actually
quite hard, but try as best you can. The lead organizer may take notes and
provide feedback after your lesson or clarify concepts to the participants. Try
to (briefly) explain as much aspects as possible of what you are doing,
including how to open RStudio or how to run code (e.g. press `Shift-Enter` in RStudio).
- **Check in with participants**: We distribute colored sticky notes to each
participant so that they can flag problems with one color and success with
another color. Use these indicators to check your pacing and where the
class is at.
    - Check in with the learners to see where they are at by saying something like:
    "Do you see the same thing as is on the screen? 
    If yes, put the 'all good' sticky on your laptop. 
    If no, use the 'need help' sticky."
    - For the reading activities, before starting, say:
    "Please read this section as instructed. 
    When you are done, put the 'all good' sticky up."
    - For exercises, before starting, say:
    "Please complete the exercise. When you are done,
    please put the 'all good' sticky up.
    If you need help, put the 'need help' sticky up."
    - Throughout the exercises and code-along sessions, reinforce the use of
    troubleshooting techniques including finding help from other resources.
- We teach the *[tidyverse][tidyverse] way of using R*, meaning we use
packages like dplyr, tidyr, rmarkdown, ggplot2, and so on. This also means making
use of the pipe `%>%` operator.
- We follow the tidyverse [*way of writing and styling R code*](https://style.tidyverse.org/).
- Be kind, and remember, your words *matter a lot*. Try to avoid words like
"basically", "its just", "as simple as", and so on. This is difficult, but at least
try.

The majority of the lesson material is *participatory live-coding*, so use of
slides is minimal. The purpose of the course is to *type with the participants*,
to show by doing. 
Live-coding is a hands-on method of teaching coding to a group in which the
instructor shares their screen with the group and types out and narrates all the 
commands in real-time on their own computer while the group follows along.
Live-coding is a very effective teaching technique: it forces the instructor to
go slowly and ensures that participants get to try out every command being used.
It allows learners to experience common errors themselves, to see errors occur
when for the instructors (thus demystifying that everyone no matter the skill level
experiences errors) and debug them in a supportive environment, to explore
variations on material as they go, and to immediately check their understanding
by trying things hands-on.

Live-coding is a technique used by [Software Carpentry](https://software-carpentry.org/about/). 
Software Carpentry has lots of great resources explaining the why and how of live-coding:

- [10 tips and tricks for instructing and teaching by means of live coding](https://software-carpentry.org/blog/2016/04/tips-tricks-live-coding.html).
- The Software Carpentry [instructor training manual](https://carpentries.github.io/instructor-training/) 
includes many resources about programming education.

### Before your session

- Have an RStudio theme that uses a white background with black text.
This setting is easier to read on projectors.
- In `Global Options -> Appearance`, 
put a higher zoom value and increase the font size (maybe around 14). 
Exact zoom and font size depends on the projector.
- Put the Console and Script panes side by side rather than stacked. 
This can be changed in the `Global Options -> Pane Layout` 
- If you use Vim or Emacs keybindings in RStudio, change to the default that
the learners use, so that 1) they see similar behaviour as what you are doing
2) doing fancy/quick stuff is *not* going to help them learn, and 3)
it slows you down a lot more since your muscle memory for the default keybindings
will probably be similar to the learners muscle memory.

### Throughout the sessions

- For most of the sessions,
there are sections that tell the participants to read on their own.
Know beforehand where these sections are and
get them to read over the section when you come to it.
Preferably, you should briefly go over the content again, to reinforce what they read and to
address any questions, but don't spend too much time on it.
- For the exercises, 
make sure to get the learners are helping each other out in their groups.
- Exercise solutions do not need to be covered by the instructor,
given the solution is provided already. However, if there is time, it can be useful
to the participants to have the instructor narrate about how the code works and
why we used this code.
- Try to keep the screen on your RStudio as much as possible 
and don't switch applications often, 
only when you need to go to the course material or to show an exercise.
Otherwise people get lost, since they have to be looking up to the screen and
then down to their own laptops, which takes a lot more time.
- For code-along sessions, narrate what you are doing as you are coding by
providing explanations of what you hope to achieve with each function/piece of
code. This is particularly important for the wrangling sessions, where you
should explain what each function does and examples of instances where you would
use each function.
- Try not to deviate too much or go on tangents during the code along. The
code-along should have almost the exact same code as is on the website.
- Be aware of how much space you have on the projector screen 
and don't let R code go too long. 
You have two options to take so that all code stays on the screen
(use which ever you find most visually appealing):
    1. Use soft-wrapping of R code. 
    You can set this in RStudio by going to `Tools -> Global
    Options -> Code -> Editing tab`
    and then tick the "Soft-wrap R source files" option.
    2. Or, adding more lines to the code then you normally would use.
    For instance, instead of:

        ```r
        ggplot(NHANES, aes(x = BMI, y = Age, colour = Diabetes)) +
            geom_point()
        ```
    
        You could add new lines like:
    
        ```r
        ggplot(NHANES, 
               aes(x = BMI, 
                   y = Age, 
                   colour = Diabetes)) +
            geom_point()
        ```

### Using the slides

The slides are generated from the [xaringan] R package,
which uses [remark.js].
In the slides, there are notes that you can read 
either by going to the source `.Rmd` file 
or by opening the slides and hitting the `p` key.
To use the slides more efficiently, 
check out the [remark.js keyword shortcuts].

[remark.js]: https://remarkjs.com/#1
[xaringan]: https://github.com/yihui/xaringan
[remark.js keyword shortcuts]: https://github.com/gnab/remark/wiki/Keyboard-shortcuts
