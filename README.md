<!---

TASK LIST:

  * Use cp -rf *.* to copy all of the files and directories in this repository
    to the starter repository for this assignment
  * Change into the directory for the starer repository
  * Update the header (e.g., #) to only give the name of the assignment
  * Update the first paragraph to include the commented-out content
  * Change the link in the # Problems section to point to this lab's starter
  * Create the assignment in the GitHub Classroom, noting the URL
  * Test the assignment by accepting it with your own GitHub account
  * Check to ensure that your GitHub repository is created correctly
  * Share the assignment link with all of the students using email or Slack

PROBLEMS?

  * Contact Gregory M. Kapfhammer by email or Slack
  * Raise an issue in the GitHub repository for this assignment

-->

# cs103-S2018-practical4-starter

Designed for use with [GitHub Classroom](https://classroom.github.com/), this
repository contains the starter for Practical 4 in Computer Science 103. Since
the Travis builds for this repository will initially fail (as evidenced by a
red &#x2717; appearing in the commit logs instead of a green &#x2714;), the
programmer is responsible for completing all of the steps needed to satisfy the
requirements for the assignment, thus causing a &#x2714; to instead appear in
the commit logs.

## Introduction

This assignment requires a programmer to implement a static web site using the
HTML and CSS programming languages. Specifically, you will develop a
professional biography site for use in a later assignment. For this laboratory
assignment, you will also link to a locally stored image that you take and
download from a mobile device. You will also continue to learn how to program
in HTML5 using tags. Next, you will learn how to reference local cascading
style sheet (CSS) files and include an emoji in your web site. You will also
style the fonts and HTML elements in your web site with a local CSS file. Then,
you will run a web server to provide local access to the static web site,
specifically loading the default document. Finally, you will continue to
practice using the [HTMLHint](http://htmlhint.com/) static analysis code tool
that can check HTML files for potential errors.

The source code in the `index.html` file must also pass additional tests set by
the [GatorGrader tool](https://github.com/gkapfham/gatorgrader). GatorGrader
will check to ensure that your HTML file contains the required header and that,
for instance, the CSS file features specifications for the correct borders and
fonts. GatorGrader will also check that you made the required number of
commits to your repository. More details about the GatorGrader checks are
included later in this document and in the assignment sheet.

When you use the `git commit` command to transfer your source code to your
GitHub repository, [Travis CI](https://travis-ci.com/) will initialize a build
of your assignment, checking to see if it meets all of the requirements. If both
your source code and writing meet all of the established requirements, then you
will see a green &#x2714; in the listing of commits in GitHub. If your
submission does not meet the requirements, a red &#x2717; will appear instead.
The instructor will reduce a programmer's grade for this assignment if the red
&#x2717; appears on the last commit in GitHub immediately before the
assignment's due date.

A carefully formatted assignment sheet for this project provides more details
about the steps that a computer scientist should take to complete this
assignment. You can view this assignment sheet by visiting the listing of
laboratories on the course web site.

## Learning

If you have not done so already, please read all of the relevant [GitHub
Guides](https://guides.github.com/) that explain how to use many of the features
that GitHub provides. In particular, please make sure that you have read the
following GitHub guides: [Mastering
Markdown](https://guides.github.com/features/mastering-markdown/), [Hello
World](https://guides.github.com/activities/hello-world/), and [Documenting Your
Projects on GitHub](https://guides.github.com/features/wikis/). Each of these
guides will help you to understand how to use both [GitHub](http://github.com)
and [GitHub Classroom](https://classroom.github.com/). To learn more about how
to include an emoji in an HTML file, please read the documentation for the
[Emoji CSS library](https://afeld.github.io/emoji-css/). To learn more about
Google's web fonts, please visit [Google Web Fonts](https://fonts.google.com/).

To do well on this assignment, you should also review Chapters 1 through 4 of
the course textbook, paying close attention to Sections 4.1 through 4.7 and
Figures 4.3, 4.18, 4.20, and 4.31 and Table 4.9. Please see the course
instructor or one of the teaching assistants or tutors if you have questions
about any of these reading assignments.

## Commands

To get started in using the GatorGrader tool, you can change into the directory
for this assignment and type the command `./gatorgrader.sh --start` in your
terminal. Now, if you want to perform all of the checks that will
automatically evaluate your assignment, you can type the command
`./gatorgrader.sh --check`. Please note that the GatorGrader tool also runs
the `htmlhint src/www/index.html` command to "lint" your HTML file.

Running this command will produce a lot of output that you should carefully
inspect. If the last line of the output indicates that GatorGrader judges that
there are no mistakes in the assignment, then this means that your source code
and writing are passing all of the automated checks. However, if the last line
of the output indicates that there are mistakes, then you will need to
understand what they are and then try to fix them.

If the course instructor publishes a new version of GatorGrader and asks you to
access it, then you need change into the tool's directory by typing `cd
gatorgrader`. Then, you can type the command `git pull` to download the new
source code for the GatorGrader tool. If this command completes successfully,
then you can return to the main directory for this practical assignment by
typing `cd ..` and then continuing your work.

## Checking

In addition to making the checks that were previously mentioned in the
introduction to this document, your final submission must meet the following
requirements.

- The `index.html` file loads the web fonts from `fonts.googleapis.com`.
- The `index.html` file loads the web fonts in the form `Montserrat|Roboto+Slab`.
- The `index.html` file includes an image called `img/professional_photo.jpg`.
- The `index.html` file includes the main header with the words `Professional Biography`.
- The `index.html` file has one `<blockquote>` that features your professional biography.
- The `index.html` file contains a footer created with the `footer` tag.
- The `index.html` file loads two emoji using the `em em-` fragment.
- The `site.css` file specifies `font-family: "Roboto Slab", serif;` for the
  header font.
- The `site.css` file specifies `font-family: "Montserrat", sans-serif;` for the
  body font.
- The GitHub repository must contain at minimum three new commits with
  descriptive messages.

## Updates

If the course instructor updates the provided material for this assignment and
you would like to receive these updates, then you can type this command in the
main directory for this assignment:

```
./gatorgrader.sh --update git@github.com:Allegheny-Computer-Science-103-S2018/cs103-S2018-practical4-starter.git
```

You should only need to type this command once; typing the command additional
times may yield an error message but will not negatively influence the state of
your repository. Now, you are ready to download the updates provided by the
course instructor by typing:

```
./gatorgrader.sh --download
```

This second command can be run whenever the course instructor needs to provide
you with new source code for this assignment. However, please note that, if you
have edited the files that the course instructor updated, running the previous
command may lead to Git merge conflicts. If this happens, you may need to
manually resolve them with the help of the instructor or a teaching assistant.

## Travis

This assignment uses [Travis CI](https://travis-ci.com/) to automatically run
the checking programs every time you commit to your GitHub repository. The
checking will start as soon as you have accepted the assignment, thus creating
your own private repository, and the course instructor enables Travis for it. If
you are using Travis for the first time, you will need to authorize Travis CI to
access the private repositories that you created on GitHub.

## Requirements

The GatorGrader software that supports the checking of this assignment was
developed for the following software and versions:

- mdl 0.4.0
- proselint 0.7.0
- python 3.5.2

## Problems

If you have found a problem with this assignment's provided source code, then
you can go to the [Computer Science 103 Practical 4
Starter](https://github.com/Allegheny-Computer-Science-103-S2018/cs103-S2018-practical4-starter)
repository and create an issue by clicking the "Issues" tab and then clicking
the green "New Issue" button. If you have found a problem with the [GatorGrader
tool](https://github.com/gkapfham/gatorgrader) and the way that it checks you
assignment, then you can follow the aforementioned steps to create an issue in
its repository. To ensure that your issue is properly resolved, please provide
as many details as is possible about the problem that you experienced. If you
discover a problem with the laboratory assignment sheet, then please raise an
issue in the
[cs103-S2018-sheets](https://github.com/Allegheny-Computer-Science-103-S2018/cs103-S2018-sheets)
repository and mention this assignment.

Students who find, and use the appropriate GitHub issue tracker to correctly
document, a mistake in any aspect of this laboratory assignment will receive
free laptop stickers and extra credit towards their grade for it.

## Assistance

If you are having trouble completing any part of this project, then please talk
with either the course instructor or a teaching assistant during the laboratory
session. Alternatively, you may ask questions in the Slack team for this
course. Finally, you can schedule a meeting during the course instructor's
office hours.
