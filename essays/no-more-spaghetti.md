---
layout: essay
type: essay
title: No More Spaghetti
# All dates must be YYYY-MM-DD format!
date: 2021-04-29
labels:
  - Design Patterns
  - MVC
---

<img style="float: left; padding-right: 10px; padding-bottom: 10px" src="../images/spaghettiCode.gif" height="250" alt="spaghetti code meme"> 

Looking back on many of the programs that I have written, I noticed that I too often I have resorted to creating 
spaghetti code - unstructured and difficult-to-maintain source code. This happens from me, and who ever I am working
with for that project, tacking on code where ever we want, and creating long-winded unfocused functions. This is a 
terrible habit to be developing, and I need to stop before it becomes too ingrained into my way of thinking. I am
declaring right now that I am giving up spaghetti. That's right. **No more spaghetti code for this guy.** My goal now is 
to become very good at using design patterns, starting with the model-view-controller design pattern. 

Design patterns provide solutions to many problems associated with program structure. In the case of the
model-view-controller design pattern, the program is split into three main sections - the model, the view, and the 
controller. The *model* is for anything related to the data. This could be a database, or a JSON object, or some other
data structures. The *view* handles anything related to visualizing data and to the user interface. This is what is used
by the user to interact with the software. Finally, there is the *controller*. The controller is basically the manager
of the entire process. It takes the input from the user and gives instructions to both the *model*, and the *view*.

