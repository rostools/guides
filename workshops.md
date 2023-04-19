# Admin and running a workshop 🏫

The [r3admin](https://github.com/rostools/r3admin) R helper package
automates many aspects of running the course, at least at the
administrative and coordinating side of things. Read the documentation
there to see how to use that package to streamline admin tasks.

## Instructor and helper number

-   The recommended number of instructors for a 25-35 class size is
    about 3-6 instructors (\~1 instructors for every 1-2 sessions). If
    there are more instructors, than less helpers are needed.

-   A recommended ratio of instructor/helper to participant is about 1
    to 4-6, which we've found ensures the smoothest learning experience.

-   Once you have confirmed your team of instructors and helpers, use a
    messaging app (WhatsApp, Telegram, Signal, or Slack) to set up a
    group chat that supports easy communication.

## Before the course

-   The function `r3admin::admin_create_planning_issue()` in the r3admin
    package creates an issue to help manage the course. Check the
    r3admin package for documentation on it.

-   Setup the course R Project beforehand so that the instructors can
    use it. Create as a Git repo and push up to GitHub, so instructors
    can clone the project before their session.

-   If there is group work, keep group size to 4 learners per group. Any
    more and they end up starting to split into smaller groups within
    the group. Plus, 4 learners per group is a good way to arrange
    learners in the room and at the tables.

    -   If there are groups, randomize it so participants go with random
        people. Since courses are also a chance to network and meet new
        people, forcing them into groups with new people helps to set
        the atmosphere so that everyone intentionally doesn't know the
        others (though they might by chance). Having people randomly
        assigned to groups also reduces the anxiety associated with
        "having to find or make a group".
    -   There are often R scripts in the course repositories that help
        with making these groups, usually in `R/create-teams.R` or
        something similar.

## The first day

-   Make sure the tables are arranged to participants are facing the
    projector, so they don't twist their necks

    -   If there are groups, keep groups connected together in tables,
        have space between the groups for instructors and helpers to
        walk through
    -   Arrange it so participants go to their assigned tables as they
        enter by putting their, for instance, name tags or names at the
        table.

-   During the introduction, don't forget to introduce all the
    instructors and helpers.

-   In the room, arrange the tables into groups for each of the teams.
    As participants come in, get them to sit in their assigned team by
    referring to the team lists placed in the middle of each table.

-   (Optional idea) Before the lunch break, get the groups to have lunch
    together and introduce each other more. Get them to say their
    program, if they've used R before, some struggles they've had with R
    and with data analysis in general, and/or why they want to learn R.

## During the course

-   Be more strict about time management of exercises (move on even if
    they don't finish).

## End of the course

-   **End of course**: Ask if any participant would like to be involved
    in next year's teaching, or in making the material, or in being a
    helper.

-   It's a good idea to do a debrief with all the instructors on what
    worked and what could be improved after the workshop finishes. It's
    also a time to give peer feedback. Workshops aren't just a source of
    learning for the participants, but also for the instructors! So,
    while you are teaching or helping out, keep note of any feedback or
    comments you could give to improve the other instructors' (and your
    own) teaching. During the debrief we'll each say one thing each of
    us should continue doing and two things that they could improve on.

## General course admin

### About using surveys

We used Google Forms to create surveys for pre-, during-, and
post-course feedback and questionnaires. The purpose of using surveys in
the current context is purely to gain feedback on aspects of the course
that could be improved in future iterations, such as the "pace" of
material being presented.

The interface for creating surveys is quite clear and functions are very
intuitive. You will see a floating menu to the right of your template
where you can add questions etc. One particularly useful tool is the
ability to duplicate question and answer matrices. If you are using this
course material to run your own independent workshop and want the
surveys to use as a template that you can then customize, create a [new
issue](https://github.com/rostools/r-cubed-intro/issues/new) to request
access.

We included survey links as a function within the r3 package so learners
can quickly access the survey. Creating surveys is quite easy with
Google Forms. Below are a list of questions to include (depending on the
survey):

-   **Pre-course**:
    -   Basic questions about the participant (position, name, place of
        work).
    -   Questions about perceived skill/knowledge on using R,
        programming, data analysis, and version control.
    -   Questions related to their pre-course tasks.
    -   Feedback on the pre-course tasks, like: What worked well? What
        could be improved?
-   **Daily feedback**:
    -   For each session, we asked: What worked well? What could be
        improved?
    -   For final session, we asked broader quantitative comments like:
        I think I learned a lot; I think the instructors communicated
        clearly; I think there was good alignment between content and
        delivery.
-   **Post-course**:
    -   Basic questions about the participant (like in the pre-course
        survey).
    -   Questions about current usage of the tools they learned during
        the course.
    -   Questions about and reflections on the course.

### About the r3 package

The r3 package is used as a companion and helper throughout this course
to making it easier to do certain tasks like go to the survey or install
packages necessary for the course. Considering this, if you want to use
this course material and run a course like this on your own, you can
clone the r3 package and modify it as necessary for your own purposes.
See the [README](https://github.com/rostools/r3/blob/main/README.md) of
the r3 package for more details.
