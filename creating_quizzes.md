# Creating Quizzes

## Use the Question Bank

Create and manage questions using the Moodle **Question Bank**.

<https://platform.codingnomads.co/learn/question/edit.php?courseid=8&cat=529%2C238>

### Create and use Categories

These help to keep questions searchable and make it easier to add and edit questions related to a specific quiz.

## Question Behavior

We want students to receive immediate feedback if possible.

Therefore, we encourage to use "Adaptive Mode" (the default) for quiz questions.

You can see other modes here:

<https://docs.moodle.org/37/en/Question_behaviours>

Please use other modes only if you have a good and justified reason to do so. Happy to chat with you about those reasons.

## Feedback

Students should be able to "check" their answers to questions and receive feedback.

For this, you will need to fill out the "Feedback" blocks when creating a question.

## Open-ended text questions

The suggested question type to use for questions that are meant to prompt students to think and formulate their own answers, is `Essay (autograded)`:

<https://github.com/gbateson/moodle-qtype_essayautograde>

Use this information "question" at the beginning of each open-ended quiz:

<https://platform.codingnomads.co/learn/question/edit.php?courseid=8&cat=530%2C238&qpage=0&category=530%2C238&qbshowtext=0&recurse=0&showhidden=0>

### Minimum setting

In order to use the default Auto-grading, specify a minimum number of words to be used.

This needs to be >0 (e.g. `5`).

If this setting is left at 0, then students will receive an "Incorrect" mark when submitting any written content.

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

**NOTE:** The plugin is designed to prevent **correct answers** that have endless possibilities - therefore the use of Regex for correct answers is limited.

This is purposefully designed like that.

The whole power of regex is available to you to identify **incorrect answers**, and you need to be more specific with correct answers.
