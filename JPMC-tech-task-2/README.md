# JPMC-tech-task-2/
## JPMorgan Chase & Co. frameworks and tools
Typically, traders monitor stock prices and trading strategies by having data displayed visually on their screens in chart form. Often these charts will be accompanied by alerts that notify users when certain events occur or when preset price thresholds are hit.

JPMorgan Chase created the Perspective tool over many years to allow users to present and manipulate data feeds visually in web applications.

Perspective provides a set of flexible data transforms, such as pivots, filters, and aggregations. It utilises bleeding-edge browser technology such as Web Assembly and Apache Arrow and is unmatched in browser performance. It is engineered for reliability and production-vetted on the JPMorgan Chase trading floor. Now it’s available to the development community as an open source library. If you want to explore that, a link is provided in the resources section.

## Here is your task
In this task you'll focus on the following: 

1. Set up your local dev environment by downloading the necessary files, tools and dependencies.
2. Fix the broken typescript files in repository to make the web application output correctly
3. Generate a patch file of the changes you made.
Submit your work

Let's go!

## Set up
Just like in the last task, you need to get your local development environment up and running. Given that you completed task 1, you should already have python installed and be familiar with git.

1. First, fork and clone the project repo: https://github.com/theforage/forage-jpmc-swe-task-2
Remember to uncheck the “Copy the main branch only” box in the fork dialog on GitHub. A model answer has been provided in a separate branch from main.
2. Create a new virtual environment in the project root. Pycharm can do this automatically for you using the “configure python interpreter” option in settings.
3. Install all project python  dependencies. These are listed in the requirements.txt file.
 
In this task, we will be working with javascript in addition to python. Javascript has a handy package manager called npm, which handles package tracking, discovery, installation, and removal. We will be using it to install a series of javascript dependencies to your machine. If you already have access to npm on your system, you can skip this step. Otherwise, you will need to acquire it by following the instructions here (npm comes bundled with nodejs): https://nodejs.dev/en/learn/how-to-install-nodejs/
For this project to work, you must have node 18.10.0 installed on your machine. Ensure you have the correct version by running “node -v” in your terminal. If you do not, consider using nvm to install the correct version for you.
 
4. Install the necessary dependencies by running `npm install` from the project repo
 
5. Start the python server by running server3.py from the project repo like so: python datafeed/server3.py (note it’s important you run it from the root of the project repo)
 
6. Start the client by running `npm start` from the project repo

## Here are some resources to help you
https://nodejs.dev/en/learn/how-to-install-nodejs/

https://jpmorganchase.github.io/perspective/

https://github.com/jpmorganchase/perspective/

## Now it's time to make changes!
When you’re in a work environment, you’ll usually receive tasks in the form of engineering tickets. Here is an example of what this task looks like in the form of an engineering ticket.

## Purpose:

The objective of this task will be for you to fix the client-side web application so that it displays a graph that automatically updates as it gets data from the server application (see Before and After images below). Currently, the web application only gets data every time you click on the 'Start Streaming Data' button and does not aggregate duplicated data.

## Acceptance Criteria:

This ticket is done when the graph displayed in the client-side web application is a continuously updating line graph whose y-axis is the stock’s top_ask_price and the x-axis is the timestamp of the stock. The continuous updates to the graph should be the result of continuous requests and responses to and from the server for the stock data.
This ticket is done when the graph is also able to aggregate duplicated data retrieved from the server

To make the requisite changes, follow this step-by-step guide below.

https://cdn.theforage.com/vinternships/companyassets/Sj7temL583QAYpHXD/JiwEkbBq8pFwMRYLc/1664363857852/task_2_guide.docx.pdf

https://cdn.theforage.com/vinternships/companyassets/Sj7temL583QAYpHXD/JiwEkbBq8pFwMRYLc/1678221840319/how-to-make-a-patch-file.pdf
