---
layout: project
type: project
image: img/unifier-logo.png
title: "Primavera Unifier C# REST Class Library & Console Application"
date: 2024
published: true
labels:
  - C#
  - REST API
  - Class Library
  - Oracle Primavera Unifier
  - Console Application  
summary: "My latest summer internship project for HART, a class library and console application prototype I built in C# to run REST API requests on Oracle Primvera Unifier."
---

## Overview
The summer of 2024 marked my second summer internship with Honolulu Authority for Rapid Transportation (HART), a semi-autonomous department of the City and County of Honolulu tasked with overseeing the construction and completion of the Honolulu rail project, now called Skyline. My first summer internship with HART was the year before, in 2023, where I worked on a project to build a business process workflow within Oracle Primavera Unifier to streamline the processes of compiling punch list items, vetting them, and overseeing their completion. Oracle Primavera Unifier, or simply Unifier, is a cloud-based project management software that HART uses to manage the construction of Skyline. The process of building the business process workflow in Unifier had little to do with my skill set as a computer science student, but it was a great learning experience in understanding how project management software works and how it can be customized to fit the needs of a project. 

After the summer 2023 internship program, I stuck around to work part-time as I returned to school up until the next summer internship in 2024. As I was learning the ins and outs of Unifier, I learned there was a way to automate record creation using web services. People who have worked for HART in the past built Python modules that leveraged Unifier's REST API to do things like create, update, and find records, download and upload attachments, as well as systems administration tasks like updating user permissions. The general idea of these libraries was to read data from a CSV file, make REST API requests to Unifier, and write the results back to a CSV file. Wanting to understand Unifier's REST API, I asked my manager to give me a project that would help me do so. What she came up with was a class library in C# that would run REST API requests on Unifier.

## The Project
The project was to build a class library in C# that would run REST API requests on Unifier. The class library would be used to build a console application that would take user input, make REST API requests to Unifier, and print the returning JSON. The class library would have methods to create, update, and find records. The console application would be a prototype that would demonstrate how the class library could be used to automate record creation in Unifier. The class library would be built in C# and the console application would be built in C# as well.

At the time, I didn't know C#, so I spent a couple weeks learning the language on top of learning Unifier's REST API. I ended up creating four libraries:
- `UnifierRestClassLibrary`: The main class library that contained the methods to make REST API requests to Unifier.
- `BusinessProcessLibrary`: A class library that contained the data fields of three business processes in Unifier: Areas, Engineer's Supplemental Instructions, and Canvassing Efforts.
- `ConsoleAppLibrary`: This class library is more of a helper library for `TestConsoleApp`, taking user input to navigate the menu, acquire integration tokens, and run REST requests.
- `TestConsoleApp`: The class that runs the console application.

I cloned the most recent state of the project from Bitbucket to my personal GitHub. You can [view the repo here](https://github.com/aldenparoni/unifier-rest-class-library).
