## Pipenv

**I use pipenv to manage my python projects. Pipenv is also the officially recommended Python packaging tool from Python.org**.

It automatically creates and manages a virtualenv for your projects, as well as adds/removes packages from your Pipfile as you install/uninstall packages. It also generates the ever-important Pipfile.lock, which is used to produce deterministic builds.

Instead of giving you verbose documentation to read I am just going to include the video that explains the install.

- Pipenv Video: https://vimeo.com/233134524
- Pipenv Documentation: https://vimeo.com/233134524

## spaCy

**spaCy is production ready NLP written in Python**

- Installation:
  - `mkdir data-science && cd data-science` create a folder and cd to that dir. Run `pipenv shell` to create your virtualenv as well as spin up spaCy. From here run, `pipenv install spacy` This installs spacy locally to this dir
  - To get the models you need, `python -m spacy.en.download en` from within the pipenv shell. You can check your install by typing `python` which opens the Python shell, and from within it you can follow these commands:
    nlp = spacy.load('en_core_web_sm')
    doc = nlp(u'Apple is looking at buying U.K. startup for $1 billion')
    for token in doc:
    print(token.text)
- If spaCy is installed correctly, your doc will be tokenized.
- You also need the vectors so install gloVe as well: `python -m spacy.en.download glove`

## Jupyter Lab

`pipenv install jupyterlab`

- This installs jupyter lab which is the newest version of what was known as 'ipython notebook.' To run the notebook, you use `jupyter lab` to start a session.

## "Other"

In the notebook, you will find that I used a few other tools. Python documentation does a more than adquete job of explanation on `shuffle(), random()` If you have questions, please feel free to reach out with a pull request.

## Running

I'm not a fan of assumptions, so I am going to step you through how to use the notebook at a high level. Each cell that you see operates as a block of code. To run that block you can use `shift and enter` at the same time. The first **4 cells** you need to `shift + enter` thru them. When we reach the cell marked `txt` with the multiline comment, we are ready to go.

- Grab text from any place that you want online. Between the multiline comment, you need to place your text and press `shift + enter`
- Grab a second set of text and do the same thing in the next cell. `shift + enter` to move forward.
- Thru the next 9 cells you can press `shift + enter` and the model will run thru your text and give you back questions and the answer.
- This was a rough run and no tests have been written. This was to work on tokenization, using models, understanding word vectors/Named entity recognition as well as scope. Not by any means a finished product.

## What I learned

**Scope and Feature creep**<br />
It was noted that the prompts are not scoped for a junior engineer and not knowing entirely what I was walking into, I ignored the logical plea to do what was asked and attempted to do the original prompt which included the things I attempted plus a web app MVP. What I came to find out was, I am just not capable of that currently without direction. The lesson was clear; Do what was asked to the best of your ability and if you have questions, _ask_ before creating some new derivative of the original task because all you do is double your work and slow your team down. Do not go rogue.

**Understanding what questions you need to ask when you are stuck.** <br>
My original plan was to do the second prompt fully, and I started great. Wireframes, sketches and what have you. I quickly realized that the knowledge needed to pull this off was not within my grasp given what I knew. What I had to accept what I did not know. During my stumbling around I ran across Geroge Polya's book, "How to solve it." I also found a rare video of one of his lectures, [Polya explains the problem-solving method](https://www.youtube.com/watch?v=h0gbw-Ur_do). His method for problem-solving is fantastic.

1. Understand the Problem
   - What are you solving
2. Devise a plan
   - Inductive reasoning to look for a pattern
   - Make a systematic list or table
   - Estimate an answer
   - Draw a picture
   - Relate problem to similar problem and reuse techniques
   - If it seems too easy, there is a reason. Start looking for a catch
   - Use your common sense
3. Execute
4. Look back and check the answer

Understanding the problem is what leads to answer. One also should not see the problem as the barrier as well because problems beg to be answered. Whatever problem you are having if you see it as an opportunity to overcome through logic, it will serve us all well.

## Approach

After the defeatism subsided and I was able to get on track I began to use the resources that I had in front of me the whole time. Youtube, documentation and slack channels gave me a lot of direction. Humility was the biggest helper because I understand that I don't know what I don't know and I am willing, even if I look stupid, to ask questions in public to get to the desired end. I reached out to people that had experience and asked those questions to get myself the the task. To close, this was beyond my reach, and instead of folding it up and quitting, I pushed. While I have a **long** way to go regardless of if this leads to a career with Volley, I'm thankful I did this.
