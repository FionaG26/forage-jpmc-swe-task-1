# JPMC Task 1
## Task 1: Interface with a stock price data feed
You’ve been asked to assist with some development to add a chart to a trader’s dashboard allowing them to better identify under/over-valued stocks.

The trader would like to be able to monitor two historically correlated stocks and be able to visualise when the correlation between the two weakens (i.e. one stock moves proportionally more than the historical correlation would imply). This could indicate a potential trade strategy to simultaneously buy the relatively underperforming stock and sell the relatively outperforming stock. Assuming the two prices subsequently converge, the trade should be profitable.

Most data visualisation for our traders is built on JPMorgan Chase's Perspective data visualisation software, which is now open source. If you want to explore that, a link is provided in the resources section.

Before implementing this request using perspective, first, you’ll need to interface with the relevant financial data feed and make the necessary adjustments to facilitate the monitoring of potential trade opportunities.

## Here's what you need to do
For the first task of this project you will need to accomplish the following:

1. Set up your local dev environment by downloading the necessary files, tools and dependencies.
2. Fix the broken client datafeed script in the repository by making the required adjustments to it.
3. Generate a patch file of the changes you made
4. (optional): Add unit tests in the test script in the repository.
Submit your work
Let's get to work!

## Set up your dev environment
### Set-Up

Before you can tackle any software development task, you need to set up your development environment. You can think of your local development environment as a virtual workbench with all the tools necessary to work on your project. To set up your dev environment, follow these instructions:

1. Install python 3 to your system - any recent version of python 3 will work fine, though the most up-to-date version is advisable. If you need help with this step, check out this excellent guide from real python: https://realpython.com/installing-python/
 
2. Fork and clone the starter repo here: https://github.com/theforage/forage-jpmc-swe-task-1
IMPORTANT! Uncheck the “Copy the main branch only” box in the fork dialog on GitHub. A model answer has been provided in a separate branch from main.
if you are unfamiliar with forking, cloning, or git in general, take a look at the first two chapters of the git book here: https://git-scm.com/book/en/v2
 
3. Open the project in your IDE of choice - if you don’t have a favourite python IDE yet, take a look at Pycharm Community Edition. It’s a well-designed IDE by Jetbrains packed with features and plugins, powerful enough to work on the most complex projects, and entirely free.
 
4. Create a new virtual environment in the project root. Pycharm can do this automatically for you using the “configure python interpreter” option in settings.
 
5. Install all project dependencies. These are listed in the requirements.txt file.

## Here are some resources to help you
https://realpython.com/installing-python/

https://git-scm.com/book/en/v2

https://docs.github.com/en/get-started/quickstart/fork-a-repo

https://www.jetbrains.com/help/pycharm/creating-and-running-your-first-python-project.html

https://perspective.finos.org/


## Making changes
When you’re in a work environment, you’ll usually receive tasks in the form of engineering tickets. Here is an example of what this task looks like in the form of an engineering ticket

## Purpose
We want to process the data feed of stock A and stock B’s price to enable us to analyse when trading for the stock should occur.

## Acceptance Criteria

getDataPoint function should return correct tuple of stock name, bid_price, ask_price and price. Note: price of a stock = average of bid and ask
getRatio function should return the ratio of the two stock prices
main function should output correct stock info, prices and ratio
