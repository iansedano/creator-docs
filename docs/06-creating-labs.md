# Lab Resources

This section contains information about code training exercises (called "labs"). You can read about logistics regarding hosting and how to include them into your course, as well as some examples of how expected lab challenges could look like.

# Lab Content

Labs are the training exercises for your students. They are the ["katas"](https://en.wikipedia.org/wiki/Kata) of a programmer and should help your students to train their skills by pushing them to type and think and type some more. Repetition is an important part of learning, and while your main focus should be on getting students to work on interesting projects, some coding concepts simply require plain old training. Breaking concepts up into small parts that can be individually trained also helps students to keep on top of the large amount of new information they need to absorb.

## Form

To make it easy for students to start coding, you should provide them with files that include instructions so that they only need to open the file their preferred text editor and start coding.

## Example

An example file for our beginner Python course looks e.g. like so:

`01_06_hello5.py`
```python
'''
Write the necessary code to display "Hello World!" 5 times.
'''

```

The file contains the instructions for the lab's task as a python multi-line comment. Right underneath the comment the student can write and execute their code:

`01_06_hello5.py`
```python
'''
Write the necessary code to display "Hello World!" 5 times.
'''

print("Hello World! " * 5)
```

After finishing the task, they can push it back up to their GitHub repo and thus keep the instructions and the code side-by-side. This makes it easy for their mentor to give them feedback on the task.

# Hosting And Accessing Labs

**GitHub Hosted:** We host labs on GitHub, one repository per course. Our lab repos should look similar to [this course example](https://github.com/mikeckennedy/write-pythonic-code-demos) and link to a call for signing up for the course in their README file.

**Students Download Or Clone Labs**: Students either download the `.zip` for the repo from GitHub, or clone the repo at the beginning of taking the course. Generally, we want to encourage students to use version control and open-source right from the start. However, for beginner courses we opt for students to download a `.zip` file rather than making them jump through the hoops of using Git and GitHub.

* **Beginner Course**: Set up a URL Resource in your course that links to a "Download ZIP" URL of your course's GitHub repo.
* **Advanced Course**: You can opt to add a resource that explains students quickly how to clone your labs repo. We can assume that advanced students are already familiar with using version control.

Pro's and Con's for Downloading vs. Cloning the labs:

- **Download:** No sync for updates we do
- **Clone:** requires some pre-existing Git knowledge

# Ordering Labs

Files and file structures can easily get out of control and there are always 100 valid ways of setting up a repository. For uniformity's sake, we ask you to stick to the following setup. However, we are open for suggestions on how to improve the structure.

## Use Logical Folder Structure

When creating your labs it is best to follow a folder structure that mirrors the section structure of your course. Each course section should have some associated labs. A logical folder structure will help your students in their learning progress.

## Use Consistent Numbering

Use double-double-digit numbering for individual labs. This helps to keeps them in the order you intend students to tackle them.

Here's a link to [a script that helps with renaming](https://github.com/CodingNomads/utils). It's likely that you'll need to rename your labs in the process of creating your course. Feel free to use and customize this script as much as is helpful for you.

## Example Folder Structure With Lab Files

```
python_labs
|
├── 01_python_fundamentals
│   ├── 01_01_run_it.py
│   ├── 01_02_seconds_years.py
│   ├── 01_03_yeehaw.py
│   ├── 01_04_formula.py
│   ├── 01_05_addition.py
│   ├── 01_06_hello5.py
│   └── 01_07_area_perimeter.py

--- snip ---

├── 17_decorators
│   ├── 17_01_wraps.py
│   └── 17_02_tags.py
└── 18_lambdas
    ├── 18_01_first_lambda.py
    ├── 18_02_return.py
    ├── 18_03_rewrite.py
    ├── 18_04_hello.py
    ├── 18_05_names.py
    └── 18_06_tuple_sort.py
```
