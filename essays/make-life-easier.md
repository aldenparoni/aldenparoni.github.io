---
layout: essay
type: essay
title: "Please... make life easier for yourself and everyone else"
# All dates must be YYYY-MM-DD format!
date: 2023-01-26
published: false
labels:
  - StackOverflow
  - Smart questions
---

In classes where independent work optimizes your learning experience, asking questions is inevitable and ultimately necessary. It hasn’t been that long since I changed my major to computer science, and I’m aware that I have some catching up to do. I am very much the same small fish I was two years ago, wagging my tiny fins in an ever-expanding ocean. Although I’ve since improved in my coding abilities, there are still times I get stumped on even the simplest things. It’s during those times when I am thankful for the convenience and helpfulness of the internet. 

For an aspiring programmer like me still learning the ropes, StackOverflow is a wonderful resource. It’s a question-and-answer forum where programmers of all skill levels can ask for help on any software engineering issue, and peers can offer suggestions on how to solve them. The concept of this website sounds awfully convenient, but convenience is taken for granted these days. Almost every conceivable question can be answered through a simple Google search. It’s a different story with technical questions. It’s not like professionals can’t be bothered to answer a novice’s question–they *are* willing to help. However, that’s not to say that they’ll spend time on a question that just wastes it. One should be able to distinguish smart questions from the not-so-smart ones. Thus, it’s important to understand how to ask clear and concise questions for everyone reading, that way you can get the best answers. 

## You probably shouldn’t be asking questions this way…
StackOverflow is surprisingly quick with closing questions that either have already been answered in other posts or are just not helpful to anyone trying to answer. This closed question in particular was of no help to either side.

Here’s the question as it shows on StackOverflow: [phone number validation conditions in javascript](https://stackoverflow.com/questions/75254328/phone-number-validation-conditions-in-javascript)

I'm working on a web form with several fields and a submit button. When the button is clicked, I have to verify that the required text boxes have been filled in and that the phone number is in the correct format. I can only accept 7 or 10 digit phone numbers, but characters such as (,), (-), etc are acceptable. If this box is empty or the phone number isn't in the correct format (not 7 or 10 numbers long, not a number) or has been left blank, I have to add a red border around the text box. This border is supposed to remain in place until the user corrects the error.

I can't get this to work properly. I have tried several different ways to go about doing this, but have gotten several different types of errors. One way seemed to work, but the red border only displayed for a second and then disappeared and the value in the textbox was reset. Would someone a little smarter than myself be able to help me with this function? Its purpose is to validate a text input in a form, a phone number field that will only accept 0-9, dash and dot. The HTML calls the function fine.

### Why is this not a helpful question?
There is an obvious lack of clarity with this question. The author of this post describes their issue without actually showing the code that could be causing it. Normally you’d expect there to be some lines of code after the first paragraph which describes what they need to do. The second paragraph could have made more sense if that was the case. If there were some code provided, then it would have been much easier for someone to point out any flaws. It was almost like I was reading the details of a homework assignment. I was confused when they asked, “Would someone a little smarter than myself be able to help me with this function?” With what code? Am I supposed to write up this function from scratch? The one person who commented on the question was nice enough to ask that the author provide code so they can actually help them work through the red-border issue. There were no answers posted to this question before it was closed.

## You’re better off asking questions this way
Here’s the question as it shows on StackOverflow: [How do I remove a property from a JavaScript object?](https://stackoverflow.com/questions/208105/how-do-i-remove-a-property-from-a-javascript-object)

Given an object:

```
let myObject = { "ircEvent": "PRIVMSG", "method": "newURI", "regex": "^http://.*" };
```

How do I remove the property regex to end up with the following myObject?

```
let myObject = { "ircEvent": "PRIVMSG", "method": "newURI" };
```

Top answer:

To remove a property from an object (mutating the object), you can do it like this:

```
delete myObject.regex; 
// or, 
delete myObject['regex']; 
// or, 
var prop = "regex"; delete myObject[prop];
```

### How is this question helpful to everyone else?
Even though this question is laid out more simply than the question before, all the necessary details are there and crystal clear. There is a singular issue that the author wants solved, and there is code provided as examples to help narrow down the possible answers. People can use the example code when writing up their answer for consistency and convenience. The reader is not left having to imagine what to do to help. This question *is* asking about a basic aspect of JavaScript, and it *was* originally posted in 2008, but it is nonetheless a smart and helpful question that can be pointed to if ever someone posts a not-so-smart question in the future.

## Know the smart questions from the not-so-smart questions
In retrospect, I probably could have searched through StackOverflow when I was starting out instead of splurging hundreds of lines of code and saying “I don’t know what’s wrong with my code” in the desperate emails I sent to my professors. Knowing what I know now, I was definitely an inconvenience to them, and I’m so much more grateful for their patience and help. Please, make life easier for yourself and everyone else on StackOverflow. If you want to ask a question, first make sure that it’s been answered before. If not, then make sure you present the issue as clearly as possible and provide code. You don’t want to embarrass yourself by doing all the wrong things and asking a not-so-smart question.
