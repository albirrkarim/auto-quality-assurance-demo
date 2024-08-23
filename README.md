# Testing Anything

Private Quality Assurance Bot.

<br/>

# Introduction

## What i want?

Im a web developer. I want my application is have a good quality. I don't wanna code the testing code. I don't wanna record user interaction with visual based recorder that many testing framework provide. I don't wanna hire tester / QA person. Im so lazy. I just wanna run "one command" on my terminal and the QA bot will do all boring stuff for me.

## Basic Testing

Basically testing is just to lock the value. Theres two output of it boolean and probability. Boolean is the output that only have two value, true or false. Probability is the output that have a range of value. The probability is more complex than boolean. But, the basic idea is still the same, to lock the value.

## Existing Solution

There are several existing solutions in the market that aim to simplify the testing process, each with its own approach and limitations. Below are some of the key solutions:

**1. Automated Testing Frameworks**

Automated testing frameworks like [Selenium](https://www.selenium.dev), [Cypress](https://www.cypress.io), and [Playwright](https://playwright.dev) allow developers to automate web application testing. These tools are powerful and flexible, enabling comprehensive test coverage across various scenarios. However, they often require developers to write detailed scripts or code to define the tests, which can be time-consuming and complex.

**2. Record and Playback Tools**

Tools like [Testim](https://www.testim.io), [Katalon Studio](https://katalon.com), and [Selenium IDE](https://www.selenium.dev/selenium-ide) simplify testing by allowing you to record your interactions with the application and replay them to verify functionality, making them accessible to non-developers by eliminating the need to write code. However, these tools have their limitations. They can struggle with complex scenarios, as the recorded tests might not capture all the nuances needed for thorough testing. Additionally, these tests can become brittle when the UI changes, requiring manual intervention to update and maintain them.

**3. AI-Powered Testing Tools**

When i see the [Mabl](https://www.mabl.com) i think they provide various solution. but the pricing is hidding.
On the [Test.ai](https://test.ai/all-products) they provide various solution too. but the pricing is hidding.

**4. Codeless Testing Platforms**

Codeless testing platforms like Leapwork and TestCraft make it easier to create tests without writing code, using drag-and-drop interfaces that are user-friendly. But even with these tools, you still need to spend time manually designing and setting up your test cases.

## Solution

I made something that just need a simple configuration file and a sitemap, then you just run one command, and the QA bot will do all the boring stuff for you. 

They do all the interaction, produce the test case, run the test case, and provide the evaluation. 

They record detailed information you dont need to understand data inside test case. They provide the evaluation in a human-readable format, with a mix of data (boolean and probability) and visual (screenshots showing where and when the bot detected an error).

It’s like having a QA person that does all the work for you, so you can focus on developing your application.

How it works:

- First, They will just run, do all interaction, and produce some test case.
- Later, They will run the test case and doing evaluation.

# Use Case

- Lock functionality
- Detect Lagging
- Detect react forever loop rerender UI
- Detect FPS drop
- Record Memory Leak
- Detect page changes, classname modification with detailed information @ 500 ms
- Detect dead link, button, and form
- Stress Testing:  Giving random, maximal, minimal and wierd value to input field (they), do hardcore interaction ( fast clicking, fast type), and see how your application can handle it
- Mixed interaction (click, type, scroll, etc)
