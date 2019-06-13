Here's what to expect:

you'll download the project starter files (one time only)
you'll run a startup script
near the end of each lesson, there will be a reading note telling you about the mini-project for that lesson
then, a series of reading notes at the end of the lesson will walk you through what you should do for that mini-project, and give you a chance to enter the answers that you get as you work through the tasks (these will look like quizzes)
you'll develop the code on your own computer based on the instructions in the reading notes
the code you write will enable you to answer the quiz questions.


Check that you have a working python installation, preferably version 2.6 or 2.7 (that’s the version that we use--other versions may work, but we can’t guarantee it). If you're using Python 3, you may find some more extensive revision of code to get things working at this time, so you may want to set up a Python 2 environment to work through the course materials.

We will use pip to install some packages. First get and install pip from here. Using pip, install a bunch of python packages:

go to your terminal line (don’t open python, just the command prompt)
install sklearn: pip install scikit-learn
-- for your reference, here’s the sklearn installation instructions
install natural language toolkit: pip install nltk
Get the source code. 

Go into the tools/ directory, and run startup.py. It will first check for the python modules, then download and unzip a large dataset that we will use heavily later. The download/unzipping can take a while, but you don’t have to wait for it to finish in order to get started on Part 1.


Create and train a SVM classifier in SVM.py. Use it to make predictions for the test set. What is the accuracy?

When training you may see the following error: UserWarning: Duplicate scores. Result may depend on feature ordering.There are probably duplicate features, or you used a classification score for a regression task. warn("Duplicate scores. Result may depend on feature ordering.")

This is a warning that two or more words happen to have the same usage patterns in the emails--as far as the algorithm is concerned, this means that two features are the same. Some algorithms will actually break (mathematically won’t work) or give multiple different answers (depending on feature ordering) when there are duplicate features and sklearn is giving us a warning. Good information, but not something we have to worry about.


If you find that the code is causing memory errors, you can also try setting test_size = 0.5 in the email_preprocess.py file.











