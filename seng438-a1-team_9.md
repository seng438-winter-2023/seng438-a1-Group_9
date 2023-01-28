
  
  

>  **SENG 438 - Software Testing, Reliability, and Quality**

  

**Lab. Report \#1 – Introduction to Testing and Defect Tracking**

  

| Group: Group Number 9 |

|-----------------|

| Student 1 Noureldin Amer|

| Student 2 Thevin Mahawatte|

| Student 3 Saman Pordanesh|

| Student 4 Bryant Stevens|

  
  

**Table of Contents**

  

(When you finish writing, update the following list using right click, then

“Update Field”)

  
  

## **NEED TO UPDATE THE HYPERLINKS*******

  

[1 Introduction](#Introduction)

  

[2 High-level description of the exploratory testing plan](#High-level-description-of-the-exploratory-testing-plan)

  

[3 Comparison of exploratory and manual functional testing](#Comparison-of-exploratory-and-manual-functional-testing)

  

[4 Notes and discussion of the peer reviews of defect reports](#Notes-and-discussion-of-the-peer-reviews-of-defect-reports)

  
[5 How the pair testing was managed and team work/effort was divided](#How-the-pair-testing-was-managed-and-team-work/effort-was-divided)
  
[6 Difficulties encountered, challenges overcome, and lessons learned](#Difficulties-encountered,-challenges-overcome,-and-lessons-earned)

[7 Comments/feedback on the lab and lab document itself](#Comments/feedback-on-the-lab-and-lab-document-itself)

  

# Introduction

  

This project allowed us to get insight into how software testing is done within teams. Going into the project it is known amongst the team that exploratory testing is used for manual testing where developers know what to look for. Manual testing is something that is used without the use of automated tools to search for bugs. Different methods of finding bugs were explored within the team. Documentation and testing of bugs within a supplied automatic teller machine (ATM) software program is used to explore the various methods of software testing. Pair testing is a technique used to enhance the learning and testability of the program between members. Jira was used for bug tracking within the team to ensure a consistent working solution for all team members. Details about the bugs that were found across two different versions of the software are reported. Collaboration and communication were effective methods to succeed in this lab. Discussion about the supplied report document follow at the end of the document.

  

# High-level description of the exploratory testing plan

  

High-level exploratory testing

In this document, we are going to state the plan for conducting an exploratory testing of the software given to us for an Automated Teller Machine. According to the requirements provided in the Appendix, we have identified some major requirements that is crucial for the operation of this software as we will mention below. For each requirement, we came up with different methods that we will discuss as this plan progress.

  

Major requirement

  

1. Personal Identification Number (PIN) provided for each card

Bank card and the related PIN is the main method of access that you get from a ATM machine to your account. As mentioned in the requirement, to continue with transactions of this account, this is the first step to follow. When entering the PIN, there is limit of 3 invalid PINs that we can provide, and the card will be retained in the ATM machine after that. Our plan is to first test with correct PIN for each card and see if the software gives access to the account. And to check invalid access, we are planning to give one random number and two very close numbers to the provided PIN to check if it detects the validity of the PIN provided.

  

2. Depositing cash and balance inquiry

This is the next main requirement we identified from the system requirement document. To test this requirement, we are going to conduct a maximum of the 2 deposits to each account with amounts of 0$ - 100$ and 1000$ - 10 000$, and after each transaction, we are going to check the balance if that has been updated in the system. When depositing the amounts, we are going to check if the system is wiling to accept any coins which cannot be completed from a ATM machine.

  

3. Dispensing cash and balance inquiry

As mentioned in the requirements, this ATM machine is supposed to dispense cash only in multiple of 20s. we will test if the machine gives any option other than a multiple of 20s, just by entering an amount like 130$ or 250$, etc. Once we determine that it can be only a multiple of 20s, we are going to enter a reasonable value and check if the balance has been updated accurately for 2-3 three times for an account. We are also planning to test if the machine is willing to dispense money more than its current balance, because that should technically terminate the process gives an error mentioning that the user cannot dispense money beyond their balance.

  

4. Transferring money between accounts and balance inquiry

This is another facility that user gets, where they can transfer the balances between accounts. For this requirement, we are mostly going to test if the balance is being updated accurately after every transfer between accounts. We are going to conduct this test simply by 2-3 transactions.

As mentioned above, these are main requirements that we identified from this software requirement document that we are focused on testing, but we might find different errors that we did not expect to happen, which we will report as a defect and report them in the bug tracking tool.

  

# Comparison of exploratory and manual functional testing

  

The following photos illustrate the reports that were generated using Jira. When creating the bugs our group used paired testing where two members would find and report bugs to Jira while the others pair would do the same. Different bugs have different levels of severity and priority and are marked accordingly.

  

# Notes and discussion of the peer reviews of defect reports

  

When bugs were reported between team members the defects were tracked using the Jira Software. This allowed all team members to understand what version was being tested and where the bugs were being found within the program. Team members created different levels priority and severity of the tags depending on how the bugs effected the functionality and display of the program.

  

# How the pair testing was managed and team work/effort was divided

  

Our team of four members was split into two groups to achieve pair testing. Each pair had one person running the program and another member to follow along and suggest different ways to run the program looking for bugs. While the one person found bugs the other member would keep track of when and where the bug popped up. While group 1 found bugs and added them to the Jira Software bug tracker group 2 also had access to the view the same bugs. This process allowed for both groups to work independently while also allowing for them to understand where the other group was when trying to test for bugs so that multiple bugs were not reported twice within the Jira Software.

  

In the first phase of the project, prior to start testing the application using exploratory, we created a high level test-plan where we consider the system requirements to the measurements. After creating the test-plan, we started implementing it by dividing the group as two pairs, where each pair tested the application just by exploring the software with the help of test-plan.

In the second phase, we were provided with a test suites with some test cases to test the application. As provided in the instructions, we tested the version 1.0 with the provided test cases and reported the bugs we found in Jira.

In the third phase, we followed the same test cases as for phase 3, but for the version 1.1 of the application. While testing the test cases, we reported all the bugs that we found into Jira.

After finalizing all the testing of the application, we collaborated on working out the document gathering all the bug reporting finalizing the bug report.

  
  

# Difficulties encountered, challenges overcome, and lessons learned

  

One main challenge during the setup of the project was trying to understand how to setup the Jira Software to create bug tracking. First our team tried using Microsoft Azure to show bugs however this did not prove to be effective. There were too many problems with understanding how to create tags across the bug tracking. This lead the team to changing to using Jira Software for bug tracking. Lessons were learned in trying to overcome a "sunken cost". Originally the group tried to use the Microsoft Azure software but wasted too much time trying to get it to work how we wanted due to some permissions conflict on "creating tags". We overcame this challenge by switching over to Jira Software for bug tracking.

  

Creating a markdown document (.md) was a new challenge for all group members. We had all been familiar with using programs like Microsoft Word, or Google Docs to create reports so there was a bit of a learning curve. Multiple resources found online proved to be useful in both understanding the syntax of a .md file. The most difficult part of creating the document was importing the proper output from Jira that showed all the bugs that we had found within the ATM program. This was achieved by first exporting all information from Jira to a PDF. Next screenshots were taken of every individual bug and uploaded to an image hosting site where the URL was used to embed the photos into the .md file using the correct syntax.

  
  

# Comments/feedback on the lab and lab document itself

  

The lab document does not give accurate information on creating the software bug tracking. There were difficulties between all team members that did not allow us to use our time efficiently at the beginning of the project. We had gotten help from the teaching assistants during the lab time but there was still a few problems that needed to be addressed with the setup of the bug tracking software that was not evident in the lab document. A suggesting would be to have a step by step process to show us how to setup Jira or Azure to be used for bug testing.
