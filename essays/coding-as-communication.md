---
layout: essay
type: essay
title: Coding as Communication
# All dates must be YYYY-MM-DD format!
date: 2021-02-11
labels:
- Coding Standards
- Communication
- Writing
---

Take a look at these two  snippets of `C` code:

#### Code Snippet A

> int main(int argc, char *argv[ ]) {<br>
> int a, b;<br>
> b = 0;<br>
> while (( a = getchar( ) ) != EOF ) {<br>
> if ( a == '&nbsp;&nbsp;&nbsp;' || a == '\n' || a == '\t' ) {<br>
> if ( ++b <= 1 ) putchar( '\n' );<br>
> } else { b = 0; putchar(a); }<br>
> } return 0;<br>
> }

<br>

#### Code Snippet B

> // &nbsp; Prints input one word per line.<br>
> 
> int main (int argc, char *argv[ ])<br>
> {<br>
> &nbsp;&nbsp;&nbsp;&nbsp; int input, escapes;<br>
> &nbsp;&nbsp;&nbsp;&nbsp; escapes = 0;<br>
> <br>
> &nbsp;&nbsp;&nbsp;&nbsp; // Reads input, 1 char at a time, until end-of-file is reached<br>
> &nbsp;&nbsp;&nbsp;&nbsp; while (( input = getchar( ) ) != EOF )<br>
> &nbsp;&nbsp;&nbsp;&nbsp; {<br>
> &nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp; // Check if input is a space, newline, or tab <br>
> &nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp; if ( input == '&nbsp;&nbsp;&nbsp;' || input == '\n' || input == '\t' )<br>
> &nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp; {<br>
> &nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp; // print a newline if less than 2 of space, newline, tab have been read<br>
> &nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp; if ( ++escapes <= 1 )<br>
> &nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp; putchar ( '\n' );<br>
> &nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp; }<br>
> &nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp; // Reset the escapes counter and print the input <br>
> &nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp; else<br>
> &nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp; {<br>
> &nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp; escapes = 0;<br>
> &nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp; putchar ( input );<br>
> &nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp; }<br>
> &nbsp;&nbsp;&nbsp;&nbsp; }<br>
> &nbsp;&nbsp;&nbsp;&nbsp; return 0;<br>
> }


When ran, both snippets of code will do the exact same thing - read input one char at a time and print one word per line. 
Snippet A is implemented in only 9 lines of code, while Snippet B is implemented in more than double the lines of Snippet A.
If both snippets do the same thing, then is there any significant difference between the two?
The significant difference is that Snippet A is just written to work, but Snippet B is written to work and also to communicate.

<img style="float: left;" src="../images/communication-skills.jpg" width="250">
When we write code, yes we are creating specific instructions for the computer to carry out a certain task, but many times, 
we also expect that other humans will read this code (even our future selves). In the presences of this expectation, code 
becomes more than just instructions to a machine, it becomes a document which communicates the computer instructions to other 
humans. In the code above, Snippet B is a document that communicates to the human being as well as provides instructions to 
the machine. Coding standards help us achieve the objective of communication.

Clearly Snippet B is following some type of coding standard. There is a specific placement of curly brackets, consistent
indentation, frequent use of comments, meaningful variable names, etc... These characteristics make this code easier to 
understand by more people. Take another look at both snippets of code. Which one requires less thinking to understand its
meaning? I bet 10 marbles that most people will choose Snippet B!

Outside the programming world, coding styles exist and serve the same purpose of efficient communication to other humans.
A great example of this is in our very own English language. I'm sure you have heard of the APA, MLA, and Chicago writing
styles for English. These writing styles provide explicit instructions on the use of punctuation, spacing, the use of capital
letters, and so on. By strictly following one of these English <em>coding standards</em>, the writer hopes to maximize meaning
and minimize ambiguity.

As does the English writer using the APA style when writing a paper, so should we, as coders, strive for maximum meaning 
and minimum ambiguity in our code. Let's view our code as documents of communication. Then knowledge can be passed from 
human to human with fewer constraints. This is easily done by following a respected coding style.

<br><br><br><br>