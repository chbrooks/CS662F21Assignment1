# CS662 Assignment 1

 ###Due Date: Monday, Sept 13, start of class.

In this assignment, you'll characterize some AI problems according to the different parameters presented in lecture and in the text. 
This assignment is also meant to get you up to speed with Python. For all
assignments, you must use the provided template code as a starting
point.

To turn in your assignment, just commit your finished code to your repo, along with a file containing the written answers.

You are expected to follow best practices in terms of software
development. In other words, please make your code easy to read and
understand. In addition, you are expected to provide a README
describing how to run your code, and a simple test script.

Also, please make sure your name is in your code! It's not always easy to match repo names to students.

(25 points) Part 1. Problem characterization.
   
Consider the following potential AI problems. For each of them:
- describe whether the environment is: 
  
   a) static or dynamic 
  
  b) fully or partially observable 
  
  c) episodic or sequential 
  
  d) deterministic or stochastic. 
  
  Please explain your reasoning.
   
- List the actions that you would use to model each of these agents.

Please place your answers in a Word or PDF document added to your repository for this assignment.

- A robot such as [Perserverance](https://www.nasa.gov/perseverance), which can explore the surface of Mars.
- An AI such as [Kuki](https://www.pandorabots.com/kuki/) that can carry on a conversation with a user.
- A robot [such as this one used by Recology](https://www.youtube.com/watch?v=ft07TQ_ul6g&ab_channel=BulkHandlingSystems%28BHS%29) that can sort through trash and select items that are not recyclable.
- OpenAI's [Five](https://openai.com/five/) agent, which is able to play the computer game Dota 2.


(25 points) Part 2: Word frequencies. One of the primary domains we'll  work
  with this semester is text. The most common approach to dealing with
  large bodies of text is statistical, which requires counting the
  number of words in a document.

wc.py gives you a starting point for a program that will read words from a file and construct a frequency distribution. Please add the following features - 
you may need to explore the Python documentation a little to figure these out.

1. The way we're processing command-line args is icky. Please replace this with the argparse module.

2. The current wc.py will only process a single file. Fix it to be able to take as input a directory name or path and call wc for all files in that directory, or subdirectories. (look at os.walk() to see how to do this.)

3. Add a '--hist=picklePfile' argument. If this is present, you should instead read in a previously pickled frequency distribution and print out the words and counts. 
   If the '-s' argument is present, print the words in order of increasing frequency.


(25 points) Part 3. Graphs. This problem will give you some experience coding in Python in an object-oriented style. 
The sample code in the assignment's github repo implements a graph as an adjacency list. Please add methods to implement:
- Breadth-first search
- Depth-first search
- Djikstra's shortest-path algorithm
- Prim's spanning-tree algorithm
- Clique detection

There are comments in the code that give more detail.


(25 points) Part 4. This problem will give you some experience working with Pandas. Please add a file called pandasExercise.py to your repo containing this part.

First, read through [10 Minutes to Pandas](https://pandas.pydata.org/docs/user_guide/10min.html#min). There's a ton of other useful documentation of the pandas site as well.

The rest of these exercises use [The Pandas Cookbook](https://github.com/jvns/pandas-cookbook)
We'll also use the breast cancer dataset included in the GitHub repo. This is a classic ML dataset originally from the [UCI ML data repository](https://archive.ics.uci.edu/ml/index.php).

a) read Chapter 1.  Then, write a function that will read in the breast cancer dataset.

b) read Chapter 2. Then, write a function that determines the most common classification for the breast cancer data. (either 'recurrence' or 'no-recurrence')

c) read Chapter 3. Then write a function that determines the most common value for age and menopause for patients with recurrences?

d) Read Chapter 4. Write a function that plots the number of recurrences for each age group.

