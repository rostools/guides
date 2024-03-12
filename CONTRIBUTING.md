# Want to contribute? Great! :tada: {#contributing}

There are a few ways in which you can contribute:

-   Participating in the discussions on issues.
-   Adding to lesson material.
-   Instructing a lesson or helping out.

## Participating in issue discussions :thought_balloon: :question:

Helping to contribute can be as simple as giving feedback, suggestions,
or thoughts about a topic or issue. You'll need a GitHub account to add
your comments on the course development in the repository. As always,
make sure to adhere to the [Code of Conduct](CODE_OF_CONDUCT.md).

## Adding to or editing lesson material :pencil: :computer:

The lesson material and website are created using
[Quarto](https://quarto.org/), which renders the `.Rmd` or `.qmd`
documents and converts the source material into a static website. A few
things to consider when contributing to the lesson material:

1.  All lesson material that contains R code chunks needs to be in R
    Markdown (`.Rmd`) or Quarto (`.qmd`) format.
2.  Every lesson "chapter" starts with and has only one first level
    "header" (`#`).
3.  Lessons include a mix of code chunks and text, organized using
    Markdown headers.
4.  Participants should be able to follow the content of the lesson from
    the text alone; i.e. the file should contain *all* conceptual
    explanations.
5.  We teach the [*tidyverse*](https://www.tidyverse.org/) *way of using
    R*, meaning we use packages like dplyr, tidyr, rmarkdown, ggplot2,
    and so on. This also means making use of the pipe `%>%` operator.
6.  We follow the tidyverse [*way of writing and styling R
    code*](https://style.tidyverse.org/).

Anyone can contribute to the course repository through GitHub by
creating a new Issue to make comments and give feedback for the material
in the course repository. This is the easiest way to contribute.

You can also contribute by adding or modifying text or code either
directly on GitHub through their editing interface (easier way) or you
can create a clone of the repository and edit through RStudio (harder
but the preferred way). If you go the clone route, please use [the
GitHub flow style](https://guides.github.com/introduction/flow/) to
manage changes. Here are some steps to follow:

1.  [Clone](https://help.github.com/articles/cloning-a-repository/) the
    repository to your local computer.
2.  In your local copy of this repository, create a new
    [branch](https://help.github.com/articles/about-branches/) that will
    address one or two Issues.
3.  Make edits to files and content that is specific to only a few
    Issues. Smaller changes made as a Pull Request are easier to review
    and merge than bigger changes. The more targeted and specific the
    changes are, the better.
4.  As you make edits, commit your changes to that branch.
5.  Push the edits on that branch to the course repository. Note that
    this assumes you have been added to the repository as a contributor.
    Otherwise, you'll need to make a
    [fork](https://docs.github.com/en/get-started/quickstart/fork-a-repo)
    of the repository first.
6.  Submit a merge/pull request of the branch into the main branch.
7.  If you receive feedback on your pull request, make further commits
    to the branch on your cloned local copy. These will automatically be
    added to your merge request after you commit and push.

Alternatively, use the usethis package
[`pr_`](https://usethis.r-lib.org/articles/pr-functions.html) helpers to
contribute. Read over the [Coding
Club's](https://coding-club.rostools.org) post on [how to use usethis to
contribute to a project on
GitHub](https://coding-club.rostools.org/posts/branches-and-actions/).

Making videos (on Linux) is done using
[Peek](https://github.com/phw/peek) (setting the window size to
1280x720), [OpenShot](https://www.openshot.org/) (to edit the video if
necessary), and the below command to reduce the video file size:

```         
ffmpeg -i input.mp4 -crf 28 output.mp4
```

### (Re-)Building the website

In order to build the website, you need to have the dependent packages
installed. Packages used and depended on for this course are included in
the `DESCRIPTION` file. To install the packages, run this function in
the root directory (where the `.Rproj` file is located):

``` r
# install.packages("pak")
pak::pak()
```

If the project is managed by renv (there is an `renv.lock` file), you
need to install the dependent packages by:

``` r
# install.packages("renv")
renv::restore()
```

To re-build the website from the source R Markdown or Quarto files, use
the keybinding `Ctrl-Shift-B` while in the RStudio Project of the
repository or by clicking the "Render" button at the top of the Source
Pane.

## Code of Conduct

We adhere to a [Code of Conduct](CODE_OF_CONDUCT.md) and by
participating, you agree to also uphold this code.

## Acknowledgements

Parts of the file were modified from
[UofTCoders](https://github.com/UofTCoders/studyGroup/blob/gh-pages/CONTRIBUTING.md)
and [The
Carpentries](https://docs.carpentries.org/topic_folders/hosts_instructors/hosts_instructors_checklist.html#instructor-checklist)
contributing guidelines.
