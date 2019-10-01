# Creator Call

- set markdown as default option in plain text editor

- example section of cloned course
    * make sure the completion settings are set correctly etc.

short screencast videos
- how to clone a resource
- what needs to be done?



* call about pedagogy
    - how to best teach content?


----


- Welcome:
    * who's who, what course
    * first batch of content creators

- Creator Docs
    * Basic Idea - make life easier, assure consistency and quality
    * writing tips
        - parallel structure
        - consistent formatting
        - tone!
    * stay DRM-free, don't plagiarize

- Use Markdown
    * why? - show process on platform
    * how? - show VSCode (or any other)
    * (host on GitHub for feedback)
    * input? - show process on platform -- ADMIN ONLY!

- Our Platform
    * copy a slice of an existing course to jumpstart
    * these docs will have important info and walkthroughs
    * ask when you're ready to input

- Quizzes
    * **Adaptive Mode** for everything
    * CodeRunner
    * Open-ended text questions

- Labs
    * Numbers + names in file name formatting
    * Instructions in code comments, so students can start coding below

- Early Feedback
    * share content while in development, let's chat about it

- Questions?
    - Jupyter Labs Server --> let's try it out





# Organization During Development
Explore whether it makes sense to use Trello boards on a per-course basis.

# Course Maintenance and Updates
It's a lot of work. How to handle this best? Eventually we should have someone who works on just that.


# General Course Settings
* set up auto-completion course-wide as follows:
    - _insert settings_

# Content
* stay DRM-free! We don't want to plagiarize.
    - Images: Only use images you made yourself or that are in the public domain. Creative Commons requires attribution, so post a link.
    - External Learning Resources: Link to great external resources you know of. Our main goal is for students to learn the topics. We want external resources to be clearly labeled and an _addition_ to our course content, not a replacement


# In-course quizzes
* quick and direct feedback - use "Adaptive Mode"
    - general quiz set-up guidelines
* sololearn style check-in quizzes
* incorporate drag&drop, cloze deletion, etc.

# Formatting: Use .md
* consistent formatting: markdown (easy to write and re-use)
* use Bootstrap for styling (it's included in the moodle theme)

## Bootstrap Elements We Use
Avoid styling pages in the editor, it makes it individual and difficult to globally adapt and keep in sync.

Best way is to use Markdown with only little extra styling.

- jumbotron for resources? (maybe tone it down?)
- quotes?

- headings (avoid bolding etc in editor)
- jumbotron resources
    * [Collapsible](https://platform.codingnomads.co/learn/mod/page/view.php?id=102) also cool for resources
    * more difficult to build every time (more HTML code)
    * create a PHP button to insert the HTML for such snippets?
- jumbotron tasks ([ex1](https://platform.codingnomads.co/learn/mod/page/view.php?id=573), [ex2 both JT](https://platform.codingnomads.co/learn/mod/page/view.php?id=156))
- quotes in `quote-card`
- container for "Notes"
- other repetitive sections?
- increased `code {font-size: 1.1em;}`
- general font-size relatively small
- code blocks for different languages (plugins!)
    * code highlighting is [sometimes bad](https://platform.codingnomads.co/learn/mod/page/view.php?id=135)

# Labs

We host labs on GitHub, one folder per course.

Students (clone or) download the ZIP from GitHub at the beginning of the course
- download: no sync for updates we do
- clone: requires some pre-existing Git knowledge

- one repo per course, like [here](https://github.com/mikeckennedy/write-pythonic-code-demos) with ads in README
- encourage version control and open-source from the start
- people who just want the exercises won't buy the course anyways - there's code snippets and projects everywhere

## Use Consistent Numbering

Double-digits (should we do triple?)

Here's a link to a tool that helps with renaming. You'll need it probably...

<https://github.com/CodingNomads/utils>



# Teachable Summit

Could be interesting (could be crap):

<https://teachable.com/live/register>


# Videos


# Thoughts
* “Workshop” resource for peer reviewed content
* Checklist resource (I did this, this, this - ok, move on!)
    - (maybe) also for **Tasks**


# Mobile
Mobile site available at https://platform.codingnomads.co/learn Tried it, works, and looks good! :)

# Grades
Checking grades on mobile threw an error that was helpful
So I switched on “Graded Roles” for course creators and teachers in
Dashboard / Site administration / Grades / General settings

But I don't think we'll need grades, so I removed it from the User menu

Aiming to keep the interface as clean as possible for students, avoid links that are not necessary.




## Disclaimers

Add disclaimers `<alert>` boxes when a new concept is mentioned but not deeply explained. You want to avoid students feeling like this:

>you know, I think my main issue is if I get to a page, and the way it is written implies I should already understand it, but it is completely new and unfamiliar. It has me worrying that it is obvious and I am the only one just not getting it.

