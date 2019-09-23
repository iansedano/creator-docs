# Creating Quizzes


Click on "Save and display"



## Use the Question Bank

Create and manage questions using the Moodle **Question Bank**.

<https://platform.codingnomads.co/learn/question/edit.php?courseid=8&cat=529%2C238>

### Create And Use Categories

These help to keep questions searchable and make it easier to add and edit questions related to a specific quiz.

## Question Behavior

We want students to receive immediate feedback if possible. Therefore, we encourage to use **"Adaptive Mode"** (the default) for quiz questions. You can see other possible modes in Moodle's docs on [Question behaviour](https://docs.moodle.org/37/en/Question_behaviours).

**Note:** Please use other modes only if you have a good and justified reason to do so. Chat me up with those reasons before getting started.

## Feedback

Students should be able to "check" their answers to questions and receive feedback. For this, you will need to fill out the "Feedback" blocks when creating a question.

## Open-Ended Text Questions

The suggested question type to use for questions that are designed to prompt students to think and formulate their own answers, is [**Essay (autograded)**](https://github.com/gbateson/moodle-qtype_essayautograde).

**Set the stage:** Use [this information-question](https://platform.codingnomads.co/learn/question/edit.php?courseid=8&cat=530%2C238&qpage=0&category=530%2C238&qbshowtext=0&recurse=0&showhidden=0) as the first question of each open-ended quiz you create. It will signify to students that they are entering exploration mode, as well as provide useful tips and a link to our forum.

### Required Settings

In order to use the default auto-grading, specify a minimum number of characters to be used. This needs to be >0 (e.g. `1`). If this setting is left at `0`, then students will receive an "Incorrect" mark when submitting any written content.

### Additional settings

You can specify keywords etc. to give students automated feedback.

## Regex short-answer questions

These work great for giving more flexibility to students' answers.

<https://docs.moodle.org/37/en/Regular_Expression_Short-Answer_question_type>

You can:

* write Regex to specify a **limited set of answers**:

    Q: Write one keyword that is part of a Python conditional
    A: (if|elif|else)

* write Regex to **exclude** a wide set of wrong answers

    Q:

**Note:** The plugin is designed to prevent **correct answers** that have endless possibilities - therefore the use of Regex for correct answers is limited.

This is purposefully designed like that.

The whole power of regex is available to you to identify **incorrect answers**, and you need to be more specific with correct answers.
