---
layout: post
title:      "Truthy or Falsey? A Quick Peek at Booleans."
date:       2020-04-25 15:58:05 +0000
permalink:  truthy_or_falsey_a_quick_peek_at_booleans
---


From conception in the 1800s by someone named George, to aiding programmers execute decisions in their code, Booleans are background players that are very important. In programming, the boolean is a data type that represents the values of true and false. "Truthy" is the programming convention for true, can you guess what "falsey" is?  That's right! It is the programming convention to describe the state of being false.

The boolean is most often used to implement flow control, which is the manipulation of the program based on certain conditions. For example, one can tell the program to execute a certain line of code if something is true and a different line of code if it is false. Written in Ruby, it might look something like this:

```
def some_code
     age = 101
		 
		 if age > 100
		      "Here's to another century!"
		 else
		      "Just another day, huh?"
		 end
end
```

If age is greater than 100, as it is - which makes it true, the program will output, "Here's to another century! If it isnt, as in else - which would mean it is false, the program will output, "Just another day, huh?"

If you would like to continue learning, I suggest looking into Boolean Operators. Thanks for stopping by!

