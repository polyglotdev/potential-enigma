# Volley Prompts Wrap Up

## Pipenv

**I use pipenv to manage my python projects. Pipenv is also the officially recommended Python packaging tool from Python.org**.

It automatically creates and manages a virtualenv for your projects, as well as adds/removes packages from your Pipfile as you install/uninstall packages. It also generates the ever-important Pipfile.lock, which is used to produce deterministic builds.

Instead of giving you verbose documentation to read I am just going to include the video that explains the install.

- Pipenv Video: https://vimeo.com/233134524
- Pipenv Documentation: https://vimeo.com/233134524

## spaCy

**spaCy is production ready NLP written in Python**

- Installation:
  - `mkdir data-science && cd data-science` create a folder and cd to that dir. Run `pipenv shell` to create your virtualenv as well as spin up spaCy. From here run, `pipenv install spacy` This will install spacy locally to this dir
  - To get the models you need, `python -m spacy.en.download all` from within pipenv shell. You can check your install by typing `python` which will open the Python shell and from within it you can follow these commands:
    ```
    nlp = spacy.load('en_core_web_sm')
    doc = nlp(u'Apple is looking at buying U.K. startup for $1 billion')
    for token in doc:
      print(token.text)
    ```
- If spaCy is installed correctly, your doc will be tokenized.
- You will also need the vectors so install gloVe as well: `python -m spacy.en.download glove`

## Jupyter Lab

`pipenv install jupyterlab`

- This will install jupyter lab which is the newest version of what was known as 'ipython notebook.' To run the notebook you use `jupyter lab` to start a session.

## "Other"

In the notebook you will find that I used a few other tools. Python documentation does a more than adquete job of explanation on `shuffle(), random()` etc etc. If you have questions please feel free to reach out with a pull request.

## Running

Im not a fan of assumptions so I going to step you through how to use the notebook at a high level. Each cell that you see operates as a block of code. To run that block you can use `shift and enter` at the same time. The first **4 cells** you just need to `shift + enter` thru them. When we reach the cell marked `txt` with the multiline comment we are ready to go.

- Grab text from any place that you want online. Between the multiline comment you need to place your text and press `shift + enter`
- Grab a second set of text and do the same thing in the next cell. `shift + enter` to move forward.
- Thru the next 9 cells you can press `shift + enter` and the model will run thru your text and give you back questions and the answer.
- This was a rough run and no tests have been written. This was to work on tokenization, using models, understanding word vectors/Named entity recognition as well as scope. Not by any means a finished product.

## What I learned..

1. Scope and Feature creep:

   - It was noted that the prompts are not scoped for a junior engineer and not knowing fully what I was walking into, I ignored the logical plea to just do what was asked and attempted to do the orginal prompt which inluded that I did plus web app that would be an mvp. What I came to find out was, I am just not capabale of that currently without direction. The lesson was clear; Do what was asked to the best of your ablity and if you have questions, _ask_ before creating some new derivative of the orginal task because all you do is double your work and slow your team down. Do go rougue.

2. Understanding what questions you need to ask when you are stuck.
   - My orginal plan was to do the second prompt fully and I started off great. Wireframes, sketches and what have you. I quickly realized that the knowledge needed to pull this off was not within my grasp given what I knew. What I had to accept what I did not know. During my stubbling around I ran across Geroge Polya's book, "How to solve it". I also found a rare video of one if his lectures, [Polya exaplains the problem solving method](https://www.youtube.com/watch?v=h0gbw-Ur_do). His method for problem solving are fantastic.
   - Understand the Problem
     - What are you solving
   - Devise a plan
     - Inductive reasoning to look for a pattern
     - Make a systematic list or table
     - Estimate an answer
     - Draw a picture
     - relate problem to similar problem and resue techniques
     - if it seems too easy there a reason so look for a catch
     - Use your common sense
   - Execute
   - Look back and check the answer

- Understanding the problem is what leads to answer. One also should not see the problem as the barrier as well. Problems beg to be answered. Whatever problem you are having if you see it as an opputurtunity to overcome through logic, it will serve us all well.

## Approach

After the defeatism subsided and I was able to get on track I began to use the resources that I had in front of me the whole time. Youtube, documentation and slack gave me the lot of direction I needed to complete a task that I was clearly not prepared for. Humility was the largest helper because I understand that I don't know what I don't know and I am willing, even if I look stupid, to ask questions in public to get to a desired end. I reached out to people that had exerpience and asked those questions to get here. This was not done by me alone, but on the backs and minds of those better than me. To close, this was beyond my reach and instead of folding it up and quitting, I pushed. While I have a **long** way to go regardless of if this leads to career with Volley, I'm thankful I did this.
