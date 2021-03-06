01_Git_and_Intro
================

Practice with basic git functions, and intro to study of Data Structures

Reading
=======

**Version Control with Git, 2nd Ed**. Loeliger and McCullough. 

http://proquest.safaribooksonline.com/book/databases/content-management-systems/9781449345037/version-control-with-git/id302681?uicode=ohlink (Free access through www.lib.miamioh.edu, but limited to 100 simultaneous users across all OhioLink. I recommend downloading/printing the required readings ahead of time, just in case.)

Read only the following:

1. Chapter 1
  * Background
  * The Birth of Git
2. Chapter 3: Getting Started
  * Intro
  * The Git Command Line
  * Quick Introduction to Using Git (read all sections)
  * Configuration files (Intro only, may skip part on aliases)
3. Chapter 4: Basic Git Concepts
  * Basic concepts (read all)
  * Object store pictures
  * Git concepts at work (read all)
4. Chapter 21: Git and Github
  * Repo for Public Code
  * Creating a GitHub Repository
  * Forks
  * Creating Pull Requests
  * Managing Pull Requests
  * Coding Models

**Open Data Structures in C++**. Morin, edition 0.1G-beta

http://opendatastructures.org/ (Free access. I recommend downloading the PDF version.)

Read the following:

1. Chapter 1 (pp. 1-21)

Homework
========

1. Create an account with github.com. You may select the free account. If you want to get some free private repos, you may apply at https://github.com/edu
2. Go to https://github.com/MiamiOH-CSE274/01_Git_and_Intro and fork the repo, which will create a copy of it in your github account.
3. Install git on your computer, if you do not already have it. I recommend installing http://windows.github.com/ if you use windows, or http://mac.github.com/ if you use Mac. **HOWEVER, I highly recommend using the command-line tools for everything, and ignoring the GUI. I will not be providing help with configuring/using the GUI.**
4. Clone your repo from github to your computer. When you are at the web page for your repo, `https://github.com/[your github id]/01_Git_and_Intro`, you will see info about how to clone it. The easiest way is to go to the command line terminal, and type `git clone git@github.com:[your github id]/01_Git_and_Intro.git`
6. Complete the exercises below by modifying this file.
7. After you complete each answer, be sure to create a new commit with the changes (using `git add README.md` and `git commit -m` as appropriate). Also, be sure to upload to github frequently by using `git push`
8. If I don't see at least 4-5 commits on this homework, I'm going to be unhappy.
9. Once complete, send me a pull request. This is your official "turn in" of the homework, which I will grade.
10. Double check that you did the right thing by going to https://github.com/MiamiOH-CSE274/01_Git_and_Intro/pulls and making sure that your pull request is there, and looks like you expect. Optimism is the root of all evil.

Exercises
=========

Collaborated with Scott McCartney

#### 1. Based on the reading in the Git book, is it okay to keep your local copy of your repo on a USB drive and just carry it around? Explain why or why not. What about keeping it on the M: drive?

It is okay to carry around a USB drive with a copy of your repository as long as you have copies elsewhere, such as your M drive or on Github.

#### 2. Imagine that you come into the lab on the weekend to work on homework with friends, but you forgot to bring your USB drive with your repo on it. What should you do?

If you forget to bring your USB drive but were responsible by copying you repository, you can always clone it from Github. 

#### 3. Morin, Exercise 1.1 (p. 25). NOTE: You should not actually implement the solution with code. Instead, explain your solution using English. Pay special attention to explaining which data structure you ought to use, and why.

1. To print the lines in reverse order, store the lines using a Stack method. When printing, the last lines stored will be the first ones out. 

2. To print the lines in the manner requested in question 2, use the Stack method within a for loop that takes in 50 lines at a time.

3. To print lines in the manner asked for, use the queue method lines removes the first input once the length of the queue reaches 42. That when when you detect a blank String,
you can print the queue in the order you want.

4. By using the priority queue method, select lines that are not duplicates and write them to the output. If the line is a duplicate, donopt write it.

5. Using the priority method, only write a method to the output if there has already been an instance of it before.

6. Sort imput line in a Sset that is organized by length with the shortest lines written first. if the two lines are of equal length, write the line that was import first.

7. Keep track of the number of times a number is output, then proceed to print each element that number of times.

8. 

9.

#### 4. Your choice: Morin, Exercise 1.2, 1.3, or 1.4 (pick one)

Note: You should not need to write any real computer code for any of these. Instead, explain how you would approach the problem using a combination of English and pseudocode. The goal is to write something that is understandable by any programmer, even if the two of you have never used the same computer language. (In other words, assume the other person does not know the syntax of Java or C/C++, but knows the basic programming constructs such as for loops, if statements, variables, and so on.)

By using the pop() method in a stack, we can remove the last element in the sequence of +1s and -1s. After doing that we can add up the sum of the remaining elements to determine whether or not
the word is a Dyck word

#### 5. Define/explain each of the following terms, as they relate to git.

1. blob - A Blob is a "Binary Large Object". Blobs do not contain any meta data.
2. tree - "A tree object represents one level of directory information. It records blob identifiers, path names, 
and a bit of metadata for all the files in one directory. It can also recursively reference other (sub)tree objects
 and thus build a complete hierarchy of files and subdirectories." ("Version Control with Git")
3. commit - Essentially a comment made about the changes to your code. Used for knowing what was deleted and added and when.
4. repo - A place to store projects using git
5. hash - "Computes the object ID value for an object with specified type with the contents of the named file (which can be
 outside of the work tree), and optionally writes the resulting object into the object database. Reports its object ID to its
 standard output. This is used by git cvsimport to update the index without modifying files in the work tree. When <type> is 
 not specified, it defaults to "blob"." (Found on https://www.kernel.org/pub/software/scm/git/docs/git-hash-object.html)
