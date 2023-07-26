The Law of Conservation of Problems
===================================

Engineers get paid to solve problems. Designers create stunning visual experiences that dazzle users and help them solve problems. Product Managers strive to find an interesting balance between user needs and business success, capably side-stepping a number of thorny problems each time they enter a room. Managers apply their problem-solving ability and marry it with adminstrative skills to solve organisational problems.

(aside : I've recently transitioned back from full-time Engineering Management into full-time Engineering and coding, and there's a variety of blog posts I could write about "what does a manager even do" or "why do they seem to be so busy while never actually getting anything done ?")

What is a problem ?
===================

The Cambridge dictionary [link](https://dictionary.cambridge.org/dictionary/english/problem) defines a problem as "a situation , person, or thing that needs attention and needs to be dealt with or solve". I think most people would agree with such a common sense definition, but I can't help feel like there's more lurking benearth the smooth surface of this unassuming word.

The word problem entered the English language in the 14th century, via the Old French [link](https://www.etymonline.com/search?q=problem) word "problème" meaning " a difficult question proposed for discussion or solution, a riddle, a scientific topic for investigation". These are things with a clear answer, a solution that anyone could arrive at. Notice that they are abstract in nature, and deal with inquiries into the nature of truth. A question, riddle, or scientific topic is decidedly not a physical thing.

On the other hand, our modern-day english definition of "a situation, person or thing" is decidedly __not__ abstract. These two things are not the same

<meme> we are not the same </meme>

A quick review of Classical Thermodynamics
==========================================

[link](https://en.wikipedia.org/wiki/Laws_of_thermodynamics)

In physics, we have the laws of thermodynamics which describe universal truths of the energy of classical systems. We have a few interesting laws here

1. The total energy of a system remains constant, although it may be converted from one form to another.
2. Heat always moves from hotter objects to colder objects
3. At absolute zero degrees, the entrophy of a a system is zero

The astute among you may already see the metaphor I mean to bring about.

Plus ça change, plus c'est la même chose
========================================

[link](https://en.wiktionary.org/wiki/plus_ça_change,_plus_c%27est_la_même_chose)

Let's take a simple example. We are working on an application where users have to enter dates. Currently users enter dates using a text field, and someone has had the great idea for us to use a date picker. Sadly, there's no native date picker for our platform. We have two choices

1. Implement a date picker ourselves
2. Use a third-party dependency that implements a date picker

Most of us would choose the second option without thinking twice. But now we have a new problem. How do we keep the dependency up to date ?

Of course, this isn't a classical problem, because it's not solved just once. This is an on-going problem that will need addressing long after the development team moves on and the application stops getting updates. What happens if this dependency has a security vulnerability, and it's author is no longer maintaining it ? 

Of course, there's no free lunch, all we've done is trade one problem (Users cannot efficiently enter dates) and traded it for another (We have a dependency that needs to be updated regularly).


Everything is a tradeoff
========================

[link](https://www.linkedin.com/pulse/myth-engineering-trade-off-brian-anderson/)
[link](https://www.forbes.com/sites/forbestechcouncil/2020/12/16/trade-offs-in-software-engineering/)

Anyone who has ever heard "good, cheap, fast -- pick two" (or its cousin, "scope, deadline, quality -- pick two") is aware that engineering is about tradeoff management. We can choose to go fast and ship our feature this week (hell, maybe even today ?) if we use a third party dependency. But that's opening the door to breaking changes, future security vulnerabilities, cryptocurrency mining on developer machines. In the worst case scenario, the dependency updates and we have to update the rest of the application around it.

I'm not here to argue "build it" is better than "buy it / vendor it" (although that is often the case). My point here is that the problem doesn't go away, it just becomes another different problem.


A few choices examples
======================

"It's hard to find a taxicab in my town" => Uber => pollution
"I'm thirsty" => Buy a drink => how to effectively recycle the bottle ?
Unsure how to get to my destination => use a map => how do I recall this information next time ?
Too many tasks to do at once => you multitask =>  how do you avoid errors ?


But wait it gets worse
===============================

So far we've considered the conservation of problems. This is far away from the idyllic world we'd like to live in where startups and engineers solve real thorny problems, but I fear the reality may even be worse. What if, instead of conserving and trading problems, our work actually generates MORE problems ? I realized this one day when this relevant XKCD comic [link](https://xkcd.com/1171/)

What if instead of just conserving problems our work actually ... creates more problems ?

If we go back to the example of Uber, the number of problems this creates is actually quite large. Once we "solve" the problem of making it easy to find a taxi, we have many new problems on our hands

* fraud
* payroll
* keeping up to date with new laws and regulations
* employee happiness
* competition
* keeping up to date with Apple and Google mobile SDKs

Perhaps I'm allowing myself to wallow in my own pessimism here, but I can't help but wonder if there isn't some truth in the adage "I used regular expressions and now I have two problems".

Perhaps the solution isn't too far from what the Supercomputer discovers at the end of the classic 80s film Wargames. The only winning move is not to play.

<IMG> TODO
