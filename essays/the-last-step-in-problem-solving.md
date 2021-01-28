---
layout: essay
type: essay
title: The Last Step in Problem Solving
# All dates must be YYYY-MM-DD format!
date: 2021-01-27
labels:
- Forums
- Problem Solving
- Smart Questions
---

<img style="float: left;" src="gear_head.png" width="450">

I have found something truly helpful to me and to many others - [How to ask questions the smart way](http://www.catb.org/esr/faqs/smart-questions.html);
it is an essay written by Eric Steven Raymond. Clearly, as indicated by its title, the essay is about asking <em>smart</em> questions. However, I almost 
feel that a more appropriate title would be <em>The Last Step in Problem Solving.</em> 

Viewing Raymond's essay as an instruction on the <em>last step in problem solving</em> makes sense to me because when I reach the point when I am 
ready to ask for help, that is the time that I feel that I have exhausted all of my problem solving options. Now having read Raymond's essay, I see that 
the problem solving process can be extended to one more step - <em>formulating the smart question.</em> 

What does it mean to formulate a smart question? The full details are best expressed in Raymond's essay (which everyone should read), but here are the two 
key messages that I received:

#### 1. Do some research to try to really understand the problem.
This point is highlighted in the section [Before You Ask](http://www.catb.org/esr/faqs/smart-questions.html#before). Taking this to heart, you may find that
in many situations, there is no need to ask a question. For example: if the problem has to do with the behavior of a built-in python function, one solution
could be to read the python documentation about the function. Another solution could be to do a google search to find a forum post where another user has already
asked about the function. Sometimes you may find that, through your own research, you find the solution to the problem, but there will still be those times
when you really <em>must</em> ask for help. This brings us to the second point.

#### 2. Communication must be complete and concise.
When asking a question on a forum, or anywhere, it is important to understand that no one knows your experience unless you tell them about it. The readers of 
your question must be brought up-to-speed about your situation so that they can provide you with the best assistance. So, to make the question <em>complete</em>,
the relevant details about your journey must be communicated. This includes, but is not limited to, <em>how you attempted to solve the problem</em> and 
<em>what was the outcome of your attempt</em>. The <em>conciseness</em> of the question has to do with the relevance of the details. Okay now let's look at some
real examples.

## Examples

The following are links to two questions asked on [Stack Overflow](https://stackoverflow.com/). The first post is an example of a <em>smart</em> question, while
the second post is a not-so-smart question.
- [php $_POST array empty upon form submission](https://stackoverflow.com/questions/1282909/php-post-array-empty-upon-form-submission)
- [Can I use C for Object Oriented Programming?](https://stackoverflow.com/questions/9224855/can-i-use-c-for-object-oriented-programming)

We will briefly examine each post, and use the lessons from [How to ask questions the smart way](http://www.catb.org/esr/faqs/smart-questions.html) to determine
what makes the question <em>smart</em> or <em>not-so-smart</em>.

### Post I

#### php $_POST array empty upon form submission

>I have a custom Content Management System (CMS) I've built that works perfectly on my dev box (Ubuntu/PHP5+/MySQL5+). 
> 
> I just moved it up to the production box for my client and now all form submissions are showing up as empty $_POST arrays. 
> 
> I found a trick to verify the data is actually being passed using `file_get_contents('php://input');` and the data is showing up fine there -- the `$_POST`/`$_REQUEST` arrays are always empty.
> 
> I've also verified the content-type headers are correct as well via firebug (`application/x-www-form-urlencoded; charset=utf-8`).
> 
> This issue is happening regardless of whether a form is submitting via AJAX or a regular form submit. 
> Any help is greatly appreciated!

There are two great things about this post that I feel give it the classification of a <em>smart</em> question. The first thing is right in the title! The post 
title is concise, conveying the perfect amount of information. It is in the <em>object - deviation</em> style, as mentioned in the section 
[Use meaningful, specific subject headers](http://www.catb.org/esr/faqs/smart-questions.html#bespecific) of Raymond's essay; the <em>object</em> being 
<strong>php $_POST array</strong> and the <em>deviation</em> being <strong>empty upon form submission</strong>. As a reader I immediately know that the writer 
is having a problem with the php `$_POST` array, and that the `$_POST` array is deviating from its expected behavior by being empty after a form is submitted.

The second thing about this post is the completeness of the question. The writer really brings us all up-to-speed about their situation. We know their development 
environment, how they noticed the issue, and three ways in which they researched the problem in order to try to understand the issue better. 

This post was well-received, getting 29 answers and over 100 up-votes. Though lots of answers were given, it is not clear whether the poster's issue was resolved, 
as they didn't <em>accept</em> any of the answers.

### Post II

#### Can I use C for Object Oriented Programming?

>Can I use C(not C++!!!) for Object Oriented Programming?

Unlike the first post, this post wasn't received so well by the community. Its vote count is -6, and it has been closed due to it being labeled as a 
<em>duplicate</em> (the question has already been asked in another post). This post easily breaks two important rules for asking a <em>smart</em> question.

One rule is to <em>try to find an answer by searching the archives of the forum</em>. This is specified in the section [Before You Ask](http://www.catb.org/esr/faqs/smart-questions.html#before).
Another rule is to generally avoid asking yes-or-no question. This is noted in the section [Prune pointless queries](http://www.catb.org/esr/faqs/smart-questions.html#prune).

This poster's question could have easily been answered if they had bothered to use the forum's search bar. If they cannot put the effort in to finding an answer,
why should we put any effort in to posting one?

## Summary

In conclusion, if you are having trouble solving a problem, and you feel that you have exhausted all options, follow Raymond's rules for [asking smart questions](http://www.catb.org/esr/faqs/smart-questions.html).
In the process of forming the question you may find the answer, but if you do end up asking the question, it will be written in such a way that the reader will 
understand your situation. This has the potential of producing good quality answers. 

Making smart questions will make you smarter.