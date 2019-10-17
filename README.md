# CMPSC 100-03 Practical Session 8

This practical asks you to consider ethical questions in the study of computer science and how an understanding of the role of ethical principles influences decisions that computer scientists make. In addition, this assignemnt is an exercise in group discussion, documentation, and teamwork. Though there is no strict "techncial" component here, this practical asks you to work on your technical writing skills of organization and clarity.

* Assigned: Friday, 18 October, 2019: 11:00 AM
* Due: Friday, 18 October, 2019: 11:50 am
* Point value: 20 points

## General guidelines for this particular practical session

* **Use your voice!** You are being asked to read sources, form an opinion, and use reasoning or evidence to support your choice. Given that you read the sources carefully, you should feel empowered to form arguments.
* **Practice your writing.** This is an opportunity for you to practice logical structure and clarity -- skills which are indispensible to both your academic and professional careers. If considered thoughfully, practice-focused issues in computer science _are meant to be hard questions_. Should you be able to communicate your thoughts clearly and logically, you'll be a step ahead of many in the discipline.
* **Try to finish during the class session.** While I provide extra time to complete the work, these assignments can be completed in 50 minutes. This will help you develop your awareness and management of time.
* **Respect one another.** Healthy dialogue starts from places of difference. Here, _difference_ may mean a host of things including: lived experience, understanding of technical issues, and much, much more. This may mean that you see things only _slightly_ different from  your team members. This may mean that you hold perspectives _dramatically_ different. In any case, seek to understand and then test your understanding based on your new knowledge. You may find that you change your mind -- even if only a little.

## Reading Assignment (Read these first!)

Read the following pieces (in order):

- [IEEE Code of Ethics](https://www.ieee.org/about/corporate/governance/p7-8.html)
- [ACM Code of Ethics and Professional Conduct](https://www.acm.org/code-of-ethics)
- [Mozilla Manifesto](https://www.mozilla.org/en-US/about/manifesto/)
- [Internet Health Report 2018](https://internethealthreport.org/2018/introduction/how-healthy-is-the-internet/)

## The activity

### Mechanics

* You will be assigned to a team (there are 4 teams).
* Locate and sit with your team at the same table.
* Designate a team leader.
* This team leader should go to the `#practicals` channel and acccept the assignment.
    * The team leader should create the team name using the materials provided at their table.
* Other team members should them clieck on the assignment link and choose `Join an Existing Team`, finding their team's name in the list.

### Discussion and writing prompts

Each team should consider, discuss, and draft responses (in the `reflection.md` file located in the repository's `writing` folder) to the following:

* What ethical considerations are important in the practice of computer science? What is unique about computer science and the ethical concerns that the discipine considers? 
    * Consider the three statements (IEEE and ACM codes of ethics, the Mozilla Manfiesto) -- what do they have in common?
* Why is it important to provide computer scientists with an ethical framework or to consider ethics when creating computational systems?
* How can computer scientists build systems that take ethics into account? For example, what responsibility do we, as computer scientists, have for building and maintaining a healther Internet, for example?

Each of these questions should be addressed using:

* Proper headings (at least 3) to separate answers to different questions
* At least 150 words per question:
    * Using least three separate paragraphs (1 per question)
    * Organized under the appropriate headings

## GatorGrader

### Docker `container`

If you do not already have the GatorGrader `container`, in a new terminal or Docker Quickstart Terminal, type `docker pull gatoreducator/dockagator` to download the correct `container`.

In the last lab session, we were able to get Docker `container` versions of GatorGrader working! That means that everyone can choose to use the `container` if they'd like. Here are a couple of ways to do it:

#### Running GatorGrader directly on `container` start

* Be sure that you are in the main directory of your practicals repository when running these commands, or you'll certainly experience issues!
* Remember that if you run `ls -la`, you should see a `.git` folder if you're in the main repository folder.
* To make sure you're in the right repository, run a `pwd` command.
    * If you recieve the expected path, you're in the right place. Else, find your way to the right location.

```
docker run -it --mount type=bind,source="$(pwd)",target="/project" --hostname GatorGrader gatoreducator/dockagator
```

#### Run `gradle` commands in the container

```
docker run -it --mount type=bind,source="$(pwd)",target="/project" --hostname GatorGrader gatoreducator/dockagator /bin/bash
```

- [ ] To `grade` your team's work, type `gradle grade` at the `command` prompt and press the `Enter` key.

### Using `gradle` commands directly

- [ ] To grade your team's work, type `gradle grade`

## `commit` your work

When you've finished your work: remember that there are three (3) steps to submitting a `git` repository: to "pack," to "label," and to "ship."

* Note: attempt all of these from the main directory of the repository.

- [ ] To "pack" the submission: `git add .`
- [ ] To "label" the submission: `git commit -m "{ADD MESSAGE DESCRIPTING PURPOSE OF COMMIT HERE}"`
- [ ] To "ship" the submission: `git push`
