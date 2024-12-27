# Auto Quality Assurance (Still planning)

Local Private Quality Assurance Bot.

<br/>

# Introduction

## What i want?

Im a web developer. I want my application is have a good quality. I don't wanna code the testing code. I don't wanna record user interaction with visual based recorder that many testing framework provide. I don't wanna hire tester / QA person. Im so lazy. I just wanna run "one command" on my terminal and the QA bot will do all boring stuff for me.

## Basic Testing

Basically testing is just to lock the value. Theres two output of it boolean and probability. Boolean is the output that only have two value, true or false. Probability is the output that have a range of value. The probability is more complex than boolean. But, the basic idea is still the same, to lock the value.

## Existing Solution

There are several existing solutions in the market that aim to simplify the testing process, each with its own approach and limitations. Below are some of the key solutions:

[EXISTING_SOLUTION.md](EXISTING_SOLUTION.md)

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
